# Code 401 | Application State with Redux

## Class 36 Reading Notes

I. Research Questions

- What are the advantages of storing tokens in “Cookies” vs “Local Storage”: The cookie is not accessible via JavaScript, so it is not so vulnerable to XSS attacks as localStorage is, though beware that cookies are limited to 4kb and some APIs require JWTs to be sent in headers, in which case local storage is your only option (["Local Storage vs Cookies"](https://dev.to/cotter/localstorage-vs-cookies-all-you-need-to-know-about-storing-jwt-tokens-securely-in-the-front-end-15id)).

- Explain third-party cookies: Third-party cookies "are stored under a different domain than you are currently visiting. They are mostly used to track users between websites and display more relevant ads between websites" (["All you need to know about Third-Party Cookies"](https://cookie-script.com/all-you-need-to-know-about-third-party-cookies.html)).

- How do pixel tags work?: it's just a function in JS that, when fires, records certain data about a user and his/her/their behavior and sends that data for processing, reporting, and use.

II. Vocabulary

- cookies: a small file with data that identifies the user, e.g., username and password.

- authorization: "Authorization is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular. More formally, "to authorize" is to define an access policy" (wikipedia).

- access control: "In the fields of physical security and information security, access control is the selective restriction of access to a place or other resource while access management describes the process. The act of accessing may mean consuming, entering, or using. Permission to access a resource is called authorization" (wikipedia).

- conditional rendering: "In React, we can create multiple components which encapsulate behavior that we need. After that, we can render them depending on some conditions or the state of our application. In other words, based on one or several conditions, a component decides which elements it will return" (["React Conditional Rendering"](https://www.javatpoint.com/react-conditional-rendering#:~:text=React%20Conditional%20Rendering,which%20elements%20it%20will%20return.)).

III. Preview Links

- ["Getting Started with Redux"](Getting Started with Redux)

IV. Questions about the Preview

A. Which 3 things had you heard about previously and now have better clarity on?

- Redux
- Pure functions
- Impure functions

B. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Redux
- Cookies
- Conditional rendering

What are you most excited about trying to implement or see in action?

- Redux

[<--back](401week8.md)

[<--home-->](../../README.md)
