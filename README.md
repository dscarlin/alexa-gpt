# Alexa Skill with ChatGPT

This repository contains an example of how to use OpenAI's ChatGPT language model to create an Alexa Skill.

## How it works

This code connects to the OpenAI ChatGPT API and sends Alexa's questions to the model, which processes them and returns the answers. Then, these responses are transmitted back to Alexa and presented to the user.

The name of this assistant is Benji. You can launch it by saying:

- "Alexa, launch Benji"
- "Alexa, start Benji"

Or ask it a question directly by saying:

- "Alexa, ask Benji to tell me ..."

## Running the example

This example was developed using Amazon's ASK CLI. To run it, you will need to install the ASK CLI and configure your Amazon Developer account.

Once configured, simply run the following commands in the terminal:

```
ask configure
ask init
ask deploy
```

This will deploy your Skill to your Amazon Developer account and make it available for use with Alexa.

## Configuration

You will need to obtain an API key from OpenAI to use the ChatGPT model. More information on how to do this can be found in the OpenAI API documentation.

Once you have your API key, simply save it as an environment variable for the aws lambda function created from your first deployment.

After your first deployment copy the skill id into the ask-states.json file to ensure updating the same skill with each deployment instead of creating a new one each time.

## Final considerations

This is just a basic example of how to use ChatGPT with Alexa. You can expand this implementation to create more complex and personalized skills. Enjoy!
