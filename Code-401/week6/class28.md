# Code 401 | Component Composition

## Class 28 Reading Notes

I. Research Questions

- Can a parent component access the state of a child component?: Not directly, but a child can certainly pass what it's storing in state back to the parent as the argument of a function passed from the parent.

- What can be passed along in a prop variable?: data or functions.

- How can a child component “know” the state of another component?:

II. Vocabulary

- Component props: "Props stands for “properties,” and they are used in a React application to send data from one React component to another React component" (["The beginner’s guide to mastering React props"](https://blog.logrocket.com/the-beginners-guide-to-mastering-react-props-3f6f01fd7099/))

- Component state: "The [sic] state is an instance of [a] React Component Class[,] [which] can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the [s]tate of a component is an object that holds some information that may change over the lifetime of the component (geekforgeeks.org).

- Application state:"Application State (also known as Program State) represents the totality of everything necessary to keep your application running.  When we refer to application state we are normally referring to the state of the program as it exists in the contents of its memory" (["What is State and Why Does it Matter?"](https://thedaylightstudio.com/blog/2018/03/14/what-is-state-in-web-application-development))

III. Preview Links

- ["These are the concepts you should know in React.js (after you learn the basics)"](https://www.freecodecamp.org/news/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030/)
- ["A quick intro to React’s props.children"](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)
- ["Composition vs Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)
- [React's Testing Library: API Example](https://testing-library.com/docs/react-testing-library/example-intro/)

IV. Questions

1. Which 3 things had you heard about previously and now have better clarity on?

- What props stand for (i.e., properties);
- What props.children are: "... used to display whatever you include between the opening and closing tags when invoking a component"; used when the children aren't known in advance (I think).
- Testing (a very little, anyway).

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- componentDidUpdate();
- React-redux (? What is it and why do we need it?);
- Composition vs. inheritance.

What are you most excited about trying to implement or see in action?: REST-y in all its final glory, assuming I ever figure it out and complete it Future self, I'm feeling pretty low right now about all of this.

[<--back](401week6.md)

[<--home-->](../../README.md)
