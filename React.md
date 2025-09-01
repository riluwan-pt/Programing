# ReactJS

1.  **How does ReactJS facilitate the development of Single Page
    Applications?**\
    ReactJS facilitates SPA development by allowing developers to create
    reusable UI components. These components can be composed together to
    build complex user interfaces, and React's virtual DOM efficiently
    updates the view when the underlying data changes, enhancing
    performance.

2.  **What is ReactJS?**\
    ReactJS is a JavaScript library for building user interfaces,
    particularly for single-page applications. It allows developers to
    create reusable UI components and efficiently manage the state of
    their applications.

3.  **How does ReactJS differ from other JavaScript frameworks?**\
    Unlike traditional MVC frameworks, ReactJS emphasizes a
    component-based architecture, making it easier to build and maintain
    complex UIs. It also uses a virtual DOM for efficient rendering,
    resulting in better performance.

4.  **What is styling components using a separate CSS file in
    ReactJS?**\
    Styling components using a separate CSS file in ReactJS involves
    separating the styling code from the component code into distinct
    files. This allows for better organization and maintenance of styles
    within a React application.

5.  **How do you link a separate CSS file to a React component?**\
    To link a separate CSS file to a React component, you import the CSS
    file at the top of the component file using the `import` statement.
    For example:\

``` javascript
import './ComponentStyles.css';
```

6.  **What is Styling using module.css in ReactJS?**\
    Styling using module.css in ReactJS refers to the practice of
    encapsulating CSS styles within individual component files using the
    `.module.css` extension. This approach helps in avoiding global
    style conflicts and provides better modularity and maintainability
    for React applications.

7.  **Why is it advantageous to use module.css for styling in
    ReactJS?**\
    Using module.css helps maintain component encapsulation, enhances
    code readability, and minimizes the risk of style clashes between
    different parts of the application.

8.  **Can you explain how to import and use a module.css file in a React
    component?**\
    To use a module.css file in a React component, you import it at the
    top of the component file like so:\

``` javascript
import styles from './ComponentName.module.css';
```

Then, you can apply the styles to elements within the component using
the styles object, such as:

``` jsx
<div className={styles.container}>
```

9.  **What are CSS classes in ReactJS?**\
    CSS classes in ReactJS are used to apply styling to elements in the
    user interface.

10. **Why is it beneficial to use separate CSS files for styling React
    components?**\
    Using separate CSS files for styling React components promotes
    modularity and reusability. It also enhances code readability and
    maintainability by keeping the styling code separate from the
    component logic.

11. **What are the advantages of using props to pass data between
    components?**\
    Props provide a straightforward and efficient way to share data
    between components, promoting modularity, reusability, and
    maintainability in React applications.

12. **What is prop drilling in ReactJS?**\
    Prop drilling is the process of passing down props through multiple
    layers of components in a React application, even when intermediate
    components do not directly use those props.

13. **What is a component state variable in ReactJS?**\
    In ReactJS, a component state variable is a special type of variable
    that allows components to manage and update their own data. It's
    used to store information that can change over time, such as user
    input or dynamic content.

14. **When should you use state variables in ReactJS?**\
    State variables should be used when you need to manage and update
    data within a component that may change over time in response to
    user interactions or other events.

15. **What is an API call in ReactJS?**\
    An API call in ReactJS is a request made to an external server or
    service to fetch or send data, typically using the `fetch()`
    function or third-party libraries like Axios.

16. **How do you make an API call in ReactJS?**\
    To make an API call in ReactJS, you typically use the `fetch()`
    function or third-party libraries like Axios. You send a request to
    the desired endpoint and handle the response asynchronously.

17. **What is the useEffect hook in ReactJS?**\
    The `useEffect` hook in ReactJS is a built-in hook that allows
    functional components to perform side effects. It's commonly used
    for tasks like fetching data, subscribing to external events, or
    manually changing the DOM.

18. **How does styling with module.css differ from traditional CSS?**\
    Traditional CSS applies styles globally across all elements of a
    webpage, while styling with module.css confines styles to specific
    components, preventing unintended style conflicts.

19. **How can you use multiple CSS classes in an element in ReactJS?**\
    You can use multiple CSS classes in an element by separating them
    with a space within the `className` attribute.

20. **Why would you use multiple CSS classes in an element?**\
    Using multiple CSS classes allows you to apply different styles to
    an element or to combine styles from different classes.
