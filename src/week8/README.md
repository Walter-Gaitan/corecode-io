# React & Node - Week 9

## Week goal 🏁



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


## Week challenges (Wednesday) 💻



## Week challenges (Thursday) 💻

