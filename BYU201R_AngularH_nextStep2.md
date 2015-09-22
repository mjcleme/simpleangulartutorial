Great! we should have have a simple user form that allows us to add styled user avatars

Let's take a moment to consider here some additional features we may like with our user avatar:
1. what if a user doesn't want to upload an avatar? We don't want to show a broken image. We may want to make sure our avatars still look ok by using a default avatar instead.
2. what about different avatar sizes to use on the main profile page, the navigation, or a user registry? How do we tell our avatar to render differently?
3. What if later we added usernames and also wanted to display that within our `avatar`

Can you see how this may get messy quickly trying to handle this within our templates and mainCtrl? Also, doesn't it just feel wrong that these general purpose things should be worried about avatar stuff?

It would be nice hide away all of the style, behavior, and implementation details into a neat package labeled `avatar component` and let that worry about all of this.

We will now refactor our code to use an Angular directive instead