# Interview Answers
Be prepared to demonstrate your understanding of this week's concepts by answering questions on the following topics. These will not be counted as a part of your sprint score but will be helpful for preparing you for your endorsement interview, and enhancing overall understanding.

1. What problem does the context API help solve?
    Context API is useful for sharing data between components without the use of props each case. Code related to state is much cleaner.

2. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?
    Actions contain a type and payload to dispatch to the reducer. This updates state according to the action payload.
    Reducers return a new, updated state object based on current state and actions dispatched with action creators.
    Store is used within Redux to update state. Store takes in a reducer and updates State accordingly.

3. What does `redux-thunk` allow us to do? How does it change our `action-creators`?
    Redux-thunk is a middleware package useful for asynchronous operations. Action creators forward actions within a reducer, and if that action is a thunk it has access to dispatch to be able to run an async function.

4. What is your favorite state management system you've learned and this sprint? Please explain why!
    Redux is useful to me currently, because it makes state management much easier for me to manage in my head while building app. Passing props confused me a bit previously.