# ProdActive

![ProdActive Logo](https://raw.githubusercontent.com/pranaynaki/ProdActive/master/chromeExtension/logo.png "ProdActive Logo")

HackTX 2017

We started off reading about a John Hopkins' research study on ways to improve productivity. We then looked into how we could put these methods into practice. First, we decided on the techniques we found most essential for improving productivity, and from there, we implemented them in an integrated manner as a Microsoft Edge and Chrome extension that would be convenient and not distracting to the user.

Some of the features we successfully implemented include creating a scheduling mechanism that allows the user to plan a task from start to completion, given an estimated duration of the task. This sets us apart from other productivity apps, since we schedule tasks in terms of the time they will take to complete, as opposed to setting aside chunks of a day to finish something. This more closely simulates how normal people get work done. The scheduler automatically alerts the user when to take breaks or continue working. It also allows the user to choose between several modes of working, such as casual, productive, or time crunch. We also keep track of the time a user spends on any particular website using Chrome and Edge extensions. This allows our extension to alert the user whenever they have exceeded a certain amount of time on "unproductive" websites, such as facebook, twitter, and youtube (this can be customized by the user), and it will be able to tell what time is actually used on productive websites as opposed to leisure sites.

We integrated with Microsoft's bot framework so that users can easily schedule tasks (using text or voice commands). LUIS allowed us to extract intents from the user-inputted command using Machine Learning, and we then make an API call to the Azure server to log the task and start the timer. The Azure server is also used to aggregate user data for statistics about time spent on different websites. On the front end side, this data is displayed on a custom website that also allows users to input tasks manually, see the amount of time they have left on a certain task, and view their personal statistics in a user-friendly format.

As a next step, we can expand the project by adding analytics for the number of times a user switches between tasks.
