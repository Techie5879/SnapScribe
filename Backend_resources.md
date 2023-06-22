# Backend Development Resources
This file contains a comprehensive list of resources that can be valuable for backend development in the SnapScribe project. These resources cover various aspects such as backend frameworks and API development.

## Backend Frameworks
For both of the suggested frameworks, basic familiarity with Python is necessary.  
- [Flask](https://flask.palletsprojects.com/en/2.3.x/) - A lightweight and versatile Python web framework. Flask provides a simple yet powerful foundation for building web applications and APIs.  

- [CS50 2020 lec 9 - Flask](https://youtu.be/x_c8pTW8ZUc) - Great tutorial for building a Flask web app. Holds your hand all the way through and explains all the basic concepts. Probably all the Flask you need to learn for this project. But remember that they use Jinja syntax which we won't be using or needing, it is old. We will need to connect it to a React frontend.

- [Django](https://docs.djangoproject.com/en/4.2/) - A high-level Python web framework known for its "batteries included" approach. It offers robust features for building scalable and secure web applications.

The preferred method for this project is a Flask web server serving the ML model, but you can use Django if you're more comfortable with that. The high level concept remains the same with any of the two, which is that you will have to build routes in the web app to serve predictions.

## HTTP Basics

- [CS50 2020 Lec 8 - Web](https://youtu.be/5g0x2xv3aHU) - Great introduction to HTTP protocols and type of requests like GET and POST, their differences and when each one is used. Also gives an intro as to what headers are. Great starting point.

- [HTTP MDN Docs](https://developer.mozilla.org/en-US/docs/Web/HTTP) - Very in-depth. Do not need to learn all of this. Don't even try to remember or read through this whole thing. Use as and when needed as reference material.

- [HTTP Headers MDN Docs](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers) - Same as above, use as reference material.

## Sending Requests and Fetching Responses

- [Requests in Python](https://docs.python-requests.org/en/latest/) - Requests is an elegant and simple HTTP library for Python. You might need to use this.

For sending and fetching requests in React, you'll need the following (basically the following will communicate between the frontend and backend - user uploads image to the frontend, that is sent to the backend and the backend responds with a caption that is then displayed by the frontend).  
- [Form Handling - Net Ninja](https://www.youtube.com/playlist?list=PL4cUxeGkcC9gZD-Tvwfod2gaISzfRiP9d) - Videos #14-32 are essential. Won't take long. Definitely watch them.

- [Axios](https://axios-http.com/docs/intro) - A popular JavaScript library for making HTTP requests from web browsers or Node.js. Axios is great for the handling of responses that it provides.

- [Axios freeCodeCamp Tutorial](https://www.freecodecamp.org/news/how-to-use-axios-with-react/) - Guide to get started with Axios and React.

- [Fetch API MDN Docs](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) - The MDN Web Docs guide to the Fetch API, a modern browser feature for making asynchronous HTTP requests.

- [Asynchronous JavaScript](https://www.freecodecamp.org/news/asynchronous-javascript) - Lean about Promises, Callbacks, and asynchronous code handling in JavaScript. You will be able to apply this in React after that.
