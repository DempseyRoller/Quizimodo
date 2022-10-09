Quizimodo
=========

The Quizimodo is an app built for answering questions in various topics,
and keeping track of your progress.

Instructions:
-------------
1. Chose a topic from four alternatives
2. You will be given a question regarding that topic and a handful of answer opitons.
3. Chose an option and the app will tell you if it was the correct one or not.
4. The application will show how many questions you've answered and how many of them were correct.


Challenges in development:
--------------------------
1. The harderst challenge I have I think was with futures. I took a wrong turn somewhere and started playing with FutureProviders to try to fix the issue of repeated api calls when resizing the app. Switching between mobile and desktop layout was especially frustrating, but in the end I rewrote all the code with FutureBuilders. Not completely satisfied with it yet, but it works 95% like it should. Refreshing the window still does a new api call and resets the StateProviders.

2. Updating StateProviders from inside a FutureBuilder isn't quite as simple as one would think. Found a fix for this from the internet which used Future.delay method. Not 100% why it works, but I think I at least know why it didn't work.

3. Knowing what to separete as a widget and what not. And especially how much you can generalize. At one moment I had different custom button widgets for all three screens, but in the end I decided and succeeded in turning them into one general purpose button. In this version there's still a few places I'm wondering if I'd like to extract the widget or not.
