# JSX and Babel in React

## What is JSX?

JSX (JavaScript XML) is a syntax extension for JavaScript.
It allows writing HTML-like code directly in JavaScript files.

```jsx
const element = <h1>Hello, JSX!</h1>;

# features of react -- 
     it is declarative   as it uses JSX (html inside javascript) 
            basically a syntax extension to javascript 
    
     it is more of a component baseed approach 
     very efficient for creating a single page applications using virtual DOM approach.



Why use JSX?
Cleaner syntax for creating UI components

Easier to read and maintain

Looks like HTML but compiles to React.createElement()

What is Babel?
Babel is a JavaScript compiler that converts JSX into standard JavaScript.

-----------------------------------------------------------------------------------

example of a simple reach app in html file 

<!DOCTYPE html>
<html>
  <head>
    <title>React Component</title>

    <!-- React CDN -->
    <script src="https://unpkg.com/react@18/umd/react.development.js" crossorigin></script>

    <!-- ReactDOM CDN -->
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js" crossorigin></script>

    <!-- Babel CDN (so we can use JSX directly in browser) -->
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
  </head>
  <body>
    <div id="root"></div>

    <script type="text/babel">
      // ? Functional Component: App
      function App() {
        return (
          <div>
            <h1>Hello, React!</h1>
            <p>This is a paragraph rendered using a functional component.</p>
            <ul>
              <li>First item</li>
              <li>Second item</li>
              <li>Third item</li>
            </ul>
          </div>
        );
      }

      // ? Render App component into root div
      const root = ReactDOM.createRoot(document.getElementById('root'));
      root.render(<App />);
    </script>
  </body>
</html>
