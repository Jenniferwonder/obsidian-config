---
title: 1 Day-React Note (Aug 18)
tags: 
status: 
started: 
closed: 
aliases: 
---
#### Time: Aug 18
#### Learning Roadmap:
1. What and why?
   - To create and reuse independent components
2. Download:
   - Node.js (Ubuntu version install error?)
      - Download: [https://nodejs.org/en/download/](https://nodejs.org/en/download/)
   - NPM
      - 
      - npm -v
      - npm install (error:)
      - npm start
   - React
      - Create React App: 
3. Create first react component: "greeting" > "bug"> "**Q: How to debug**? **(eg. spelling mistake: greeting> greeeting)**"

```jsx
import React from 'react';
import ReactDOM from 'react-dom/client';
import './index.css';
import Hello from './Hello';
import reportWebVitals from './reportWebVitals';
import "tachyons";
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <Hello greeting={"Hello React Ninjia"}/>
);
//ReactDOM.render(<Hello greeting={'Hello' + 'React Ninjia'}/>, document.getElementById('root'));
// If you want to start measuring performance in your app, pass a function
// to log results (for example: reportWebVitals(console.log))
// or send to an analytics endpoint. Learn more: https://bit.ly/CRA-vitals
reportWebVitals();
```

```jsx
import React, { Component } from 'react';
import "./Hello.css";
class Hello extends Component {
    render() {
        return (
            <div className="fi tc">
                <h1>Hello, World!</h1>
                <p>{this.props.greeeting}</p>
            </div>
        );
    }
}
export default Hello;
```

```jsx
const Hello = (props) => {
    return (
        <div className="fi tc">
            <h1>Hello World</h1>
            <p>{props.greeting}</p>
        </div>
    );
}
```

![image.png](https://cdn.nlark.com/yuque/0/2022/png/29677165/1660875331401-762a43af-7dbb-4dd9-8404-ca6143eadb6f.png#clientId=uf62f54b7-8bfa-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=250&id=u6f97b1a2&margin=%5Bobject%20Object%5D&name=image.png&originHeight=500&originWidth=2388&originalType=binary&ratio=1&rotation=0&showTitle=false&size=45009&status=done&style=none&taskId=uc9db8970-f594-4774-9f91-5fd413a8040&title=&width=1194)
4. Robotfriend
- Delete unnecessary file in React app
- 
- destructure

```jsx
import React from 'react';
const Card = (props) => {
    return (
        <div className='tc bg-light-green dib br3 pa3 ma2 grow bw2 shadow-5'>
            <img alt='robots' src={`https://robohash.org/${props.id}?200x200`}/>
            <div>
                <h2>{props.name}</h2>
                <p>{props.email}</p>
            </div>
        </div>
    );
}
export default Card;
```

```jsx
import React from 'react';
const Card = (props) => {
    const { name, email, id} = props;
    return (
        <div className='tc bg-light-green dib br3 pa3 ma2 grow bw2 shadow-5'>
            <img alt='robots' src={`https://robohash.org/${id}?200x200`}/>
            <div>
                <h2>{name}</h2>
                <p>{email}</p>
            </div>
        </div>
    );
}
export default Card;
```

```jsx
import React from 'react';
const Card = ({ name, email, id}) => {
    return (
        <div className='tc bg-light-green dib br3 pa3 ma2 grow bw2 shadow-5'>
            <img alt='robots' src={`https://robohash.org/${id}?200x200`}/>
            <div>
                <h2>{name}</h2>
                <p>{email}</p>
            </div>
        </div>
    );
}
export default Card;
```

- card component

```jsx
import React from 'react';
import ReactDOM from 'react-dom/client';
import './index.css';
import Card from './Card';
import reportWebVitals from './reportWebVitals';
import "tachyons";
import { robots } from './robots';
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <div>
    <Card id={robots[0].id} name={robots[0].name} email={robots[0].email}/>
    <Card id={robots[1].id} name={robots[1].name} email={robots[1].email}/>
    <Card id={robots[2].id} name={robots[2].name} email={robots[2].email}/>
  </div>
);
// If you want to start measuring performance in your app, pass a function
// to log results (for example: reportWebVitals(console.log))
// or send to an analytics endpoint. Learn more: https://bit.ly/CRA-vitals
reportWebVitals();
```

```jsx
import React from 'react';
import ReactDOM from 'react-dom/client';
import './index.css';
import CardList from './CardList';
import reportWebVitals from './reportWebVitals';
import "tachyons";
import { robots } from './robots';
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <CardList robots={robots}/>
);
reportWebVitals();
```

```jsx
import React from 'react';
import Card from './Card';
const CardList = ({robots}) => {
    const cardsArray = robots.map((user, i) => {
        return <Card id={robots[i].id} name={robots[i].name} email={robots[i].email}/> 
    })
    return (
        <div>
            {cardsArray}
        </div>
    );
}
export default CardList;
```

```jsx
import React from 'react';
import Card from './Card';
const CardList = ({robots}) => {
    return (
        <div>
            {
                robots.map((_user, i) => {
                    return (
                        <Card
                            key={i} 
                            id={robots[i].id} 
                            name={robots[i].name} 
                            email={robots[i].email}
                            />
                    ); 
                })
            }
        </div>
    );
}
export default CardList;
```

- searchbar (static)
   - STATE: the description of your application
   - PROP: 

```jsx
import React from 'react';
import CardList from './CardList';
import SearchBox from './SearchBox';
import { robots } from './robots';
const App = () => {
    return (
        <div className='tc'>
            <h1>Robot Friends</h1>
            <SearchBox /> 
            <CardList robots={robots}/>
        </div>
        );
    }
export default App;
```

```jsx
import React from 'react';
import ReactDOM from 'react-dom/client';
import './index.css';
import App from './App';
import reportWebVitals from './reportWebVitals';
import "tachyons";
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <App/>
);
// If you want to start measuring performance in your app, pass a function
// to log results (for example: reportWebVitals(console.log))
// or send to an analytics endpoint. Learn more: https://bit.ly/CRA-vitals
reportWebVitals();
```

```jsx
import React from 'react';
const SearchBox = () => {
    return (
        <div className='pa2'>
            <input 
            className='pa3 ba b--green bg-lightest-blue'
            type='search' placeholder='Search robots' />
        </div>
        
    );
}
export default SearchBox;
```

- searchbar (dynamic by using STATE)

```jsx
import React, { Component } from 'react';
import CardList from './CardList';
import SearchBox from './SearchBox';
import { robots } from './robots';
import './App.css';
class App extends Component {
    constructor() {
        super()
        this.state = {
            robots: robots,
            searchfield: ''
        }
    }
    onSearchChange = (event) => {
        //console.log(event.target.value);
        this.setState({ searchfield: event.target.value });
        //console.log(filterRobots);
    }
    render() {
        const filteredRobots = this.state.robots.filter(robots => {
            return robots.name.toLowerCase().includes(this.state.searchfield.toLowerCase());
        });
        return (
            <div className='tc'>
                <h1 className='f1'>RoboFriends</h1>
                <SearchBox searchChange={this.onSearchChange}/> 
                <CardList robots={filteredRobots}/>
            </div>
            );
        }
    }
export default App;
```

```jsx
import React from 'react';
const SearchBox = ({searchfield, searchChange}) => {
    return (
        <div className='pa2'>
            <input 
            className='pa3 ba b--green bg-lightest-blue'
            type='search' placeholder='Search robots'
            onChange={searchChange}
            />
        </div>
        
    );
}
export default SearchBox;
```

- App.css (using @font-face)
   - 

```jsx
/* #### Generated By: http://www.cufonfonts.com #### */
@font-face {
    font-family: 'SEGA LOGO FONT';
    font-style: normal;
    font-weight: normal;
    src: local('SEGA LOGO FONT'), url('SEGA.woff') format('woff');
    }
h1 {
    font-family: 'SEGA LOGO FONT', serif;
    font-weight: 200;
    color: #0ccac4;
}
```

- React components
   - 
      - Mounting
      - Updating
      - Unmounting 
#### Resources:
- Github portfolio template: [https://github.com/cobiwave/simplefolio](https://github.com/cobiwave/simplefolio)
- Libraries: npm install tachyon 
- VS Code React Extension Pack 
- React fragment and semantic HTML: 
- React Docs: 
- we were late before you	even came here auto
