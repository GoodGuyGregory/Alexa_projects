# Alexa Projects

Must be build on the Alexa Skills Kit

Alexa Skills kit is Available to Node.js, C#, Java and Python

Initial Project will be using Java Script for the skills 

## SDK for Node.js  

In order to build a skill for Alexa you will need to use the Alexa Skills Kit for your language below is Node.js  

https://github.com/alexa/alexa-skills-kit-sdk-for-nodejs

# Anatomy of Custom Skills:  

needs a **Custom Interaction Model**: Basically the ability for the user to be udnerstood by Alexa  by training it to respond in certain ways 

Innvocation -> Skill Service

Innvocation: for example: "Alexa, ask **Treehouse** whats the Meaning of HTML"  
                          "Alexa, play **Spotify**   
The Bold words represent Invocation Names: which should be used in combination with an Utterance. 
For example "Alexa, play **Weekly Discovery** from Spotify" is an example of a wake word ***Alexa*** combined with an Invocation ***Spotify*** combined with an **Utterance** and or **slot** of  ***Discover Weekly***.  

## More Technical Gargon  

Anatomy of an Alexa Request
Examples:

Alexa, ask Treehouse, what does CSS mean?

Alexa is the wake word.

Alexa, ask Treehouse, what does CSS mean?

Treehouse is an example of the invocation name, the name of the custom skill.

Alexa, ask Treehouse, what does CSS mean?

what does CSS mean is an example of an utterance. The command or question routed to your skill service.  

------------------------------  

## Creating Your Skill: 

In order to actually create a skill you need to build an *User Interaction Model* for you skill. Starting by creating some example Phrases.  

Terms: HTML, CSS, Javascript  

**Alexa, ask Treehouse...

Examples: 

What does HTML mean..
What does HTML stand for
What's the definition of CSS
What is the definition of Javascript
What Are some Common Programming languages?  
What the definition of Javascript.  

Intents: Get Definition or Explaination.  

-----------  

## Actual Development:  

Visit this site and sign up for a free account https://developer.amazon.com/

### Invocation: ###   
This is the first step you need to follow on the appplication site, Creating a two word  max invocation that Alexa can understand  

### Intent: ###   
Next building an intent Schema is the intents of what your application will do in other words the types of skills or tasks it can accomplish This program is written in a JSON format

**example:** 

`{  

  "intents": [  
    {  
      "intent": "GetDefinition",  
      "slots": [  
        {  
          "name": "Term",
          "type": "LIST_OF_TERMS"
        }
      ]
    },
    {
      "intent": "AMAZON.HelpIntent"
    },
    {
      "intent": "AMAZON.StopIntent"
    },
    {
      "intent": "AMAZON.CancelIntent"
    }
  ]
}`

--------  

## Testing:  

You can test your programmed skills by using the site https://echosim.io/welcome  

## Certification:   

to create a compliant certified Service skill you must have the following:  

**Required Intents**  
  -LaunchRequest  
  -AMAZON.StopIntent  
  -AMAZON.CancelIntent  
  -AMAZON.HelpIntent  
  
--------  

## Certification Specs:  

### Icons: 
 
 Small: 108px x 108px
 Large: 512px x 512px
