# Code 401 | Props and State

## Class 27 Reading Notes

I. Research Questions

A. Does a deployed React application require a server?: Yes. (No? Maybe?)

B. Why do we prefer to test a React application at the behavior level rather than the unit level?: because testing for the right outcome given certain user behaviors yields a more accurate picture of the code's state than does testing to see whether a piece of code is doing a thing on the way to reaching the desired outcome.

C. What does npm run build do?: "npm run build creates a build directory with a production build of your app. Set up your favorite HTTP server so that a visitor to your site is served index.html, and requests to static paths like /static/js/main.<hash>.js are served with the contents of the /static/js/main.<hash>.js file" ([Create-React-App.dev](https://create-react-app.dev/docs/deployment/)).

D. Describe the actual composition and architecture of a React application: It is designed to depend on one point of access, or parent, with children, called components, that manage various aspects of the app. The idea is to make the code modular to such an extent that a change to one part of a comonent won't affect the overall running of the application.

II. Vocabulary

- BDD: behavior-driven development = developing based on what a user will be doing on a site and testing for expected results of that behavior (click, input, etc.).

- Acceptance Tests: "An acceptance test is a formal description of the behavior of a software product, generally expressed as an example or a usage scenario. ... Similar to a unit test, an acceptance test generally has a binary result, pass or fail" (agileallegiance.org).

- Mounting: "Mounting is a process by which the operating system makes files and directories on a storage device (such as hard drive, CD-ROM, or network share) available for users to access via the computer's file system" (wikipedia.org).

- Build: "In a programming context, a build is a version of a program. As a rule, a build is a pre-release version and as such is identified by a build number, rather than by a release number. ... As a verb, to build can mean either to write code or to put individual coded components of a program together" (SearchSoftwareQuality.TechTarget.com).

III. Preview links

- ["Understanding React 'setState'"](https://css-tricks.com/understanding-react-setstate/)

- ["Handling Events"](https://reactjs.org/docs/handling-events.html)

- [React: Forms](https://reactjs.org/docs/forms.html)

- [React: State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

- [React: Components and Props](https://reactjs.org/docs/components-and-props.html)

- ["The Complete Beginner's Guide to Testing React Apps (Updated for 2020"](https://thomlom.dev/beginner-guide-testing-react-apps/)

IV. Questions

A. Which 3 things had you heard about previously and now have better clarity on?

- The history behind and purpose of React;
- Use cases for React;
- How to make an API call in React.

B. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Setting up the other three http calls (put, update, delete (and get one by id));
- Testing in React;
- Handling events in React.

C. What are you most excited about trying to implement or see in action?: handling events in React.

[<--back](401week6.md)

[<--home-->](../../README.md)
