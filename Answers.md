1. Name 3 JavaScript Array/Object Methods that do not produce side-effects? Which method do we use to create a new object while extending the properties of another object?

map, filter, concat! Object.assign is used to create a new object while extending the props of another object.

2. Describe actions, reducers and the store and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

Actions are an object that describes an event that has occurred in the UI. Reducers keep track of state; makes copies, edits those copies, then silently replaces state with those copies. Store is an all-knowing holder of all application knowledge; it is consistant and uneditable regardless who or what is sneaking a peak at it.

3. What is the difference between Application state and Component state? When would be a good time to use one over the other?

Application state is controlled by the store; component state is the state on individual components. Application state is used when multiple components are reading and action on the same data. Component state is used when only one component needs the data.

4. What is middleware? Middleware are functions that modify actions before they reach the reducers.

5.Describe redux-thunk, what does it allow us to do? How does it change our action-creators?

Enables asynchronous actions to occur before they're allowed passage to the synchronous reducers. It gives action creators access to the dispatch and the ability to return functions.

6. Which react-red ux method links up our components with our redux store?

connect 4