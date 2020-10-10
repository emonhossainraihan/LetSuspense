## LetSuspense Component

The LetSuspense is quite simple, it needs to accept a placeholder component, the actual component and a condition. It should render the placeholder as long as the condition is not met and the actual component when the condition is met.

I’ll define a few more properties to enhance the LetSuspense.

## Properties

| Property     |                                                            Description                                                            |
| ------------ | :-------------------------------------------------------------------------------------------------------------------------------: |
| condition    |                                   (bool) [false] Determines when components should be rendered                                    |
| placeholder  |                (React.Component) [undef] A React component that will be rendered as long as the condition is false                |
| children     |                      (JSX) [undef] The actual component(s) that will be rendered when the condition is true                       |
| multiplier   |                                      (Number) [1] The number of placeholders to be rendered                                       |
| initialDelay |                             (Number) [0] Minimum time in milliseconds before a component is rendered                              |
| checkOnce    | (bool) [false] Checks the condition just once, useful for data that doesn’t need to be re-rendered even if the condition changes. |


In summary, this component will help us:

- Improve the user’s visual experience.
- Write less code since our loader logic will be encapsulated and re-used in a declarative manner.