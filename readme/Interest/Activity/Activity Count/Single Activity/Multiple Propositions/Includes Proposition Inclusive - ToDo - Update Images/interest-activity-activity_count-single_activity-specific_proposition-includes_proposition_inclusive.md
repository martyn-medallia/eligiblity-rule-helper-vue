In this example, we will get the cumulative `Activity Count` where the `Proposition` includes "Level 2" and its children and the `Activity Type` is "AT 1". This shows us how to get the cumulative `Activity Count` for any case where we are exactly specifying the parent `Proposition` and the `Activity Type`.

The `Activity Type` section of the `Proposition Data Adapter` has no cumulative option, but we can replicate this functionality.

To do this we first need to create a supporting rule that gets us `Proposition Name` for the `Proposition` we want. The value of `Proposition Name` will include the full path uniquely identifying the selected `Proposition` and so will not match `Propositions` with the same name.

![](interest-activity-activity_count-single_activity-specific_proposition-includes_proposition_inclusive-1.png)

You can then save this rule:

![](interest-activity-activity_count-single_activity-specific_proposition-includes_proposition_inclusive-2.png)

As we are aggrigating, we first need to select which aggrigation `function` we are using. We will be using `Sum of the elements in` to get the total number of times this `Activity Type` has be linked to an event.

![](interest-activity-activity_count-single_activity-specific_proposition-includes_proposition_inclusive-3.png)


You will notice that as we have used this `function`, when we extern the `DIP` we are limted to only fields that return a `number` and that we are not required to apply any filters:

![](interest-activity-activity_count-single_activity-specific_proposition-includes_proposition_inclusive-4.png)


We will select the rule we made to get the `Proposition Path`, and apply our `Activity Type` filter:

![](interest-activity-activity_count-single_activity-specific_proposition-includes_proposition_inclusive-5.png)


We can now save our rule. Also note how there are square brackets (`[]`) around the `function` input, this is because it is taking a list.

![](interest-activity-activity_count-single_activity-specific_proposition-includes_proposition_inclusive-6.png)
