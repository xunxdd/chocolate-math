# Chocolate Math Game

A little fun game full of whimsical math word questions. Best suited for kids who love both math and chocolates. The game is also equipped with sounds of cheers whenever you answer your questions correctly, or sighs if you answer the question wrong.


# Installation

```bash
	npm install
```

# Sample Conversations
>
/*
Examples:

 Example 1:
 User: Alexa ask chocolate math
 Alexa: Welcome to chocolate Math Land. [sound of game start] ... How many math questions would you like to have?
 User: Five
 Alexa: Five questions that is. Question 1: Tommy has 5 ninja figures, Peter has 2 ninja figures. How many ninja figures do Tommy and Peter have together?
 User: Seven
 Alexa: You answered Seven. [sound of Cheers] ... You now have 10 chocolates. Question 2 ...
 ...
 ...
 Alexa: Good job. [sound of Game over] You have completed the chocolate Math game.  You have earned 50 chocolates. It was a pleasure playing with you. Come to visit Jolly Rancher Math Land soon. Goodbye!


 Example 2:
 User: Alexa open chocolate math
 Alexa: Welcome to chocolate Math Land. [sound of Game start] ... How many math questions would you like to have?
 User: Ten
 Alexa: Ten questions that is. Question 1: Tommy has 5 ninja figures, Peter has 2 ninja figures. How many ninja figures do Tommy and Peter have together?
 User: Seven
 Alexa: You answered Seven. [sound of beep] ... Then answer is wrong. You now have 0 chocolates. Question 2 ...
 ...
 ...
 Alexa: Good job. [sound of Game over] You have completed the chocolate Math game.  You have earned 50 chocolates. It was a pleasure playing with you. Come to visit Jolly Rancher Math Land soon. Goodbye!
*/

# Video Demo

[![IMAGE ALT TEXT HERE](https://i.ytimg.com/vi/oA_NJw17ul8/default.jpg?sqp=CPy668MF&rs=AOn4CLD7Elwvg_GQKU-jnWuGmmr-kDINSQ)](https://www.youtube.com/watch?v=oA_NJw17ul8)

# Notes

- The app is built using [alexa-server-app by Matt Kruse] (https://github.com/matt-kruse/alexa-app).
- Server side code / food look up using google place api in node js
- Use SSML to include audio

### Intents
```
{
  "intents": [
    {
      "intent": "questionsTotalIntent",
      "slots": [
        {
          "name": "answerSlot",
          "type": "NUMBER"
        }
      ]
    },
    {
      "intent": "answerIntent",
      "slots": [
        {
          "name": "answerSlot",
          "type": "NUMBER"
        }
      ]
    },
    {
      "intent": "answerOnlyIntent",
      "slots": [
        {
          "name": "answerSlot",
          "type": "NUMBER"
        }
      ]
    },
    {
      "intent": "AMAZON.StartOverIntent",
      "slots": []
    },
    {
      "intent": "AMAZON.HelpIntent",
      "slots": []
    },
    {
      "intent": "doNotKnowIntent",
      "slots": []
    },
    {
      "intent": "AMAZON.StopIntent",
      "slots": []
    },
    {
      "intent": "AMAZON.CancelIntent",
      "slots": []
    },
    {
      "intent": "AMAZON.RepeatIntent",
      "slots": []
    }
  ]
}
```

### Utterances

```
questionsTotalIntent	{answerSlot} questions
answerIntent	The answer is {answerSlot}
answerOnlyIntent	{answerSlot}
doNotKnowIntent	Don't Know
doNotKnowIntent	Not Sure
doNotKnowIntent	I do not know
doNotKnowIntent	I don't know
```

## History

- 0.0.1 - Dec 22, 2016
  - Launch and enjoyed by little kids