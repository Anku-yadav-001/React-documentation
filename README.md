# React-documentation

1. React:-React is a JavaScript library for building user interfaces that simplifies the communication
          between developers and the DOM API.

2. Who made React?
=> React is created by "Jordan Walke", an engineer who was working for facebook.

3. What is Babel?
=> Babel is a free and opens-source transcompiler that is mainly used to convert ES6 code into backwords-compatible javascript code that can be run by older javascript engines.

4. How does Babel convert html code in React into valid code?
=> JSX code is not directly understandable by browsers, as they expect javascript. Babel comes into play to transform JSX code into regular javascript code.
This process is usually performed by a Babel preset like @babel/preset-react.
JSX-code
[
    let element =<h1>Hello, let's working with react</h1>
]
JavaScript-code
[
    let element=React.createElement("h1", null, "let's working eith react")
]

5. What is ReactDOM used for? Write an example?
=> ReactDOM is a package in react that provides methods for working with DOM.

The main method provided by ReacrDOM is render().

let App=()=>{
    return(<>
    <p>Hello,everyone</p>
    <h1>THis is h1 tag</h1>
    </>)
}
ReactDOm.render(<App/>,document.getElementById("someid"))

6. What are the packages that you need to import for react to work with?
=> There are some packages, we have need to import for work with react.
a. ReactDOM-If we are use JSX code in our react code we have need Babel to transplit our code into plan javascript
("<script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>").

b.React-It is the javascript library for building user interfaces
("<script src="https://www.unpkg.com/react@18.2.0/umd/react.development.js"></script>").

c.react-dom-It is used to works with DOM.
("<script src="https://www.unpkg.com/react-dom@18.2.0/umd/react-dom.development.js"></script>").

7. How do you add react to a web application?
=> a. Set up a javascript that lets you use the JSX syntax, split your code into modules with the import/export, and use packages for the npm package regidtry.

b.Render your react components where you e=want to see them on the web page. 

8. What is React.createElement?
=>React.createElement is a fundamental method of React JS. The main use of React.createElement is the creation of a react component. It is the Javascript format for creating react components. Also, the JSX react component when transpired invokes this only method for creating the component.
React.createElement(type,property,children)
React.createElement("div",claaName=myclass",children="This is div tag").

9. What are the three properties that createElement accept?
=>There are three properties that the createElement accept

a. Type(name of the tag)
  React.createElement('div')

b. Properties(idName,className,style)
  React.createElement('div',{className:'myclass'})

c. Children(content inside the tag)
   React.createElement('div',{className:'myclass'},children:'Hello this is div tag').


10. What is the meaning of render and root?
=> "render" refers to the process of converting a React component into its corresponding representation in the DOM.The ReactDOM.render() function is a key method for rendering React components. 

"root" commonly refers to the DOM element where the main React component is rendered.