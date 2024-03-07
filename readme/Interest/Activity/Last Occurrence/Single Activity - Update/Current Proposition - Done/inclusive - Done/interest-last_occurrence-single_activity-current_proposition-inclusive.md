In this example, we will get the cumulative `Last Occurrence` where the `Proposition` is the `Proposition` we have assigned to our `Action` and its children, and the `Activity Type` is "AT 1". This shows us how to get the cumulative `Last Occurrence` for any case where we want to get the cumulative `Last Occurrence` for the `Proposition` we have assigned to an `Action` and its children, and an `Activity Type`.

The `Activity Type` section of the `Proposition Data Adapter` has no cumulative option, but we can replicate this functionality.

To do this we first need to create a supporting rule that gets us `Proposition Path` for the `Proposition` we want. The value of `Proposition Path` will include the full path uniquely identifying the `Actions` `Proposition` and so will not match `Propositions` with the same name.

![](interest-last_occurrence-single_activity-current_proposition-inclusive-1.png)

You can then save this rule:

![](interest-last_occurrence-single_activity-current_proposition-inclusive-2.png)

This `Proposition Name` will match the parent `Proposition` and its children as we wanted it to. To make the set-up consistant with when we want to exclude the parent, we will wrap this rule in a new rule:

![](interest-last_occurrence-single_activity-current_proposition-inclusive-3.png)

As we are aggrigating, we first need to select which aggrigation `function` we are using. We will be using `Sum of the elements in` to get the total number of times this `Activity Type` has be linked to an event.

![](interest-last_occurrence-single_activity-current_proposition-inclusive-4.png)

You will notice that as we have used this `function`, when we extern the `DIP` we are limted to only fields that return a `number` and that we are not required to apply any filters:

![](interest-last_occurrence-single_activity-current_proposition-inclusive-5.png)


We will select the rule we made to get the `Proposition Path`, and apply our `Activity Type` filter:

![](interest-last_occurrence-single_activity-current_proposition-inclusive-6.png)


We can now save our rule. Also note how there are square brackets (`[]`) around the `function` input, this is because it is taking a list.

![](interest-last_occurrence-single_activity-current_proposition-inclusive-7.png)
