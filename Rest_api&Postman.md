# REST API and Postman Basics with Examples

1. **What is a REST API?**  
A REST API (Representational State Transfer Application Programming Interface) is a set of rules and protocols that allow different software applications to communicate with each other over the internet.  

**Example:**  
A weather application uses a REST API to get real-time weather data from a weather service.

---

2. **How is data typically transferred in a REST API?**  
Data is typically transferred using JSON or XML formats. JSON is simpler and easier to read.  

**Example JSON response:**  
```json
{
    "city": "London",
    "temperature": 22,
    "unit": "Celsius"
}
```

---

3. **What are some common HTTP methods used in RESTful APIs?**  
- **GET:** Retrieves data  
- **POST:** Creates a resource  
- **PUT:** Updates a resource  
- **DELETE:** Removes a resource  

**Example:**  
```http
GET /users
POST /users
PUT /users/1
DELETE /users/1
```

---

4. **What is Postman?**  
Postman is an API testing tool with a friendly interface.  

**Example:**  
You can send a **GET** request to `https://jsonplaceholder.typicode.com/posts` in Postman to fetch fake post data.

---

5. **What are HTTP status codes?**  
They are codes returned by the server to indicate request results.  

**Example:**  
`200 OK` means the request was successful.

---

6. **Example of a commonly encountered HTTP status code:**  
`200 OK` – Request succeeded.  

**Example in fetch:**  
```javascript
fetch('https://jsonplaceholder.typicode.com/posts/1')
    .then(res => {
        if(res.status === 200) console.log("Success!");
    });
```

---

7. **What does a 404 status code signify?**  
Resource not found.  

**Example:**  
Visiting `https://example.com/nopage` returns 404.

---

8. **How can you test an API using Postman?**  
Choose the method, enter the URL, set parameters/headers/body, then click **Send**.  

**Example:**  
Send a POST request to `https://jsonplaceholder.typicode.com/posts` with JSON data.

---

9. **What are query parameters in API testing?**  
Extra data sent in the URL.  

**Example:**  
`https://api.example.com/users?age=25&city=London`

---

10. **How do you pass query parameters in Postman?**  
In the Params tab, add:  
`age` = `25`, `city` = `London`.  

**Example URL generated:**  
`https://api.example.com/users?age=25&city=London`

---

11. **What are headers in API testing?**  
Metadata sent with requests or responses.  

**Example:**  
`Content-Type: application/json`

---

12. **How do you pass data using headers in Postman?**  
Add in Headers tab:  
`Authorization: Bearer token_here`  

**Example in fetch:**  
```javascript
fetch('https://api.example.com/data', {
    headers: { "Authorization": "Bearer token_here" }
});
```

---

13. **What is the request body in API testing?**  
The part of a request that contains data.  

**Example JSON body:**  
```json
{
    "name": "John",
    "age": 30
}
```

---

14. **What does it mean to call an API from a browser using fetch?**  
It means using JavaScript’s `fetch()` to send HTTP requests.  

**Example:**  
```javascript
fetch('https://jsonplaceholder.typicode.com/posts')
    .then(res => res.json())
    .then(data => console.log(data));
```

---

15. **How can you initiate an API call from a browser using fetch in JavaScript?**  
Use `fetch()` with URL, method, headers, and body if needed.  

**Example:**  
```javascript
fetch('https://jsonplaceholder.typicode.com/posts', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ title: 'foo', body: 'bar', userId: 1 })
})
.then(res => res.json())
.then(data => console.log(data));
```
