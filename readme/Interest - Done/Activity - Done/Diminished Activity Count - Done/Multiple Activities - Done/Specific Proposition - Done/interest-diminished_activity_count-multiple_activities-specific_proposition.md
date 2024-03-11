In this example, we will get the `Diminished Activity Count` where the `Proposition` is "Root" and the `Activity Type` contains the text "Checkout -". This shows us how to get the `Diminished Activity Count` for any case where we are exactly specifying the `Proposition` and we want to match multiple `Activity Types`.

As we are aggrigating, we first need to select which aggrigation `function` we are using. We will be using `Sum of the elements in` to get the total number of times these `Activity Types` have be linked to an event.

![](interest-diminished_activity_count-multiple_activities-specific_proposition-1.png)

You will notice that as we have used this `function`, when we extern the `DIP` we are limted to only fields that return a `number` and that we are not required to apply any filters:

![](interest-diminished_activity_count-multiple_activities-specific_proposition-2.png)

We will apply our `Proposition` filter and then apply our `Activity Type` filter:

![](interest-diminished_activity_count-multiple_activities-specific_proposition-3.png)

We can now save our rule. Also note how there are square brackets (`[]`) around the `function` input, this is because it is taking a list.

![](interest-diminished_activity_count-multiple_activities-specific_proposition-4.png)