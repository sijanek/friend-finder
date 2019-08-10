## Friend Finder
homework wk 13 

## What does this application do

This app is compatibility-based "FriendFinder" application -- basically a dating app. However, I have created an array of made up friend-names and used images from https://www.pexels.com/search/man/. This is a full-stack app. The users are required to fill out a survey form, including their name, provide an HTTP link to their picture and they are asked to answer all questions.  After that, the results from user are compared with the answers of other users. Then the app will then display the name and picture of the user with the best overall match. The closest match will be the user with the least amount of difference.

## Technologies used
* Express (to handle the routing)
* Node.js
* Require
* Path
* API routes
* HTML routes
* Heroku

The app contains 10 questions to be answered on a scale of 1-5 (1 being Strongly Disagree and 5 being Strongly Agree):

1.  Your mind is always buzzing with unexplored ideas and plans.
1.  Generally speaking, you rely more on your experience than your imagination.
1.  You find it easy to stay relaxed and focused even when there is some pressure.
1.  You rarely do something just out of sheer curiosity.
1.  People can rarely upset you.
1.  It is often difficult for you to relate to other people’s feelings.
1.  In a discussion, truth should be more important than people’s sensitivities.
1.  You rarely get carried away by fantasies and ideas.
1.  You think that everyone’s views should be respected regardless of whether they are supported by facts or not.
1.  You feel more energetic after spending time with a group of people.


The compatibility is determined by a scoring methodology, using a following logarithm:


User 1: [5, 1, 4, 4, 5, 1, 2, 5, 4, 1]

User 2: [3, 2, 6, 4, 5, 1, 2, 5, 4, 1]

Total Difference: 2 + 1 + 2 = 5

where each answer to each question is subtracted from the same numerical answer to the same question for each Friend in the pool. The differences (all absolute values) are added together to obtain a final score. The lowest score will represent the most compatible friend.

A modal popup is constructed to display the results; the name and a photo of the best match.

Go to [Heroku](https://serene-thicket-42231.herokuapp.com/) or [GitHub](https://sijanek.github.io/friend-finder/) to check out my version of the app.

