# what is a useCallback Hook in React. ?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1677601686827/5e0b183b-9920-4ff3-96ab-623474127323.jpeg align="center")

In React, `useCallback` is a hook that is used to memoize a function. When a function is memoized, it means that the function is only re-created when its dependencies change, and not on every render.

The syntax for `useCallback` is as follows:

```plaintext
javascriptCopy codeconst memoizedCallback = useCallback(
  () => {
    // function logic here
  },
  [/* dependencies */],
);
```

The first argument to `useCallback` is the function you want to memoize. The second argument is an array of dependencies that the memoized function relies on. If any of the dependencies change, the memoized function will be re-created.

Here is an example of how to use `useCallback` in a React component:

```plaintext
javascriptCopy codeimport React, { useCallback, useState } from 'react';

function MyComponent() {
  const [count, setCount] = useState(0);

  const handleClick = useCallback(() => {
    setCount((prevCount) => prevCount + 1);
  }, []);

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={handleClick}>Increment Count</button>
    </div>
  );
}
```

In this example, we define a state variable `count` using the `useState` hook. We also define a memoized function `handleClick` using `useCallback`. The function increments the `count` state variable when the button is clicked.

By using `useCallback`, we ensure that the `handleClick` the function is only re-created when the `count` state variable changes, and not on every render. This can help improve performance in components that rely on expensive functions or are re-rendered frequently.

---

if you like my work then don’t forget to follow back I daily bring a new topic from this huge network and try to make it easy and clear to understand

you can follow me on [Twitter](https://twitter.com/nishar_multani)

if you have any suggestions on any topic to cover you can comment below.