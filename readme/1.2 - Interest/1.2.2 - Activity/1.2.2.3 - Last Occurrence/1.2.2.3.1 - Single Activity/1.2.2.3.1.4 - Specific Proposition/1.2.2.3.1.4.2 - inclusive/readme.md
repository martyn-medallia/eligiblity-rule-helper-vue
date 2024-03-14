In this example, we will get the sum of `Last Occurrences` where the `Proposition` is "Level 2" and its children, and the `Activity Type` is "AT 1".

First, we need to make a supporting rule that gets us the `Proposition Path` of the `Proposition` "Level 2". The `Proposition Name` in the `Proposition` `Data Adapter` is actually the full `Proposition Path` and so this field will be retrieved:

![alt text](image_1.png)

We can then save this rule:

![alt text](image_2.png)

This `Proposition Path` will match the `Proposition` "Level 2" and its children. In order to make our rules consistant between when we want to include or exclude the parent, we will wrap this rule is a new rule:

![alt text](image_3.png)

As we are aggrigating, we first need to select which aggrigation `function` we are using. We will be using `Latest date in` to get the latest date from the `Last Occurrence` for each matching `Proposition` & `Activity Type`:

![](image_4.png)

Next, we open the `DIP`, select the field we want:

![](image_5.png)

You will notice that as we have used this `function`, when we enter the `DIP` we are limted to only fields that return a `Datetime` and that we are not required to apply any filters.

We will select the rule we made for the `Proposition`, and apply our `Activity Type` filter:

![](image_6.png)

Finally, we save our rule:

![](image_7.png)