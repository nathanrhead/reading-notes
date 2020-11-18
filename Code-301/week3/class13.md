# Code 301 | Sending Form Data

## Class 13 Reading Notes

### [MDN: Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data)

I. Introduction: "This article looks at what happens when a user submits a form — where does the data go, and how do we handle it when it gets there? We also look at some of the security concerns associated with sending form data."

II. Client-server architecture

- "The <form> element defines how the data will be sent" from the client to the server.

- "The two most important attributes [of the form element] are action and method."

III. The Action and Method Attributes

- Action takes a URL or a server route that contains a url in its callback. "The action value should be a file on the server that can handle the incoming data, including ensuring server-side validation."

- "The method attribute defines how data is sent. The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method."
IV. GET and POST

- "The GET method is the method used by the browser to ask the server to send back a given resource." It's sent as a key-value pair appended to the browser and takes its name from the name attribute of the input element and its value from the value attribute of the same input element, and looks like this: www.wesite.sample/?key1=value1&key2=value2.

- POST is "the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request." The form data is appended in the body of the request (req.body). 

V. Viewing HTTP Requests

- In Chrome, it's under network > headers in the developer tools. 

- Don't send passwords using GET, because they'll be displayed in the URL. 

- Large amounts of form data should be sent using PUT, because browsers limit the size of URLs. 

VI. Retrieving the Data on the Server Side

- Regardless of method, "the server receives a string that will be parsed in order to get the data as a list of key/value pairs."

- It's recommended that you use a framework to make your server-side life easier. 

VII. Sending Files (not text)

- Files are considered "binary data," while all other data is text.

- The enctype attribute "lets you specify the value of the Content-Type HTTP header included in the request generated when the form is submitted," telling the server what kind of data to expect. "By default, its value is application/x-www-form-urlencoded. In human terms, this means: 'This is form data that has been encoded into URL parameters.'"

- The 3 extra steps required to send files

    - "Set the method attribute to POST because file content can't be put inside URL parameters."
    - "Set the value of enctype to multipart/form-data because the data will be split into multiple parts, one for each file plus one for the text data included in the form body (if text is also entered into the form)."
    - "Include one or more `<input type="file">` controls to allow your users to select the file(s) that will be uploaded."

VIII. Security

- "HTML forms are by far the most common server attack vectors," the problems coming not from the forms, but from how the server handles the data being sent. 

- Be paranoid: never trust your users.

    - "All data that comes to your server must be checked and sanitized. Always. No exception."
    - "Things to watch out for are character sequences that look like executable code (such as JavaScript or SQL commands)."
    - "Limit the incoming amount of data to allow only what's necessary."
    - "Sandbox uploaded files. Store them on a different server and allow access to the file only through a different subdomain or even better through a completely different domain."

### [Useful Reference for Forms from htmlreference.io](https://htmlreference.io/forms/)

### [Video Reference for Styling Forms](https://www.youtube.com/playlist?list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK)

[<--back](301week3.md)

[<--home-->](../../README.md)
