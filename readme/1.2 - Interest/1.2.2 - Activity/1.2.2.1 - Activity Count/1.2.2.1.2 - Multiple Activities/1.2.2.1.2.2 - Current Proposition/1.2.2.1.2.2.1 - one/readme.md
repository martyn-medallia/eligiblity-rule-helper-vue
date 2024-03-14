In this example, we will get the `Activity Count` where the `Proposition` is the Proposition we have assigned to the `Action` that `MXO` is evaluating the `Eligibility` for, and the `Activity Type` contains the text "Checkout -".

As we are aggrigating, we first need to select which aggrigation `function` we are using. We will be using `Sum of the elements in` to get the total number of `Activity Count` for each matching `Proposition` & `Activity Type`:

![](image_1.png)

Next, we open the `DIP`, select the field we want:

![](image_2.png)

You will notice that as we have used this `function`, when we enter the `DIP` we are limted to only fields that return a `number` and that we are not required to apply any filters.

Next, we will apply our `Proposition` filter, we do this by using the option `Current proposition`, and apply our `Activity Type` filter:

![](image_3.png)

Finally, we save our rule:

![](image_4.png)