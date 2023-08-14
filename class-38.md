# Reading Questions

## Lifting State Up in React

Lifting state up in React involves moving state from a child component to a parent component. This centralizes data flow, making it consistent and easier to manage. Benefits include data consistency, predictable flow, simplified components, and easier testing.

## Conditional Rendering in React

Conditional rendering in React displays different content based on conditions. For example:

```jsx
function Greeting({ isLoggedIn }) {
  return (
    <div>
      {isLoggedIn ? <h1>Welcome back!</h1> : <h1>Please log in.</h1>}
    </div>
  );
}
```

## Thinking in React Principles

"Thinking in React" involves designing with these principles:

1. **Component Hierarchy:** Organize UI into a component hierarchy with single responsibilities.

2. **Single Responsibility:** Each component should do one thing well and be reusable.

3. **Unidirectional Data Flow:** Data flows from parent to child components via props.

4. **Top-Down Approach:** Start design from top-level components and work down.

5. **Reusable Components:** Design components for reusability across the app.
```
