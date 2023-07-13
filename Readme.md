• React is a JavaScript library.
• CDN?
• Cross origin?
• We are importing 2 scripts:
    ○ react.development.js : Core of the React library algorithm.
    ○ react-dom.development.js: React library which is useful for DOM modification. 
• Why we need 2 files?
    ○ As react doesn't only work on DOM. It is also work on mobile phone using React Native. As it use different function/method.
    ○ So for DOM modification perspective we are using react-dom.development.js library.
• How to create Element and when we should use React or ReactDOM?
    ○ `const heading = React.createElement("h1", {}, "Heading Text"); `
        § As h1 is created inside react that's why we are using "React.createElement".
        § {} is for adding attribute for an element i.e. {id:"heading"}
        § console.log(heading); // It give us an object. Heading is an react element and react element is just an Object.
    ○ `const root = ReactDOM.createRoot(document.getElementById("root"));`
        § We have to put h1 element inside the DOM or the browser so that's why we are using ReactDOM library function. 
        § It will create the root first. 
    ○ `root.render(heading);`
        
Rendering the heading element inside the root.