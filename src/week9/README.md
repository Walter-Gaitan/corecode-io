# React & Node - Week 9

## Week goal 🏁

Learn about React/Node.JS and its capabilities

---
## Week challenges (Monday) 💻

### Easter egg list in ReactJS
```javascript
import React from 'react';


export const EggList = (props) => {
  return <ul>{props.eggs.map((egg, index) => <EasterEgg key={index} name={egg}/>)} </ul>
};

export const EasterEgg = (props) => {
  const name = props.name;
  return( <li key={name} >{name}</li>)

};
```

## Week challenges (Tuesday) 💻

1. Read about Node.js
2. The V8 Javascript Engine is an interpreter created by Google Chrome to run your Javascript code independently of the browser. This enhances the performance since you don't need to wait for the script to give a response to load the rest of the webpage.
3. NVM is a tool used to download Node.js and manage the versions you have installed. The beauty of NVM is that it lets you keep multiple versions of Node.js to run specific projects
4. Depending on you are using Javascript or Node.js, the default modules would be ES modules or CommonJS modules respectively. This standardization affects whether you are working with Javascript or Node.js, also, ES modules are synchronous while CommonJS asynchronous.

## Week challenges (Wednesday) 💻

### Answer the question: Are APIs only available on the Internet?
When we talk about APIs, we usually speak about their web versions, but that doesn't mean that those are the only ones. In different words, *All Web Services are APIs but not al APIs are Web Services*
You can also use APIs using only local files, because at the end, this is just a way for two applicacions to communicate with each other. That doesn't require a connection to the internet to happen, but it can happen within a single device.

## Week challenges (Thursday) 💻

### Postman alternatives

1. Thunder Client

*Website:* [Thunder Client](https://www.thunderclient.com/)

The first one is the one that I recommend the most since is just an extension that you can use in VS Code. It is very similar to Postman so, if you already know this tool the learning curve is not really high. The best is that it is 100% free.

2. Testfully

*Website:* [Testfully.io](https://testfully.io/)

This is a great option to start with since you don't need to install any software, because it runs in the browser. It stores your request in the cloud, so you can use re-tests. It also offers a free plan with unlimited team members

3. Insomnia

*Website:* [Insomnia Rest](https://insomnia.rest/)

This is an open source API client that let's you use it for free and the base price starts at $5. With it, you can centralize and automate tests, build API pipelines, define multiple environments, and so on. This one has a very simple interface, which makes it a better alternative to Postman if you're just a begginer, it also loads faster.