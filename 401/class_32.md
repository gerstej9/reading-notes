# Code 401 Class 32 Reading Notes

## What does a component's lifecycle refer to?
* A component's lifecycle refers to it's mounting, updating, unmounting and error handling
* [Source Reactjs.org](https://reactjs.org/docs/react-component.html)

## Why do you sometimes need to "wrap" functions in useCallback when called from within useEffect?
* UseCallback helps to prevent a function from being declared everytime useEffect is called
* [Source Stack Overflow](https://stackoverflow.com/questions/57156582/should-i-wrap-all-functions-that-defined-in-component-in-usecallback#:~:text=useCallback%20will%20help%20in%20avoiding,caused%20by%20recreation%20of%20functions.&text=You%20are%20specifying%20a%20function%20as%20a%20dependency%20to%20useEffect%20.)

## Why are functional components prefereed over class components
* Functional components provide greater readibility, ease of testing, and end up being plain javascript without state or life-cycle hooks. They are considered best practices
* [Source David Joch on Medium](https://djoech.medium.com/functional-vs-class-components-in-react-231e3fbd7108#:~:text=Functional%20component%20are%20much%20easier,you%20to%20use%20best%20practices.)

## What is wrong with the following code?
```
  import React, {useState, useEffect} from 'react';

  function MyComponent(props) {
  const [count, setCount] = useState(0);
  function changeCount(e) {
    setCount(e.target.value);
  }
  let renderedItems = []
  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);
    renderedItems.push(<div key={i}>Item</div>);
  }
    return (<div>
  <input type='number' value={count} onChange={changeCount}/>
    {renderedItems}
    </div>);
  }
```
* The above code does not have an export of the function MyComponent. 

## Define the following terms
* State hook
  * A state hook consists of a setter and getter and creates a function that is able to set a certain value within state
* Effect hook
  * An effect hook results in an action whenever a specified value is changed
* Reducer Hook
  * A reducer hook is a complex version of a state hook that is used when the updated value is dependent on the previous value being change. It is also helpful when their are multiple sub-values to be changed
  * [Source Reactjs.Org](https://reactjs.org/docs/hooks-reference.html#usereducer)
  

[Table of Contents](README.md)