In this example, we will get the `Activity Count` where the `Proposition` is the Proposition we have assigned to our `Action` and the `Activity Type` contains the text "Checkout -". This shows us how to get the `Activity Count` for any case where we want to match multiple `Activity Types`, and the `Proposition` has been assigned to the action.

As we are aggrigating, we first need to select which aggrigation `function` we are using. We will be using `Sum of the elements in` to get the total number of times these `Activity Types` have be linked to an event.

![](interest-activity_count-multiple_activities-current_proposition-one-1.png)

You will notice that as we have used this `function`, when we extern the `DIP` we are limted to only fields that return a `number` and that we are not required to apply any filters:

![](interest-activity_count-multiple_activities-current_proposition-one-2.png)

We will apply our `Proposition` filter, we do this by using the option `Current proposition`, and then apply our `Activity Type` filter:

![](interest-activity_count-multiple_activities-current_proposition-one-3.png)

We can now save our rule. Also note how there are square brackets (`[]`) around the `function` input, this is because it is taking a list.

![](interest-activity_count-multiple_activities-current_proposition-one-4.png)