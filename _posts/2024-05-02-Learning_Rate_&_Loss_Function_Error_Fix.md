### Issues with Finding a Learning Rate

Today I was trying to find an optimal learning rate for my model when I ran into a runtime error:

> grad can be implicitly created only for a scalar outputs.

This took a bit of research, but it turns out this error typically occurs when the loss function doesn’t reduce to a scalar value. This is important for calculating gradients during the learning rate search.

Now the loss function I was using is the CrossEntropyLoss function with the parameter `reduction=none`. This tells the function not to reduce the loss to a scalar value. Go figure that’s my issue.

Removing that parameter solved my issue. How good 😊
