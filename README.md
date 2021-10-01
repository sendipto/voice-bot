<h1 align="center" style="border-bottom: none;"> 🤖 Chatbot using IBM Watson </h1>
<h3 align="center">Node.js application using Speech to Text, Text to Speech and Assistant </h3>

## Prerequisites

1. Sign up for an [IBM Cloud account](https://cloud.ibm.com/registration/).
2. Download the [IBM Cloud CLI](https://cloud.ibm.com/docs/cli/index.html#overview).
3. Create an instance of the Speech to Text, Text to Speech and Assistant service and get your credentials:
    - Copy the `apikey` value.
    - Copy the `url` value.

## Configuring the application
1. Open the *config/config.env* file and add the service credentials that you obtained in the previous step.

```
PORT=8080

### Watson Speech to Text
SPEECH_TO_TEXT_IAM_APIKEY="***"
SPEECH_TO_TEXT_URL="https://api.***.speech-to-text.watson.cloud.ibm.com/instances/***"

### Watson Text to Speech
TEXT_TO_SPEECH_IAM_APIKEY="***"
TEXT_TO_SPEECH_URL="https://api.***.text-to-speech.watson.cloud.ibm.com/instances/***"

### Watson Assistant
ASSISTANT_APIKEY="***"
ASSISTANT_IAM_APIKEY="same as before"
ASSISTANT_URL="https://api.***.assistant.watson.cloud.ibm.com/instances/***"

### Optionally, use a non-default skill by specifying your own workspace ID or name.
workspaceId="***"

```

## Running locally

1. Install the dependencies

    ```
    npm install
    ```

2. Run the application

    ```
    npm start
    ```

3. View the application in a browser at `localhost:8080`

4. It will works like a charm
