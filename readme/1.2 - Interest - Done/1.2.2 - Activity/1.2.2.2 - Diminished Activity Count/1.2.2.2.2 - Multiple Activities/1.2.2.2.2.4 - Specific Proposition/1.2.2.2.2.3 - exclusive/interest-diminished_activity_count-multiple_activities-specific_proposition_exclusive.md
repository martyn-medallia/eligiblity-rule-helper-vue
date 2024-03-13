In this example, we will get the cumulative `Diminished Activity Count` where the `Proposition` includes "Level 2"'s children but not the `Proposition` "Level 2" itself, and the `Activity Type` contains the text "Checkout -". This shows us how to get the cumulative `Diminished Activity Count` for any case where we want to get the cumulative `Diminished Activity Count` for a spcific `Proposition`'s children, but not itself, and we want to match multiple `Activity Types`.

The `Activity Type` section of the `Proposition Data Adapter` has no cumulative option, but we can replicate this functionality.

To do this we first need to create a supporting rule that gets us `Proposition Name` for the `Proposition` we want. The value of `Proposition Name` will include the full path uniquely identifying the selected `Proposition` and so will not match `Propositions` with the same name.

![](interest-diminished_activity_count-multiple_activities-specific_proposition_exclusive-1.png)

You can then save this rule:

![](interest-diminished_activity_count-multiple_activities-specific_proposition_exclusive-2.png)

This `Proposition Name` will still match the parent `Proposition`. If we want to exclude the parent `Proposition` we need to add an `/` onto the `Proposition Name`. We do this by using the `Function` `Concatenate` to append the `/` to the end:

![](interest-diminished_activity_count-multiple_activities-specific_proposition_exclusive-3.png)

As we are aggrigating, we first need to select which aggrigation `function` we are using. We will be using `Sum of the elements in` to get the total number of times these `Activity Types` have be linked to an event.

![](interest-diminished_activity_count-multiple_activities-specific_proposition_exclusive-4.png)

You will notice that as we have used this `function`, when we extern the `DIP` we are limted to only fields that return a `number` and that we are not required to apply any filters:

![](interest-diminished_activity_count-multiple_activities-specific_proposition_exclusive-5.png)


We will select the rule we made to get the `Proposition Path`, and apply our `Activity Type` filter:

![](interest-diminished_activity_count-multiple_activities-specific_proposition_exclusive-6.png)


We can now save our rule. Also note how there are square brackets (`[]`) around the `function` input, this is because it is taking a list.

![](interest-diminished_activity_count-multiple_activities-specific_proposition_exclusive-7.png)
