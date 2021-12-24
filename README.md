# react-better-alerts

**react-better-alerts** is a npm library that gives you acces to React component to easly manage alerts in your react app

# Install

```
npm install react-better-alerts
```

# How to Use

in your `App.js` File:

```jsx
import { AlertWrapper } from "react-better-alerts";

function App() {
  //...code
  return <AlertWrapper>/*Code...*/ Code</AlertWrapper>;
}

export default App;
```

# In any other Component

```jsx
import { Alert } from "react-better-alerts";

function MyComponent() {

  function createAlert() {
    Alert.createAlert({
      icon: "warnning",
      color: "red",
      title: "Alert !",
      message: "Welcome in the Alert MADAFACKU",
      callback: () => console.log("Clicked");
    });
  }

  return (
    <div>
      <h1>Welcome to MyComponent !</h1>
      <button onClick={createAlert}>Create Alert</button>
    </div>
  );
}

export default MyComponent;
```
