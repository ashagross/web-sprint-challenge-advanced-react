1. Explain how to build stateful class components.

class Car extends React.Component {
  constructor() {
    super();
    this.state = {color: "red"};
  }
  render() {
    return <h2>I am a Car!</h2>;
  }
}

If there is a constructor() function in your component, this function will be called when the component gets initiated.
The constructor function is where you initiate the component's properties.
The constructor function is also where you honor the inheritance of the parent component by including the super() statement, which executes the parent component's constructor function, and your component has access to all the functions of the parent component (React.Component).


2. Describe the different phases of the component lifecycle.
Mounting - puts element into the DOM
Updating - Component updates whenever theres a change to the state or props
Unmounting - component gets removed from DOM

3. Demonstrate an understanding of class component lifecycle methods.
Mounting is the birth of the component, updating is whenever there are changes, and unmounting is the death of the copmonent.

4. Define stateful logic.
Stateful logic is any code that uses state, but in the case of hooks it is defined as a behaviour created with the use of one or more hooks.

5. Describe how to test a React component with React Testing Library.
-Create a test.js file
-Add test case assertion (what to expect in jest) which turn out to be red(errors) or green(successful).
-npm test 