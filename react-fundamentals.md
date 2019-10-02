### Remember

Answer these on your own, then compare answers as a group

1.  What is React?
    // React is a JavaScript library for building user interfaces. It is the view layer for web applications. At the heart of all React applications are components.

2.  What is create-react-app?
    // create-react-app is a tool (built by developers at Facebook) that gives you a massive head start when building React apps. It saves you from time-consuming setup and configuration. You simply run one command and Create React APP Sets up the tools you need to start your React project.

    - boilerplate
    - a tool that helps get a starting react envionrment off the ground and ready to start coding
    - configuration free

3.  What is Component Based Architecture?
    // Component-based architecture focuses on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties.
    - encapsulation

4)  What is JSX?
    // JSX is an XML/HTML-like syntax used by React that extends ECMAScript so that XML/HTML-like text can co-exist with JavaScript/React code. ...Unlike the past, instead of putting JavaScript into HTML, JSX allow us to put HTML into JavaScript.

```js
function Cool(props) {
  retunr <label>{props.label}</label>;
}
```

should transpile to

```js
function Cool(props) {
  return react.createElement("label", null, props.label);
}
```

5.  What is the virtual DOM?
    // The virtual DOM(VDOM) is a programming concept where an ideal, or "virtual", representation of a UI is kept in memory and synced with the "real" DOM by a library such as ReactDom. This process is called reconciliation. ... They may also be considered a part of "virtual DOM" implementation in React.

6.  What is unidirectional (one-way) data flow?
    // Unidireactional Data Flow is not a concept unique to React, but as a JavaScript developer this might be the first time you hear it. In general this concept means that data has one, and only one way to be transferred to other parts of the application.

- react uses Parent => Child data flow

### Understand

Discuss these questions in pairs if you have a 4-person group

7.  Summarize what happens when you run `create-react-app my-app`

8)  Explain what this code does:

```jsx
import React from "react";

const Mentor = props => (
  <div className="mentor-container">
    <h1 className={props.title === "Lead Mentor" ? "lead" : ""}>Tim Biles</h1>
    <ul>
      <li>Fort Worth, TX</li>
      <li>My email address is timbilestimbiles@gmail.com</li>
    </ul>
  </div>
);

export default Mentor;
```

9.  Explain how data is passed from a parent component to a child component.

### Apply

Try these on your own, but work together if you start to get stuck.

10. Use `create-react-app` to create a new React application called `student-directory`

11. Use the code from `Mentor` above to create a new functional, stateless component called `User` with a list of friends. Hard code the list of friends, do not use state or props.

### Analyze, Evaluate, Create

Discuss these questions as a group

12. What are the benefits and drawbacks of using a tool like create-react-app?

13. Compare and contrast JSX with other templating options, such as those used in Angular or Vue

14. Compare and contrast one-way data flow with two-way data binding.
