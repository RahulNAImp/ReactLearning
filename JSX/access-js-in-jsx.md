example is 

note : prepare the react app 1st then do use this syntax

import './App.css';


whenever you want to render the dynamic concent you can create a function any type arrow or normal one 
and make sure you return whatever your function does 


function sum() {
  let a = 10+4;
  return a;
}

 const App = () => {
  return (
    <div className="App">
     <>
      <h1>About React Fragments</h1>
      <ul>
        <li>unlike just creating a parent div everytimme you can create a subsequient child class</li>
        <li>this is what the unrordered list looks like </li>
        <li>sum of the numbers is {sum()}</li>

        // while calling the custom function you need to call it inside a braces and then how normally you cann a function with paranthesis 

      </ul>
     </>
    </div>
    
  );
}

export default App;


----------------------------------------------------------------------------

how to render the arrays or object inside the jsx 

