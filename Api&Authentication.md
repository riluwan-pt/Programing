# JavaScript, APIs, and Authentication

1. **What is the purpose of calling an API from a browser using fetch?**  
   The purpose of calling an API from a browser using fetch is to retrieve data or perform actions on a server without requiring a full page reload, allowing for more dynamic and interactive web applications.  
   **Example:**  
   ```javascript
   fetch('https://api.example.com/data')
     .then(response => response.json())
     .then(data => console.log(data))
     .catch(error => console.error('Error:', error));
   ```

2. **What is a POST API?**  
   A POST API is a type of HTTP request method used to submit data to be processed by a server. It's commonly used for creating or updating resources on a server.  
   **Example:**  
   ```javascript
   fetch('https://api.example.com/users', {
     method: 'POST',
     headers: { 'Content-Type': 'application/json' },
     body: JSON.stringify({ name: 'John Doe', email: 'john@example.com' })
   })
   .then(response => response.json())
   .then(data => console.log(data));
   ```

3. **What is authentication?**  
   Authentication is the process of verifying the identity of a user, typically through the use of credentials such as usernames and passwords.  
   **Example:** Entering a username and password on a login form.

4. **What is authorization?**  
   Authorization is the process of determining whether a user has permission to access certain resources or perform certain actions within a system or application.  
   **Example:** Only admin users can delete a post in a forum.

5. **How does authentication differ from authorization?**  
   Authentication verifies the identity of a user, while authorization determines what actions or resources that authenticated user is allowed to access.  
   **Example:**  
   - Authentication: Logging in with username/password  
   - Authorization: Admin panel access granted only to admin users.

6. **What are some common methods of authentication?**  
   Common methods of authentication include username/password authentication, biometric authentication (such as fingerprint or facial recognition), and token-based authentication.  
   **Example:** Google login using OAuth tokens.

7. **How does authentication typically work in JavaScript-based REST APIs?**  
   Authentication in JavaScript-based REST APIs often involves using tokens, such as JSON Web Tokens (JWT), which are sent along with each request to verify the user's identity. These tokens are typically generated upon successful login and are validated on the server side.  
   **Example:**  
   ```javascript
   fetch('https://api.example.com/profile', {
     headers: { 'Authorization': 'Bearer your_jwt_token' }
   })
   .then(res => res.json())
   .then(data => console.log(data));
   ```

8. **What is JWT? How does JWT work?**  
   JWT stands for JSON Web Token. It's a compact and self-contained way for securely transmitting information between parties as a JSON object. JWT works by digitally signing the payload (the data being transmitted) with a secret key, which can then be verified by the recipient to ensure its authenticity.  
   **Example Structure:**  
   ```
   header.payload.signature
   ```

9. **What are the components of a JWT?**  
   A JWT consists of three main parts:  
   - **Header:** `{ "alg": "HS256", "typ": "JWT" }`  
   - **Payload:** `{ "userId": 123, "role": "admin" }`  
   - **Signature:** Encrypted string for verification.

10. **How does a login API work in JavaScript?**  
    A login API in JavaScript typically involves sending user credentials (such as username and password) to a server, which then validates the credentials. Upon successful validation, the server responds with a token or session identifier, granting the user access to protected resources.  
    **Example:**  
    ```javascript
    fetch('https://api.example.com/login', {
      method: 'POST',
      headers: { 'Content-Type': 'application/json' },
      body: JSON.stringify({ username: 'user1', password: 'pass123' })
    })
    .then(res => res.json())
    .then(data => {
      localStorage.setItem('token', data.token);
    });
    ```

11. **What are browser storages in JavaScript?**  
    Browser storages in JavaScript are mechanisms provided by web browsers to store data locally on the user's device.  
    **Example:** localStorage, sessionStorage, cookies.

12. **What is local storage in JavaScript?**  
    Local storage is a browser storage mechanism in JavaScript that allows data to be stored persistently on the user's device without an expiration date. `localStorage` is a web storage API provided by browsers to store key-value pairs locally within the user's browser.  
    **Example:**  
    ```javascript
    localStorage.setItem('theme', 'dark');
    console.log(localStorage.getItem('theme')); // dark
    ```

13. **How does session storage work in JavaScript?**  
    Session storage is similar to local storage but stores data only for the duration of the page session. Once the browser tab is closed, the data is cleared.  
    **Example:**  
    ```javascript
    sessionStorage.setItem('sessionUser', 'John');
    console.log(sessionStorage.getItem('sessionUser'));
    ```

14. **What are cookies in JavaScript?**  
    Cookies are small pieces of data stored on the user's device by the web browser. They are commonly used for tracking and session management purposes.  
    **Example:**  
    ```javascript
    document.cookie = "username=John; path=/; max-age=3600";
    console.log(document.cookie);
    ```

15. **What are the main differences between local storage and session storage?**  
    Local storage persists data indefinitely until explicitly removed, whereas session storage only persists data for the duration of the page session. Additionally, local storage data is accessible across browser tabs, while session storage is limited to the current tab.

16. **How can you access and manipulate browser storages in JavaScript?**  
    Browser storages can be accessed and manipulated using the `localStorage`, `sessionStorage`, and `document.cookie` objects in JavaScript, respectively.  
    **Example:**  
    ```javascript
    localStorage.removeItem('theme');
    sessionStorage.clear();
    ```

17. **What is a token in web development?**  
    In web development, a token is typically a piece of data used for authentication and authorization purposes. It's often generated by the server and sent to the client to identify the user's session.

18. **How do you store a token in localStorage using JavaScript?**  
    To store a token in localStorage, you can use the `setItem` method like this:  
    ```javascript
    localStorage.setItem('token', 'your_token_here');
    ```

19. **Why would you store a token in localStorage?**  
    Storing a token in localStorage allows for persistent storage of authentication tokens within the user's browser, enabling seamless authentication across page reloads and browser sessions.
