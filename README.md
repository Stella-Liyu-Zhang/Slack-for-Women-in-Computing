# Slack for Women in Computing

In this project, I created a full stack Real time chat application using getstream-io and ReactJS with registration and authentication. I also implemented the backend using NodeJS and Express.

I wanted to build an app from women in tech. However, I just implemented some basic functions of chatting in slack or discord, like Signing up, logging in, channels with a specific group of people added, direct messaging, etc. 

I'm still figuring out how to securely limit my user group to female and non-binary users in my app. 

## Setup
### To run the client side, navigate to the client folder by
```
cd client
```
if you haven't created the react-app yet, feel free to do so by typing: 
*(./ specifies the directory where we are creating our react app.)*
```
npx create-react-app ./
```
, then run
```
npm start
```

### To run the server side, navigate to the server folder by
```
cd server
```
if you haven't intialized the server yet, feel free to do so by typing
```
npm init -y
```
, then run
```
npm run dev
```
## User Stories: 
1) As a woman in tech, I want to join a community with only fellow female tech workers, to talk in a more free, comfortable, and confident way. 

## Competitive Product Analysis:
- Tbh Slack is much better than my app. I cannot compete with it. 
- And you could make a female-only slack group too, as long as you know anyone in real person.
- So I'm still thinking about how to solve users' pain points in my app.

## Major UIs:

### Sign up form:
The sign up form will require the user's
- full name
- username
- a profile image url
- phone number
- password authentication
![Sign up form](./imgs/image%20(2).png)

### Sign in form:
The sign in form will query in the database to see if your info (username and password) inputted matches. If matching, the user will be successfully signed in.
![Sign in form](./imgs/image%20(3).png)

### Direct Messaging box in web:
The real time chat box has some highlights including:
- Sending texts
- Sending medias
    - Sending gifs and emojis
    - Sending documents
    - Sending pictures
- CRUD Functionalities
    - Edit message
    - Delete Message
And other functions including:
    - Pin a message
    - Reply in a thread
    - React to a message with emoji.
![Sign in form](./imgs/chatboxweb.png)
![EMOJIS](./imgs/emojis.png)
### Direct Messaging box in mobile:
![Sign in form](./imgs/chatbox.png)
### channel in web:
![Sign in form](./imgs/channel.png)
### channel in mobile:
![Sign in form](./imgs/channel2.png)

## client side npm dependencies we installed include:
- stream-chat 
- stream-chat-react 
- universal-cookie

## server side npm packages we installed include:
- bcrypt
- crypto
- dotenv
- express
- getstream
- stream-chat
- nodemon
- twilio
