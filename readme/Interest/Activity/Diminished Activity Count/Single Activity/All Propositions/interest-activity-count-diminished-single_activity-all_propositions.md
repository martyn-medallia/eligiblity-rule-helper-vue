In this example, we will get the `Activity Count` where the `Proposition` can be anything and the `Activity Type` is "AT 1". This shows us how to get the `Activity Count` for any case where we are exactly specifying the `Activity Type`, but the `Proposition` can be anything.

As we are aggrigating, we first need to select which aggrigation `function` we are using. We will be using `Sum of the elements in` to get the total number of times this `Activity Type` has be linked to an event.

![example-activity-count-any-prop-1]

You will notice that as we have used this `function`, when we extern the `DIP` we are limted to only fields that return a `number` and that we are not required to apply any filters:

![example-activity-count-any-prop-2]

We will leave the `Proposition` filter blank, and apply our `Activity Type` filter:

![example-activity-count-any-prop-3]

We can now save our rule. Also note how there are square brackets (`[]`) around the `function` input, this is because it is taking a list.

![example-activity-count-any-prop-4]
