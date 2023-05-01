# Questions and Answers

## How Web Apps Works?

- 1. [HTTP & Servers](https://blog.isquaredsoftware.com/2020/11/how-web-apps-work-http-server/)
- 2. [Client Deployment & Development](https://blog.isquaredsoftware.com/2020/11/how-web-apps-work-client-dev-deployment/)
- 3.  [Browsers, HTML & CSS](https://blog.isquaredsoftware.com/2020/11/how-web-apps-work-html-css/)
- 4. [JavaScript & DOM](https://blog.isquaredsoftware.com/2020/11/how-web-apps-work-javascript-dom/)
- 5. [Ajax, APIs & Data Transfers](https://blog.isquaredsoftware.com/2020/11/how-web-apps-work-ajax-apis-data/)

## what the heck is the components anyway?
- A **component** is self-contained, independent, and reusable piece of code that bundles the UI and it's related functionality.
- Though, In _React.js_, **components** are the _main_ building blocks of  the _UI_.
- **Components** are nothing but _JavaScript Functions_ that return a particular piece of UI based on the input.

## 2 Types of Components :)
- **Function Components**.
    - A **function component** is basically a **JavaScript function** that returns a **React element(JSX)**.
    - _They_ are used when you _don't need to managestate or use lifecyle methods_.
    -```javascript
        function Greeting(props) {
            return <h1>Helo, {props.name}!</h1>;
        }
        ```
    - Alternatively, you can use an **arrow function** to define a _function component_.
    -```javascript
        const Greeting = (props) => {
            return <h1>Hello, {props.name}!</h1>
        }
        ```
    - To use a _component_ later, you first _export_ it, by doing something like this :
    ```javascript
        export default Greeting;
        ```
    - Then, when you want to use that, particular component, you _import_ it, by doing something like this : 
    ```javascript
        import Greeting from './Greeting';

        function App() {
            return (
                <div className="App">
                    <Greeting name='Devanshu' />
                </div>
            )
        }
        ```
    - **NOTE** : _The name of the component should always start with a capital letter_.
- **Class Components**.
    - 
