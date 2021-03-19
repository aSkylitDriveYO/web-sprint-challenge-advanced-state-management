# Interview Answers

Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?

The issue prop drilling in larger applications which can easily become inefficient in larger apps where state is needed in multiple components across the app . Using Context API in such a case can eliminate prop drilling altogether if so desired, and helps to produce cleaner, more readable, more easily managed code & state/data.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

Actions: Actions are the director in the action/reducer - they dictate when and how the reducers need to update state.

Reducers: If actions are the director, reducers are the actors - they take direction through action types and payloads and use that direction to know when, where, and how to update our state.

Store: Continuing this analogy, I suppose you could say the store is like the studio - It's the piece of the loop that links our state, reducers, and actions to our App, while our App connects to it. The store is our singular source of truth for the rest of our application and ties the whole package together.

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?

Thunk allows us to use our action creators to perform asynchronous actions/functions/operations with our action creators. Because the Redux action -> reducer flow is by nature synchronous, this is vital for allowing our actions to do things like make API calls to receive data and update our state accordingly. It can also change our action reducers in the form of allowing us to combine all of our action creators into one single thunk-function package, which can simplify things.

4. What is your favorite state management system you've learned and this sprint? Please explain why!

My favorite is Redux. Context API is nice because it's lightweight in nature, taking less boilerplate and initial setup, but in my opinion I feel as though the entire Redux system/workflow gives much more functionality for our applications. On the other hand they all have their own uses depending on what needs to be done; Context API for smaller, simpler applications, and Redux for larger, more robust applications.
