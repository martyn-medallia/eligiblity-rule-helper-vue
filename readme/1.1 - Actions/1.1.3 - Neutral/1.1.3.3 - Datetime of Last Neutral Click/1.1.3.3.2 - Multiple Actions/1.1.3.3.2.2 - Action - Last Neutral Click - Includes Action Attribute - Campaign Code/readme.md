In this example we will get the most recent `Datetime of Last Neutral Click` for all `Actions` whose name includes "Usecase - Popup".

First we need to make a supporting rule that gets us the `Campaign Code` assigned to the `Action` that `MXO` is evaluating the `Eligibility` for:

![alt text](image_1.png)

As we are aggrigating, we first need to select which aggrigation `function` we are using. We will be using `Latest date in` to get the value of `Datetime of Last Neutral Click` from the matching `Actions`:

![alt text](image_2.png)

Next we open the `DIP`, select the field we want:

![alt text](image_3.png)

After we apply our filter:

![alt text](image_4.png)

Finally, we save our rule:

![alt text](image_5.png)