# abb-frontend

A basic front-end using Vue3 that receieves data from the abb-backend via WebSockets

## Run (after starting the back-end app first)

```
npm install
npm run serve
```

## Requirements
- NodeJS v16.0.0
- npm 7.10.0

### About

Although the app uses the Vue framework it doesn't display anything!  I decided to focus mainly on the [back-end](https://github.com/louis-sanchez/abb-backend) since I am applying as a backender and if I had extra time use Vue to display the data via Components (spoiler-alert:  I didn't).  The purpose of this app is primarily to test the back-end is successfully sending the generated Parts via WebSocket communication (open console to view logs).

### If I had more time I would ...

- Finish the frontend
- Write some tests (although we could also write these together in a followup interview!)
- Dockerize

## Feedback

- The assignment is very vague and is missing key information such as what type of sample data should be used, but I am guessing that is not the
important part of the exercise.

- This is *not* a backend test!  I definitely recommend ABB find a seperate way to challenge NodeJS backenders.  If I had more direction on how to create the backend I could have
gotten more done in less time.  
