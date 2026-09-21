# ⚛️ React Interview Questions — Practice Edition

A hands-on set of **58 interview questions**, **6 predict-the-output puzzles**, a **rapid-fire round**, and **13 coding exercises** for React developers. Every answer is hidden behind a collapsible block so you can test yourself first, then check.

> All questions are written from scratch to be practiced, not memorized. Explain each answer **out loud** as if you were in an interview.

## How to use this guide

1. Read the question and try to answer it out loud or on paper.
2. Click **💡 Show answer** and compare. Note anything you missed.
3. For coding exercises, build them yourself in a sandbox (Vite, StackBlitz, CodeSandbox) before opening the solution.
4. Come back a few days later and redo the ones you got wrong.

**Difficulty legend:** 🟢 Beginner &nbsp;·&nbsp; 🟡 Intermediate &nbsp;·&nbsp; 🔴 Advanced

## Table of Contents

| No. | Questions |
| --- | --------- |
| | **🧱 Core Concepts** |
| 1 | [What is React and what problem does it solve?](#1-what-is-react-and-what-problem-does-it-solve) |
| 2 | [What is JSX and how is it different from HTML?](#2-what-is-jsx-and-how-is-it-different-from-html) |
| 3 | [What is the Virtual DOM?](#3-what-is-the-virtual-dom) |
| 4 | [What is the difference between a React element and a React component?](#4-what-is-the-difference-between-a-react-element-and-a-react-component) |
| 5 | [Function components vs class components – which should you use?](#5-function-components-vs-class-components--which-should-you-use) |
| 6 | [What are props? Can a child component change them?](#6-what-are-props-can-a-child-component-change-them) |
| 7 | [What is the difference between state and props?](#7-what-is-the-difference-between-state-and-props) |
| 8 | [Why do list items need a `key`, and why is the array index a risky key?](#8-why-do-list-items-need-a-key-and-why-is-the-array-index-a-risky-key) |
| 9 | [What are controlled and uncontrolled components?](#9-what-are-controlled-and-uncontrolled-components) |
| 10 | [What is a Fragment and why would you use it?](#10-what-is-a-fragment-and-why-would-you-use-it) |
| 11 | [What are the common ways to render conditionally, and what is the `&&` pitfall?](#11-what-are-the-common-ways-to-render-conditionally-and-what-is-the--pitfall) |
| 12 | [What does "lifting state up" mean?](#12-what-does-lifting-state-up-mean) |
| 13 | [What is prop drilling and how do you avoid it?](#13-what-is-prop-drilling-and-how-do-you-avoid-it) |
| 14 | [What is the `children` prop and why is it useful?](#14-what-is-the-children-prop-and-why-is-it-useful) |
| | **🪝 Hooks** |
| 15 | [What are the Rules of Hooks and why do they exist?](#15-what-are-the-rules-of-hooks-and-why-do-they-exist) |
| 16 | [How does `useState` work, and why use the functional update form?](#16-how-does-usestate-work-and-why-use-the-functional-update-form) |
| 17 | [How does the dependency array of `useEffect` behave?](#17-how-does-the-dependency-array-of-useeffect-behave) |
| 18 | [How and why do you clean up an effect?](#18-how-and-why-do-you-clean-up-an-effect) |
| 19 | [What is `useRef` used for?](#19-what-is-useref-used-for) |
| 20 | [What is the difference between `useMemo` and `useCallback`?](#20-what-is-the-difference-between-usememo-and-usecallback) |
| 21 | [How does `useContext` work, and what is its main performance caveat?](#21-how-does-usecontext-work-and-what-is-its-main-performance-caveat) |
| 22 | [When would you choose `useReducer` over `useState`?](#22-when-would-you-choose-usereducer-over-usestate) |
| 23 | [What is the difference between `useEffect` and `useLayoutEffect`?](#23-what-is-the-difference-between-useeffect-and-uselayouteffect) |
| 24 | [What is a custom hook? Write one.](#24-what-is-a-custom-hook-write-one) |
| 25 | [What do `useTransition` and `useDeferredValue` do?](#25-what-do-usetransition-and-usedeferredvalue-do) |
| 26 | [Why does my effect run twice in development?](#26-why-does-my-effect-run-twice-in-development) |
| | **⚡ Rendering & Performance** |
| 27 | [What causes a component to re-render?](#27-what-causes-a-component-to-re-render) |
| 28 | [What is reconciliation and how does React's diffing work?](#28-what-is-reconciliation-and-how-does-reacts-diffing-work) |
| 29 | [What does `React.memo` do and when is it not helpful?](#29-what-does-reactmemo-do-and-when-is-it-not-helpful) |
| 30 | [Why do inline objects and functions defeat memoization?](#30-why-do-inline-objects-and-functions-defeat-memoization) |
| 31 | [How do you split code with `React.lazy` and `Suspense`?](#31-how-do-you-split-code-with-reactlazy-and-suspense) |
| 32 | [How would you render a list with 10,000 rows efficiently?](#32-how-would-you-render-a-list-with-10000-rows-efficiently) |
| 33 | [What is automatic batching (React 18)?](#33-what-is-automatic-batching-react-18) |
| 34 | [What is an error boundary and what can it NOT catch?](#34-what-is-an-error-boundary-and-what-can-it-not-catch) |
| | **🗃️ State Management & Data Fetching** |
| 35 | [Context vs Redux vs Zustand – how do you choose?](#35-context-vs-redux-vs-zustand--how-do-you-choose) |
| 36 | [How do you fetch data in an effect without race conditions?](#36-how-do-you-fetch-data-in-an-effect-without-race-conditions) |
| 37 | [What is the difference between server state and client state?](#37-what-is-the-difference-between-server-state-and-client-state) |
| 38 | [Why must state be treated as immutable?](#38-why-must-state-be-treated-as-immutable) |
| 39 | [What is Redux Toolkit and how does it simplify Redux?](#39-what-is-redux-toolkit-and-how-does-it-simplify-redux) |
| 40 | [What is "derived state" and why should you avoid storing it?](#40-what-is-derived-state-and-why-should-you-avoid-storing-it) |
| | **🧭 Events, Forms & Routing** |
| 41 | [What are synthetic events and what is a classic mistake with handlers?](#41-what-are-synthetic-events-and-what-is-a-classic-mistake-with-handlers) |
| 42 | [How would you handle a form with validation?](#42-how-would-you-handle-a-form-with-validation) |
| 43 | [How does client-side routing work (React Router)?](#43-how-does-client-side-routing-work-react-router) |
| 44 | [How do you implement a protected route?](#44-how-do-you-implement-a-protected-route) |
| | **🧩 Advanced Patterns** |
| 45 | [What is a Higher-Order Component (HOC)?](#45-what-is-a-higher-order-component-hoc) |
| 46 | [What is the render props pattern?](#46-what-is-the-render-props-pattern) |
| 47 | [What is the compound component pattern?](#47-what-is-the-compound-component-pattern) |
| 48 | [What are Portals and when do you need them?](#48-what-are-portals-and-when-do-you-need-them) |
| 49 | [How do you pass a `ref` to a child component?](#49-how-do-you-pass-a-ref-to-a-child-component) |
| 50 | [Why does React prefer composition over inheritance?](#50-why-does-react-prefer-composition-over-inheritance) |
| | **🚀 Modern React (18 / 19) & Frameworks** |
| 51 | [What is concurrent rendering?](#51-what-is-concurrent-rendering) |
| 52 | [What is the difference between Server Components and Client Components?](#52-what-is-the-difference-between-server-components-and-client-components) |
| 53 | [What is the difference between CSR, SSR, SSG and hydration?](#53-what-is-the-difference-between-csr-ssr-ssg-and-hydration) |
| 54 | [What are the notable features introduced in React 19?](#54-what-are-the-notable-features-introduced-in-react-19) |
| 55 | [What is the React Compiler?](#55-what-is-the-react-compiler) |
| | **🧪 Testing, Security & Accessibility** |
| 56 | [How do you test React components?](#56-how-do-you-test-react-components) |
| 57 | [How does React protect against XSS, and where can it go wrong?](#57-how-does-react-protect-against-xss-and-where-can-it-go-wrong) |
| 58 | [What are the basics of accessibility (a11y) in React?](#58-what-are-the-basics-of-accessibility-a11y-in-react) |
| | **🎯 Predict the Output** |
| P1 | [Batched updates](#predict-1-batched-updates) |
| P2 | [Stale value in a timeout](#predict-2-stale-value-in-a-timeout) |
| P3 | [The mysterious zero](#predict-3-the-mysterious-zero) |
| P4 | [Effect order](#predict-4-effect-order) |
| P5 | [Mutating state](#predict-5-mutating-state) |
| P6 | [Effect that never stops](#predict-6-effect-that-never-stops) |
| | **⚡ Rapid-Fire Round** |
| | **💻 Coding Exercises** |
| E1 | [Counter with limits](#exercise-1-counter-with-limits) |
| E2 | [Accordion (one panel open at a time)](#exercise-2-accordion-one-panel-open-at-a-time) |
| E3 | [Todo list](#exercise-3-todo-list) |
| E4 | [Fetch and display users](#exercise-4-fetch-and-display-users) |
| E5 | [Debounced search box](#exercise-5-debounced-search-box) |
| E6 | [`useLocalStorage` hook](#exercise-6-uselocalstorage-hook) |
| E7 | [Star rating](#exercise-7-star-rating) |
| E8 | [Countdown timer](#exercise-8-countdown-timer) |
| E9 | [Modal with a portal](#exercise-9-modal-with-a-portal) |
| E10 | [Multi-step form (stepper)](#exercise-10-multi-step-form-stepper) |
| E11 | [🐞 Fix the bug: the counter that gets stuck](#exercise-11--fix-the-bug-the-counter-that-gets-stuck) |
| E12 | [🐞 Fix the bug: the list that shows the wrong row](#exercise-12--fix-the-bug-the-list-that-shows-the-wrong-row) |
| E13 | [Build a `useFetch` hook](#exercise-13-build-a-usefetch-hook) |

---

## 🧱 Core Concepts

### 1. What is React and what problem does it solve?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

React is a JavaScript library for building user interfaces out of small, reusable **components**. It solves the problem of keeping the UI in sync with changing data: you *declare* what the UI should look like for a given state, and React works out how to update the DOM.

Key ideas:
- **Component-based** – UI is a tree of self-contained pieces.
- **Declarative** – describe the result, not the DOM steps.
- **One-way data flow** – data moves from parent to child through props.
- **Library, not framework** – routing, data fetching and build tooling come from the ecosystem (React Router, TanStack Query, Vite, Next.js, ...).

</details>

**[⬆ Back to Top](#table-of-contents)**

### 2. What is JSX and how is it different from HTML?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

JSX is a syntax extension that lets you write markup inside JavaScript. A compiler (Babel, SWC, esbuild) turns it into function calls that create React elements.

```jsx
const el = <h1 className="title">Hello, {user.name}</h1>;
// compiles to roughly:
const el = jsx('h1', { className: 'title', children: ['Hello, ', user.name] });
```

Differences from HTML:
| HTML | JSX |
| ---- | --- |
| `class` | `className` |
| `for` | `htmlFor` |
| `onclick="..."` | `onClick={fn}` |
| `style="color: red"` | `style={{ color: 'red' }}` |
| Tags may be unclosed (`<br>`) | Every tag must be closed (`<br />`) |
| Multiple root nodes allowed | One root – wrap in `<>...</>` |

Anything inside `{}` is a JavaScript **expression** (not a statement like `if` or `for`).

</details>

**[⬆ Back to Top](#table-of-contents)**

### 3. What is the Virtual DOM?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

The Virtual DOM is a lightweight JavaScript representation of the UI. When state changes:

1. React renders the component again and produces a **new** virtual tree.
2. It **diffs** the new tree against the previous one (reconciliation).
3. It applies only the **minimal set of changes** to the real DOM.

The benefit is not that it is magically faster than hand-written DOM code, it is that you get a simple declarative programming model with good-enough performance by default.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 4. What is the difference between a React element and a React component?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

- An **element** is a plain object describing what you want on screen: `{ type: 'button', props: { children: 'Save' } }`. It is immutable and cheap.
- A **component** is a function (or class) that accepts props and **returns elements**.

```jsx
function Greeting({ name }) {      // component
  return <p>Hello {name}</p>;      // returns an element
}
const element = <Greeting name="Ada" />; // an element whose type is a component
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 5. Function components vs class components – which should you use?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

Use **function components with hooks** for all new code. Class components still work and you will meet them in legacy code bases. The one thing that still requires a class is writing your own **error boundary**.

| Class | Function + hooks |
| ----- | ---------------- |
| `this.state` / `setState` | `useState`, `useReducer` |
| `componentDidMount` | `useEffect(fn, [])` |
| `componentDidUpdate` | `useEffect(fn, [deps])` |
| `componentWillUnmount` | cleanup function returned from `useEffect` |
| `static contextType` | `useContext` |

</details>

**[⬆ Back to Top](#table-of-contents)**

### 6. What are props? Can a child component change them?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

Props are the inputs a parent passes to a child. They are **read-only**: a component must never modify its own props. If a child needs to request a change, the parent passes down a **callback**.

```jsx
function Parent() {
  const [name, setName] = useState('Ada');
  return <Child name={name} onRename={setName} />;
}

function Child({ name, onRename }) {
  return <button onClick={() => onRename('Grace')}>{name}</button>;
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 7. What is the difference between state and props?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

| | Props | State |
| --- | ----- | ----- |
| Owned by | The parent | The component itself |
| Mutable by the component? | No | Yes, through the setter |
| Purpose | Configure a component | Remember data that changes over time |
| Change causes | Re-render (when the parent re-renders with new values) | Re-render |

A good rule: if a value can be calculated from props or other state, do **not** store it in state.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 8. Why do list items need a `key`, and why is the array index a risky key?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

`key` tells React which item is which between renders, so it can reuse, move or remove the correct DOM nodes and component state.

Using the **index** breaks when the list is reordered, filtered, or has items inserted at the top: React thinks "item 0" is still the same item, so local state (like an input's text) sticks to the wrong row.

```jsx
// ✅ stable, unique id from your data
{todos.map(todo => <TodoItem key={todo.id} todo={todo} />)}

// ⚠️ only OK for static lists that never reorder
{items.map((item, i) => <li key={i}>{item}</li>)}
```

`key` is not passed to the component as a prop. Never use `Math.random()` as a key – it forces a remount on every render.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 9. What are controlled and uncontrolled components?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

- **Controlled** – React state is the single source of truth for the input value.
- **Uncontrolled** – the DOM keeps the value; you read it when needed through a `ref` or `FormData`.

```jsx
// Controlled
const [email, setEmail] = useState('');
<input value={email} onChange={e => setEmail(e.target.value)} />

// Uncontrolled
const ref = useRef(null);
<input defaultValue="" ref={ref} />
// later: ref.current.value
```

Controlled inputs make live validation and formatting easy. Uncontrolled inputs are simpler and re-render less (this is the approach React Hook Form uses).

</details>

**[⬆ Back to Top](#table-of-contents)**

### 10. What is a Fragment and why would you use it?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

A Fragment lets a component return several siblings without adding an extra DOM node.

```jsx
return (
  <>
    <h1>Title</h1>
    <p>Body</p>
  </>
);
```

The short syntax `<>` cannot take a `key`. When you need one (for example, when mapping), use `<Fragment key={id}>`.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 11. What are the common ways to render conditionally, and what is the `&&` pitfall?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

```jsx
if (loading) return <Spinner />;                 // early return

{isAdmin ? <AdminPanel /> : <UserPanel />}       // ternary

{hasError && <ErrorMessage />}                   // logical AND
```

**Pitfall:** `0` and `NaN` are rendered by React, so `{items.length && <List />}` prints `0` when the list is empty. Use `{items.length > 0 && <List />}` or a ternary instead.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 12. What does "lifting state up" mean?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

When two sibling components need the same data, move the state to their **closest common parent** and pass the value and the setter down as props.

```jsx
function Converter() {
  const [celsius, setCelsius] = useState(0);
  return (
    <>
      <CelsiusInput value={celsius} onChange={setCelsius} />
      <FahrenheitView value={celsius * 9 / 5 + 32} />
    </>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 13. What is prop drilling and how do you avoid it?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

Prop drilling is passing props through many intermediate components that do not use them, just to reach a deeply nested child.

Ways to avoid it, from simplest to heaviest:
1. **Composition** – pass ready-made elements as `children` or props so the middle layers do not need to know about the data.
2. **Context** – for values many components read (theme, current user, locale).
3. **A state library** – Redux Toolkit, Zustand, Jotai, when state is large or updates often.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 14. What is the `children` prop and why is it useful?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

`children` is whatever you put between a component's opening and closing tags. It enables **composition**: the parent decides the content, the component decides the layout.

```jsx
function Card({ title, children }) {
  return (
    <section className="card">
      <h2>{title}</h2>
      {children}
    </section>
  );
}

<Card title="Profile"><Avatar /><Bio /></Card>
```

</details>

**[⬆ Back to Top](#table-of-contents)**

## 🪝 Hooks

### 15. What are the Rules of Hooks and why do they exist?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

1. Call hooks only at the **top level** – never inside loops, conditions, or nested functions.
2. Call hooks only from **function components** or **custom hooks**.

React tracks hooks by the **order** in which they are called on each render. Changing that order between renders would attach state to the wrong hook. The `eslint-plugin-react-hooks` package enforces both rules.

```jsx
// ❌ conditional hook
if (isLoggedIn) { const [name, setName] = useState(''); }

// ✅ hook always runs, logic is conditional
const [name, setName] = useState('');
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 16. How does `useState` work, and why use the functional update form?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

`useState(initial)` returns `[value, setValue]`. State is a **snapshot**: inside one render, `value` never changes. Calling the setter schedules a new render.

If the next state depends on the previous one, pass a function so you always get the latest value:

```jsx
setCount(count + 1); setCount(count + 1);   // ends up +1 (both use the same snapshot)
setCount(c => c + 1); setCount(c => c + 1); // ends up +2
```

For expensive initial values use **lazy initialization**: `useState(() => computeExpensive())` – the function runs only on the first render.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 17. How does the dependency array of `useEffect` behave?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

| Dependency array | When the effect runs |
| ---------------- | -------------------- |
| omitted | After **every** render |
| `[]` | After the first render only (on mount) |
| `[a, b]` | After the first render and whenever `a` or `b` changed (compared with `Object.is`) |

Effects run **after** the browser has painted. Every reactive value used inside the effect (props, state, functions defined in the component) must be listed as a dependency – the lint rule `react-hooks/exhaustive-deps` helps you get this right.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 18. How and why do you clean up an effect?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

Return a function from the effect. React runs it **before the effect runs again** and when the component **unmounts**. Use it to remove listeners, clear timers, close connections and cancel requests.

```jsx
useEffect(() => {
  const onResize = () => setWidth(window.innerWidth);
  window.addEventListener('resize', onResize);
  return () => window.removeEventListener('resize', onResize);
}, []);
```

Without cleanup you get memory leaks, duplicate listeners, and state updates from stale requests.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 19. What is `useRef` used for?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

`useRef` returns a mutable object `{ current }` that **persists across renders** and does **not** trigger a re-render when changed.

Common uses:
- Access a DOM node (focus, scroll, measure).
- Store values that should not cause renders (timer ids, previous value, "is mounted" flags).

```jsx
function SearchBox() {
  const inputRef = useRef(null);
  return (
    <>
      <input ref={inputRef} />
      <button onClick={() => inputRef.current.focus()}>Focus</button>
    </>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 20. What is the difference between `useMemo` and `useCallback`?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

- `useMemo(() => compute(a, b), [a, b])` caches a **value**.
- `useCallback(fn, [deps])` caches a **function** (it is shorthand for `useMemo(() => fn, [deps])`).

Use them when:
- a calculation is genuinely expensive, or
- you pass an object/function to a `React.memo` child or to another hook's dependency array and need a stable reference.

They are **performance hints**, not guarantees, and they have a cost. Measure first – do not wrap everything.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 21. How does `useContext` work, and what is its main performance caveat?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

```jsx
const ThemeContext = createContext('light');

function App() {
  const [theme, setTheme] = useState('dark');
  const value = useMemo(() => ({ theme, setTheme }), [theme]);
  return (
    <ThemeContext.Provider value={value}>
      <Page />
    </ThemeContext.Provider>
  );
}

function Button() {
  const { theme } = useContext(ThemeContext);
  return <button className={theme}>Click</button>;
}
```

**Caveat:** every component that reads the context re-renders whenever the provider `value` changes (by reference). Memoize the value and split unrelated data into separate contexts.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 22. When would you choose `useReducer` over `useState`?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

Choose `useReducer` when state has several related fields, when the next state depends on complex rules, or when you want all transitions in one testable pure function.

```jsx
function reducer(state, action) {
  switch (action.type) {
    case 'add':    return { ...state, items: [...state.items, action.item] };
    case 'remove': return { ...state, items: state.items.filter(i => i.id !== action.id) };
    default:       return state;
  }
}

const [state, dispatch] = useReducer(reducer, { items: [] });
dispatch({ type: 'add', item: { id: 1, name: 'Book' } });
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 23. What is the difference between `useEffect` and `useLayoutEffect`?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

- `useEffect` runs **after** the browser paints – it does not block the screen.
- `useLayoutEffect` runs **synchronously after DOM updates but before paint**.

Use `useLayoutEffect` only when you must read layout (for example, measure an element) and change the DOM before the user sees the first frame, to avoid flicker. Because it blocks painting, prefer `useEffect` in every other case.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 24. What is a custom hook? Write one.

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

A custom hook is a function whose name starts with `use` and that calls other hooks to share **stateful logic** between components. Each component that calls it gets its **own** isolated state.

```jsx
function useDebounce(value, delay = 300) {
  const [debounced, setDebounced] = useState(value);

  useEffect(() => {
    const id = setTimeout(() => setDebounced(value), delay);
    return () => clearTimeout(id);
  }, [value, delay]);

  return debounced;
}

const debouncedQuery = useDebounce(query, 500);
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 25. What do `useTransition` and `useDeferredValue` do?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

Both let you mark some updates as **non-urgent** so typing and clicking stay responsive.

```jsx
const [isPending, startTransition] = useTransition();

function onChange(e) {
  setText(e.target.value);                       // urgent: update the input now
  startTransition(() => setFilter(e.target.value)); // non-urgent: heavy list can wait
}
```

- `useTransition` – wraps a **state update** you control.
- `useDeferredValue(value)` – gives you a **lagging copy of a value**, useful when the value comes from props and you cannot wrap the setter.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 26. Why does my effect run twice in development?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

In development, `<StrictMode>` deliberately **mounts, unmounts, and re-mounts** each component once to reveal effects that are missing cleanup. This does not happen in production.

If the double run causes a bug (duplicate requests, duplicate subscriptions), the fix is to write a proper cleanup function – not to remove StrictMode or add a "ran once" ref.

</details>

**[⬆ Back to Top](#table-of-contents)**


## ⚡ Rendering & Performance

### 27. What causes a component to re-render?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

A component re-renders when:
1. Its own **state** changes.
2. Its **parent re-renders** (even if the props are identical, unless wrapped in `React.memo`).
3. A **context** it consumes changes.

Changing a *prop* by itself does not trigger anything – the parent must render again to pass a new prop. Also note that a **render is not a DOM update**: React re-runs your function, diffs the result, and touches the DOM only where something actually changed.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 28. What is reconciliation and how does React's diffing work?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

Reconciliation is how React compares the previous and next element trees. It uses two heuristics to stay fast:

1. Elements of a **different type** (`<div>` → `<span>`, `<A>` → `<B>`) produce a completely new subtree – the old one is unmounted and its state is lost.
2. In lists, **`key`** identifies which child is which across renders.

If the type and position are the same, React keeps the instance, updates the changed props, and recurses into the children.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 29. What does `React.memo` do and when is it not helpful?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

`React.memo(Component)` skips re-rendering when the props are **shallowly equal** to the previous props.

```jsx
const Row = React.memo(function Row({ item, onSelect }) {
  return <li onClick={() => onSelect(item.id)}>{item.name}</li>;
});
```

It does not help when a prop gets a **new reference on every render** (inline object, array, or function), when the component is cheap, or when it consumes a context that changes. Pair it with `useCallback`/`useMemo` for the props you pass down.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 30. Why do inline objects and functions defeat memoization?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

Every render creates new objects and functions, and `{} !== {}`. So a memoized child sees "new" props each time.

```jsx
// ❌ new object + new function every render → Row always re-renders
<Row style={{ color: 'red' }} onSelect={() => select(id)} />

// ✅ stable references
const style = useMemo(() => ({ color: 'red' }), []);
const handleSelect = useCallback(() => select(id), [id]);
<Row style={style} onSelect={handleSelect} />
```

Moving constants **outside** the component also gives a stable reference for free.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 31. How do you split code with `React.lazy` and `Suspense`?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

```jsx
import { lazy, Suspense } from 'react';

const Dashboard = lazy(() => import('./Dashboard'));

function App() {
  return (
    <Suspense fallback={<Spinner />}>
      <Dashboard />
    </Suspense>
  );
}
```

The bundler puts `Dashboard` in a separate chunk that is downloaded the first time it renders. The most common split points are **routes** and **heavy, rarely-used components** (charts, editors, modals).

</details>

**[⬆ Back to Top](#table-of-contents)**

### 32. How would you render a list with 10,000 rows efficiently?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

Use **virtualization (windowing)**: render only the rows visible in the viewport plus a small buffer. Libraries: `react-window`, `@tanstack/react-virtual`.

Other helpers: paginate or infinite-scroll from the server, memoize row components, keep row props stable, and avoid layout thrashing with fixed or estimated row heights.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 33. What is automatic batching (React 18)?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

React groups multiple state updates into **one re-render**. Before React 18 this only worked inside React event handlers; now it works everywhere – timeouts, promises, native event handlers.

```jsx
setTimeout(() => {
  setCount(c => c + 1);
  setFlag(f => !f);
  // React 18: ONE render. React 17: TWO renders.
}, 1000);
```

Use `flushSync` from `react-dom` in the rare case you need the DOM updated immediately.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 34. What is an error boundary and what can it NOT catch?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

An error boundary is a **class component** that catches errors thrown while rendering its children and shows a fallback UI instead of crashing the whole app.

```jsx
class ErrorBoundary extends React.Component {
  state = { hasError: false };
  static getDerivedStateFromError() { return { hasError: true }; }
  componentDidCatch(error, info) { logError(error, info); }
  render() {
    return this.state.hasError ? <p>Something went wrong.</p> : this.props.children;
  }
}
```

It does **not** catch errors in: event handlers, asynchronous code (`setTimeout`, promises), server-side rendering, or the boundary itself. The `react-error-boundary` package gives you a ready-made function-friendly wrapper.

</details>

**[⬆ Back to Top](#table-of-contents)**

## 🗃️ State Management & Data Fetching

### 35. Context vs Redux vs Zustand – how do you choose?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

| Need | Good fit |
| ---- | -------- |
| Rarely-changing global values (theme, locale, auth user) | **Context** |
| Small/medium shared client state with minimal boilerplate | **Zustand / Jotai** |
| Large app, strict conventions, time-travel debugging, many developers | **Redux Toolkit** |
| Data that comes from a server | **TanStack Query / RTK Query / SWR** (not a global store) |

Start with local state, lift it up when needed, and only add a library when the pain is real.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 36. How do you fetch data in an effect without race conditions?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

If `userId` changes quickly, an older request can finish **after** a newer one and overwrite the correct data. Ignore or cancel stale requests in the cleanup:

```jsx
useEffect(() => {
  const controller = new AbortController();

  async function load() {
    try {
      const res = await fetch(`/api/users/${userId}`, { signal: controller.signal });
      setUser(await res.json());
    } catch (err) {
      if (err.name !== 'AbortError') setError(err);
    }
  }
  load();

  return () => controller.abort();
}, [userId]);
```

In real apps a data library (TanStack Query, SWR) handles this, plus caching, retries and de-duplication.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 37. What is the difference between server state and client state?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

- **Client state** lives only in the browser: modal open, selected tab, form draft.
- **Server state** is a *copy* of remote data that can become stale, is shared, and needs loading/error handling.

Server state needs caching, background refetching, invalidation after mutations, and request de-duplication – exactly what TanStack Query or RTK Query provide. Putting it in `useState` or Redux means re-implementing all of that by hand.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 38. Why must state be treated as immutable?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

React (and `memo`, `useMemo`, dependency arrays) decides whether something changed by comparing **references**. If you mutate an object or array in place, the reference stays the same, so React may skip the update.

```jsx
// ❌ mutation – UI may not update
todos.push(newTodo);
setTodos(todos);

// ✅ new array
setTodos([...todos, newTodo]);

// ✅ update one item immutably
setTodos(todos.map(t => t.id === id ? { ...t, done: true } : t));
```

Libraries like **Immer** (built into Redux Toolkit) let you write "mutating" code that produces immutable updates.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 39. What is Redux Toolkit and how does it simplify Redux?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

Redux Toolkit (RTK) is the official, opinionated way to write Redux. It removes most of the boilerplate:

- `configureStore` – sets up the store with good defaults and DevTools.
- `createSlice` – generates action creators and the reducer together; uses Immer so you can write `state.value += 1`.
- `createAsyncThunk` – standard pattern for async actions.
- **RTK Query** – built-in data fetching and caching.

```js
const counterSlice = createSlice({
  name: 'counter',
  initialState: { value: 0 },
  reducers: {
    increment: state => { state.value += 1; },
    addBy: (state, action) => { state.value += action.payload; },
  },
});
export const { increment, addBy } = counterSlice.actions;
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 40. What is "derived state" and why should you avoid storing it?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

Derived state is a value you can compute from existing props or state. Storing it separately creates two sources of truth that can go out of sync.

```jsx
// ❌ duplicated state must be kept in sync manually
const [todos, setTodos] = useState([]);
const [doneCount, setDoneCount] = useState(0);

// ✅ compute during render (wrap in useMemo only if it is expensive)
const doneCount = todos.filter(t => t.done).length;
```

</details>

**[⬆ Back to Top](#table-of-contents)**

## 🧭 Events, Forms & Routing

### 41. What are synthetic events and what is a classic mistake with handlers?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

React wraps native browser events in a cross-browser object called `SyntheticEvent` (same API: `preventDefault()`, `stopPropagation()`, `target`, ...). Handlers are attached through event delegation at the root.

**Classic mistake:** calling the function instead of passing it.

```jsx
<button onClick={handleClick()}>Save</button>      // ❌ runs during render
<button onClick={handleClick}>Save</button>         // ✅ pass the function
<button onClick={() => handleClick(id)}>Save</button> // ✅ when you need arguments
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 42. How would you handle a form with validation?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

**Small forms** – controlled inputs plus an `errors` object, validated on submit (and optionally on blur).

```jsx
function handleSubmit(e) {
  e.preventDefault();
  const errs = {};
  if (!email.includes('@')) errs.email = 'Enter a valid email';
  if (password.length < 8) errs.password = 'At least 8 characters';
  setErrors(errs);
  if (Object.keys(errs).length === 0) submit({ email, password });
}
```

**Larger forms** – use **React Hook Form** (uncontrolled inputs, fewer re-renders) with a schema validator such as **Zod**. Always validate again on the server.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 43. How does client-side routing work (React Router)?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

The router uses the browser **History API** to change the URL without a page reload, then renders the component that matches the new path. `<Link>` and `useNavigate` update history instead of making a network request.

```jsx
<BrowserRouter>
  <Routes>
    <Route path="/" element={<Home />} />
    <Route path="/users/:id" element={<UserPage />} />   {/* useParams() → { id } */}
    <Route path="*" element={<NotFound />} />
  </Routes>
</BrowserRouter>
```

Because the server only ever serves `index.html`, it must be configured to return that file for unknown paths (SPA fallback).

</details>

**[⬆ Back to Top](#table-of-contents)**

### 44. How do you implement a protected route?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

Wrap the private routes in a component that checks authentication and redirects otherwise.

```jsx
import { Navigate, Outlet, useLocation } from 'react-router-dom';

function ProtectedRoute() {
  const { user } = useAuth();
  const location = useLocation();
  return user
    ? <Outlet />
    : <Navigate to="/login" replace state={{ from: location }} />;
}

<Route element={<ProtectedRoute />}>
  <Route path="/dashboard" element={<Dashboard />} />
</Route>
```

Remember: client-side checks only improve UX. The **API must enforce authorization**.

</details>

**[⬆ Back to Top](#table-of-contents)**

## 🧩 Advanced Patterns

### 45. What is a Higher-Order Component (HOC)?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

A HOC is a function that takes a component and returns a new component with extra behavior.

```jsx
function withLoading(Component) {
  return function Wrapped({ isLoading, ...props }) {
    return isLoading ? <Spinner /> : <Component {...props} />;
  };
}

const UserListWithLoading = withLoading(UserList);
```

HOCs were the main reuse tool before hooks. Today, **custom hooks** are usually simpler, but HOCs are still common in older code and libraries (`connect`, `withRouter`).

</details>

**[⬆ Back to Top](#table-of-contents)**

### 46. What is the render props pattern?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

A component receives a **function** as a prop (or as `children`) and calls it to decide what to render, sharing its internal state with the caller.

```jsx
function MouseTracker({ children }) {
  const [pos, setPos] = useState({ x: 0, y: 0 });
  return (
    <div onMouseMove={e => setPos({ x: e.clientX, y: e.clientY })}>
      {children(pos)}
    </div>
  );
}

<MouseTracker>{({ x, y }) => <p>{x}, {y}</p>}</MouseTracker>
```

Custom hooks have replaced most uses, but render props remain useful for flexible UI libraries.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 47. What is the compound component pattern?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

Several components work together and share implicit state (usually via context), giving consumers a flexible, readable API – like `<select>` and `<option>`.

```jsx
const TabsContext = createContext();

function Tabs({ children, defaultValue }) {
  const [active, setActive] = useState(defaultValue);
  return <TabsContext.Provider value={{ active, setActive }}>{children}</TabsContext.Provider>;
}
function Tab({ value, children }) {
  const { active, setActive } = useContext(TabsContext);
  return <button aria-selected={active === value} onClick={() => setActive(value)}>{children}</button>;
}
function Panel({ value, children }) {
  return useContext(TabsContext).active === value ? <div>{children}</div> : null;
}

<Tabs defaultValue="a">
  <Tab value="a">A</Tab><Tab value="b">B</Tab>
  <Panel value="a">Content A</Panel><Panel value="b">Content B</Panel>
</Tabs>
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### 48. What are Portals and when do you need them?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

`createPortal(children, domNode)` renders children into a **different DOM node** (usually `document.body`) while keeping them in the same React tree, so context and event bubbling still work.

```jsx
import { createPortal } from 'react-dom';

function Modal({ children }) {
  return createPortal(<div className="overlay">{children}</div>, document.body);
}
```

Typical uses: modals, tooltips, dropdowns – anything that must escape a parent's `overflow: hidden` or `z-index` stacking context.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 49. How do you pass a `ref` to a child component?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

Before React 19, function components could not receive `ref` as a normal prop, so you wrapped them in `forwardRef`:

```jsx
const FancyInput = forwardRef(function FancyInput(props, ref) {
  return <input ref={ref} {...props} />;
});
```

In **React 19**, `ref` is a regular prop for function components:

```jsx
function FancyInput({ ref, ...props }) {
  return <input ref={ref} {...props} />;
}
```

`forwardRef` still works in existing code. Use `useImperativeHandle` if you want to expose only a limited API (e.g. `focus()`) instead of the raw DOM node.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 50. Why does React prefer composition over inheritance?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

Components customize behavior by **containing** other components and accepting props/children – not by extending base classes. Composition is more flexible (you can mix and match), avoids deep hierarchies, and keeps data flow explicit.

```jsx
// Instead of DangerButton extends Button ...
function DangerButton(props) {
  return <Button {...props} variant="danger" />;
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

## 🚀 Modern React (18 / 19) & Frameworks

### 51. What is concurrent rendering?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

Concurrent rendering lets React **prepare an update in the background and pause or abandon it** if something more urgent (like a keystroke) arrives. Rendering becomes interruptible instead of one long blocking task.

Features built on it: `useTransition`, `useDeferredValue`, streaming SSR, and `Suspense` for data. You opt in simply by using `createRoot` (React 18+).

</details>

**[⬆ Back to Top](#table-of-contents)**

### 52. What is the difference between Server Components and Client Components?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

| | Server Component | Client Component |
| --- | --- | --- |
| Runs on | Server (build or request time) | Browser (and is pre-rendered on the server) |
| Can use | `async/await`, DB access, secrets | `useState`, `useEffect`, event handlers, browser APIs |
| JS sent to client | None for the component itself | Yes |
| How to declare | Default in frameworks like Next.js App Router | Add `'use client'` at the top of the file |

Rule of thumb: keep components on the server by default, and push `'use client'` down to the small interactive leaves.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 53. What is the difference between CSR, SSR, SSG and hydration?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

- **CSR** – the browser downloads JS and renders everything on the client.
- **SSR** – the server renders HTML on each request; faster first paint and better SEO.
- **SSG** – HTML is generated once at build time and served from a CDN.
- **Hydration** – React attaches event handlers and state to server-rendered HTML in the browser.

A **hydration mismatch** happens when the server HTML differs from the first client render (e.g. using `Date.now()`, `Math.random()` or `window` during render). Move such logic into `useEffect`.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 54. What are the notable features introduced in React 19?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

- **Actions** – async functions used for transitions, e.g. `<form action={fn}>`, with pending state handled for you.
- **`useActionState`** – manage the state and pending status of a form action.
- **`useOptimistic`** – show an optimistic UI while a request is in flight.
- **`use`** – read a promise or context during render (can be called conditionally).
- **`ref` as a prop** – no more `forwardRef` needed for function components.
- Built-in support for rendering `<title>`, `<meta>` and `<link>` tags from components.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 55. What is the React Compiler?

🔴 Advanced

<details>
<summary>💡 Show answer</summary>

The React Compiler is a build-time tool that **automatically memoizes** components and values, so you rarely need to write `useMemo`, `useCallback` or `React.memo` by hand. It relies on your code following the Rules of React (pure render functions, no mutating props/state), and it comes with an ESLint rule that reports violations.

</details>

**[⬆ Back to Top](#table-of-contents)**

## 🧪 Testing, Security & Accessibility

### 56. How do you test React components?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

Use **React Testing Library** with a runner like Vitest or Jest. Test what the **user sees and does**, not implementation details such as internal state.

```jsx
import { render, screen } from '@testing-library/react';
import userEvent from '@testing-library/user-event';

test('increments the counter', async () => {
  render(<Counter />);
  await userEvent.click(screen.getByRole('button', { name: /increment/i }));
  expect(screen.getByText('Count: 1')).toBeInTheDocument();
});
```

Prefer queries in this order: `getByRole` → `getByLabelText` → `getByText` → `getByTestId` (last resort). Use Playwright or Cypress for end-to-end flows.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 57. How does React protect against XSS, and where can it go wrong?

🟡 Intermediate

<details>
<summary>💡 Show answer</summary>

JSX **escapes** values before rendering, so `{userInput}` is treated as text, not HTML.

Risky spots:
- `dangerouslySetInnerHTML` – only use with content sanitized by a library such as **DOMPurify**.
- User-controlled URLs in `href`/`src` (`javascript:` URLs) – validate the protocol.
- Storing tokens in `localStorage` – prefer `HttpOnly` cookies.

</details>

**[⬆ Back to Top](#table-of-contents)**

### 58. What are the basics of accessibility (a11y) in React?

🟢 Beginner

<details>
<summary>💡 Show answer</summary>

- Use **semantic HTML** (`button`, `nav`, `main`, `label`) before reaching for `div` + ARIA.
- Every input needs a label (`<label htmlFor>` or `aria-label`).
- Everything clickable must be **keyboard accessible** and show a visible focus style.
- Manage focus in modals and route changes; announce dynamic updates with `aria-live`.
- Provide `alt` text for images.
- Lint with `eslint-plugin-jsx-a11y` and test with a screen reader.

</details>

**[⬆ Back to Top](#table-of-contents)**


## 🎯 Predict the Output

Read each snippet, decide what happens **before** opening the answer.

### Predict 1: Batched updates

<details>
<summary>👀 Show snippet</summary>

```jsx
function App() {
  const [count, setCount] = useState(0);
  const handleClick = () => {
    setCount(count + 1);
    setCount(count + 1);
    setCount(count + 1);
  };
  return <button onClick={handleClick}>{count}</button>;
}
```

**What does the button show after ONE click?**

</details>

<details>
<summary>💡 Show answer</summary>

**`1`.** All three calls use the same `count` snapshot (`0`), so each one says "set to 1". Use `setCount(c => c + 1)` to get `3`.

</details>

**[⬆ Back to Top](#table-of-contents)**

### Predict 2: Stale value in a timeout

<details>
<summary>👀 Show snippet</summary>

```jsx
function handleClick() {
  setCount(count + 1);
  console.log(count);
  setTimeout(() => console.log(count), 1000);
}
// count is 0 when the button is clicked
```

**What is logged, and what does the UI show?**

</details>

<details>
<summary>💡 Show answer</summary>

Logs `0`, then `0` again after one second. The UI shows `1`. State is a snapshot – the handler and the timeout callback both close over the `count` of the render in which they were created.

</details>

**[⬆ Back to Top](#table-of-contents)**

### Predict 3: The mysterious zero

<details>
<summary>👀 Show snippet</summary>

```jsx
const items = [];
return <div>{items.length && <List items={items} />}</div>;
```

**What is rendered?**

</details>

<details>
<summary>💡 Show answer</summary>

A literal **`0`**. `0 && x` evaluates to `0`, and React renders numbers. Use `items.length > 0 && ...`.

</details>

**[⬆ Back to Top](#table-of-contents)**

### Predict 4: Effect order

<details>
<summary>👀 Show snippet</summary>

```jsx
function Child() {
  console.log('child render');
  useEffect(() => console.log('child effect'), []);
  return null;
}
function Parent() {
  console.log('parent render');
  useEffect(() => console.log('parent effect'), []);
  return <Child />;
}
```

**What is the console order on first mount (no StrictMode)?**

</details>

<details>
<summary>💡 Show answer</summary>

```
parent render
child render
child effect
parent effect
```

Rendering goes top-down; effects run **bottom-up** (children first).

</details>

**[⬆ Back to Top](#table-of-contents)**

### Predict 5: Mutating state

<details>
<summary>👀 Show snippet</summary>

```jsx
const [user, setUser] = useState({ name: 'Ada' });
<button onClick={() => { user.name = 'Grace'; setUser(user); }}>
  {user.name}
</button>
```

**Does the button text change after a click?**

</details>

<details>
<summary>💡 Show answer</summary>

**No.** The object was mutated but the reference is the same, so React sees no change and bails out. Use `setUser({ ...user, name: 'Grace' })`.

</details>

**[⬆ Back to Top](#table-of-contents)**

### Predict 6: Effect that never stops

<details>
<summary>👀 Show snippet</summary>

```jsx
function Profile() {
  const options = { verbose: true };
  useEffect(() => {
    fetchData(options);
  }, [options]);
  // ...
}
```

**How often does the effect run?**

</details>

<details>
<summary>💡 Show answer</summary>

After **every render**. `options` is a new object each time, so `Object.is` says it changed. Move it outside the component, wrap it in `useMemo`, or depend on the primitive values you actually use.

</details>

**[⬆ Back to Top](#table-of-contents)**

## ⚡ Rapid-Fire Round

Answer each one in **10 seconds or less**.

1. Which hook replaces `componentDidMount`?
2. Can you call a hook inside a loop?
3. Is `setState` synchronous?
4. Does changing `ref.current` re-render the component?
5. How can you force a component to remount?
6. What does `useId` give you?
7. What is the difference between `useMemo` and `React.memo`?
8. Can you pass an `async` function directly to `useEffect`?
9. What renders for `null`, `undefined`, `true` and `false` in JSX?
10. Which hook would you use to remember the previous value of a prop?
11. What is the value of `useContext(Ctx)` when there is no Provider above?
12. What does `flushSync` do?
13. Which lifecycle needs a class component today?
14. What is `dangerouslySetInnerHTML` and why the scary name?
15. What does `<StrictMode>` do in production?

<details>
<summary>💡 Show answers</summary>

1. `useEffect(fn, [])`
2. No – hooks must run in the same order on every render.
3. No – updates are batched and the new value appears on the next render.
4. No.
5. Change its `key`.
6. A stable, unique id (SSR-safe) – handy for linking `label`/`input` and ARIA attributes.
7. `useMemo` caches a **value**; `React.memo` skips re-rendering a **component** when props are equal.
8. No – define an async function **inside** the effect and call it (the effect must return nothing or a cleanup function).
9. Nothing.
10. `useRef` (update it in an effect).
11. The default value passed to `createContext(default)`.
12. Forces React to apply the state update to the DOM synchronously.
13. Error boundaries.
14. It injects raw HTML into an element; the name warns you about XSS if the HTML is not sanitized.
15. Nothing – it only adds extra checks in development.

</details>

**[⬆ Back to Top](#table-of-contents)**

## 💻 Coding Exercises

Try each exercise **yourself first** (a Vite + React sandbox or StackBlitz works well). Then compare with the sample solution. There are many valid solutions – what matters is that yours meets the requirements.

### Exercise 1: Counter with limits

🟢 Beginner

**Requirements:** show a number; `+` and `-` buttons; the value must stay between `min` and `max` (disable buttons at the limits); a Reset button.

<details>
<summary>💡 Show solution</summary>

```jsx
function Counter({ min = 0, max = 10 }) {
  const [count, setCount] = useState(min);
  return (
    <div>
      <button onClick={() => setCount(c => c - 1)} disabled={count <= min}>-</button>
      <span>{count}</span>
      <button onClick={() => setCount(c => c + 1)} disabled={count >= max}>+</button>
      <button onClick={() => setCount(min)}>Reset</button>
    </div>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 2: Accordion (one panel open at a time)

🟢 Beginner

**Requirements:** render a list of `{ id, title, content }`; clicking a title opens its panel and closes the others; clicking the open one closes it. Add `aria-expanded`.

<details>
<summary>💡 Show solution</summary>

```jsx
function Accordion({ items }) {
  const [openId, setOpenId] = useState(null);
  return (
    <div>
      {items.map(({ id, title, content }) => {
        const isOpen = openId === id;
        return (
          <div key={id}>
            <button aria-expanded={isOpen} onClick={() => setOpenId(isOpen ? null : id)}>
              {title}
            </button>
            {isOpen && <p>{content}</p>}
          </div>
        );
      })}
    </div>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 3: Todo list

🟢 Beginner

**Requirements:** add a todo (ignore empty text), toggle done, delete. Use stable ids as keys. Bonus: show "n items left".

<details>
<summary>💡 Show solution</summary>

```jsx
function Todos() {
  const [todos, setTodos] = useState([]);
  const [text, setText] = useState('');

  const add = e => {
    e.preventDefault();
    const value = text.trim();
    if (!value) return;
    setTodos(t => [...t, { id: crypto.randomUUID(), text: value, done: false }]);
    setText('');
  };
  const toggle = id => setTodos(t => t.map(x => (x.id === id ? { ...x, done: !x.done } : x)));
  const remove = id => setTodos(t => t.filter(x => x.id !== id));
  const left = todos.filter(t => !t.done).length; // derived, not stored

  return (
    <>
      <form onSubmit={add}>
        <input value={text} onChange={e => setText(e.target.value)} placeholder="New todo" />
        <button>Add</button>
      </form>
      <ul>
        {todos.map(t => (
          <li key={t.id}>
            <label style={{ textDecoration: t.done ? 'line-through' : 'none' }}>
              <input type="checkbox" checked={t.done} onChange={() => toggle(t.id)} />
              {t.text}
            </label>
            <button onClick={() => remove(t.id)}>✕</button>
          </li>
        ))}
      </ul>
      <p>{left} items left</p>
    </>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 4: Fetch and display users

🟡 Intermediate

**Requirements:** fetch `https://jsonplaceholder.typicode.com/users` on mount; show *Loading…*, an error message, or the list of names; cancel the request on unmount.

<details>
<summary>💡 Show solution</summary>

```jsx
function Users() {
  const [state, setState] = useState({ status: 'loading', data: [], error: null });

  useEffect(() => {
    const controller = new AbortController();
    fetch('https://jsonplaceholder.typicode.com/users', { signal: controller.signal })
      .then(res => {
        if (!res.ok) throw new Error(`HTTP ${res.status}`);
        return res.json();
      })
      .then(data => setState({ status: 'success', data, error: null }))
      .catch(error => {
        if (error.name !== 'AbortError') setState({ status: 'error', data: [], error });
      });
    return () => controller.abort();
  }, []);

  if (state.status === 'loading') return <p>Loading…</p>;
  if (state.status === 'error') return <p role="alert">Error: {state.error.message}</p>;
  return <ul>{state.data.map(u => <li key={u.id}>{u.name}</li>)}</ul>;
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 5: Debounced search box

🟡 Intermediate

**Requirements:** as the user types, call an API only after they stop typing for 400 ms; ignore outdated responses; clear results when the input is empty.

<details>
<summary>💡 Show solution</summary>

```jsx
function useDebounce(value, delay) {
  const [debounced, setDebounced] = useState(value);
  useEffect(() => {
    const id = setTimeout(() => setDebounced(value), delay);
    return () => clearTimeout(id);
  }, [value, delay]);
  return debounced;
}

function Search() {
  const [query, setQuery] = useState('');
  const [results, setResults] = useState([]);
  const debounced = useDebounce(query.trim(), 400);

  useEffect(() => {
    if (!debounced) { setResults([]); return; }
    const controller = new AbortController();
    fetch(`/api/search?q=${encodeURIComponent(debounced)}`, { signal: controller.signal })
      .then(r => r.json())
      .then(setResults)
      .catch(() => {});
    return () => controller.abort(); // stale responses are cancelled
  }, [debounced]);

  return (
    <>
      <input value={query} onChange={e => setQuery(e.target.value)} placeholder="Search…" />
      <ul>{results.map(r => <li key={r.id}>{r.title}</li>)}</ul>
    </>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 6: `useLocalStorage` hook

🟡 Intermediate

**Requirements:** `const [value, setValue] = useLocalStorage('theme', 'light')` behaves like `useState` but persists the value. Handle invalid JSON and storage errors.

<details>
<summary>💡 Show solution</summary>

```jsx
function useLocalStorage(key, initialValue) {
  const [value, setValue] = useState(() => {
    try {
      const saved = localStorage.getItem(key);
      return saved !== null ? JSON.parse(saved) : initialValue;
    } catch {
      return initialValue;
    }
  });

  useEffect(() => {
    try {
      localStorage.setItem(key, JSON.stringify(value));
    } catch {
      /* storage full or unavailable */
    }
  }, [key, value]);

  return [value, setValue];
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 7: Star rating

🟡 Intermediate

**Requirements:** `max` stars (default 5); hovering previews the rating; clicking sets it; call `onChange(value)`; buttons must be accessible.

<details>
<summary>💡 Show solution</summary>

```jsx
function StarRating({ max = 5, onChange }) {
  const [rating, setRating] = useState(0);
  const [hover, setHover] = useState(0);

  return (
    <div onMouseLeave={() => setHover(0)}>
      {Array.from({ length: max }, (_, i) => {
        const value = i + 1;
        return (
          <button
            key={value}
            aria-label={`${value} star${value > 1 ? 's' : ''}`}
            onMouseEnter={() => setHover(value)}
            onClick={() => { setRating(value); onChange?.(value); }}
          >
            {value <= (hover || rating) ? '★' : '☆'}
          </button>
        );
      })}
    </div>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 8: Countdown timer

🟡 Intermediate

**Requirements:** start from N seconds; Start/Pause and Reset buttons; stop automatically at 0; no leaked intervals.

<details>
<summary>💡 Show solution</summary>

```jsx
function Countdown({ from = 10 }) {
  const [seconds, setSeconds] = useState(from);
  const [running, setRunning] = useState(false);

  useEffect(() => {
    if (!running) return;
    const id = setInterval(() => setSeconds(s => s - 1), 1000);
    return () => clearInterval(id);
  }, [running]);

  useEffect(() => {
    if (seconds === 0) setRunning(false);
  }, [seconds]);

  return (
    <div>
      <h2>{seconds}s</h2>
      <button onClick={() => setRunning(r => !r)} disabled={seconds === 0}>
        {running ? 'Pause' : 'Start'}
      </button>
      <button onClick={() => { setRunning(false); setSeconds(from); }}>Reset</button>
    </div>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 9: Modal with a portal

🔴 Advanced

**Requirements:** render into `document.body`; close on Escape and on overlay click (but not when clicking inside the dialog); remove listeners on close.

<details>
<summary>💡 Show solution</summary>

```jsx
import { useEffect } from 'react';
import { createPortal } from 'react-dom';

function Modal({ open, onClose, children }) {
  useEffect(() => {
    if (!open) return;
    const onKey = e => { if (e.key === 'Escape') onClose(); };
    document.addEventListener('keydown', onKey);
    return () => document.removeEventListener('keydown', onKey);
  }, [open, onClose]);

  if (!open) return null;

  return createPortal(
    <div className="overlay" onClick={onClose}>
      <div role="dialog" aria-modal="true" onClick={e => e.stopPropagation()}>
        {children}
      </div>
    </div>,
    document.body
  );
}
```

Bonus: move focus into the dialog on open and restore it on close.

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 10: Multi-step form (stepper)

🟡 Intermediate

**Requirements:** three steps; Back is disabled on the first step and Next on the last; show which step is current.

<details>
<summary>💡 Show solution</summary>

```jsx
const steps = ['Account', 'Profile', 'Confirm'];

function Stepper() {
  const [step, setStep] = useState(0);
  return (
    <div>
      <ol>
        {steps.map((name, i) => (
          <li key={name} aria-current={i === step ? 'step' : undefined}>{name}</li>
        ))}
      </ol>
      <button onClick={() => setStep(s => s - 1)} disabled={step === 0}>Back</button>
      <button onClick={() => setStep(s => s + 1)} disabled={step === steps.length - 1}>Next</button>
    </div>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 11: 🐞 Fix the bug: the counter that gets stuck

🟡 Intermediate

```jsx
function Timer() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    const id = setInterval(() => setCount(count + 1), 1000);
    return () => clearInterval(id);
  }, []);

  return <h1>{count}</h1>;
}
```

**Problem:** the number goes `0 → 1` and then stops. Why, and how do you fix it?

<details>
<summary>💡 Show solution</summary>

The effect runs once (`[]`), so the interval callback closes over `count = 0` forever – it always sets `0 + 1`. Use the **functional update** so it never needs `count`:

```jsx
useEffect(() => {
  const id = setInterval(() => setCount(c => c + 1), 1000);
  return () => clearInterval(id);
}, []);
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 12: 🐞 Fix the bug: the list that shows the wrong row

🟡 Intermediate

```jsx
function List() {
  const [items, setItems] = useState(['a', 'b', 'c']);

  const removeFirst = () => {
    items.shift();
    setItems(items);
  };

  return (
    <>
      <button onClick={removeFirst}>Remove first</button>
      {items.map((item, i) => <input key={i} defaultValue={item} />)}
    </>
  );
}
```

**Problem:** there are **two** bugs. Find them both.

<details>
<summary>💡 Show solution</summary>

1. `items.shift()` **mutates** state and then passes the same reference to `setItems`, so React may not re-render.
2. Using the **index as key** means that after removing the first row, the remaining inputs keep the wrong `defaultValue` (their internal DOM state is tied to the index).

```jsx
function List() {
  const [items, setItems] = useState([
    { id: 1, text: 'a' }, { id: 2, text: 'b' }, { id: 3, text: 'c' },
  ]);

  const removeFirst = () => setItems(prev => prev.slice(1));

  return (
    <>
      <button onClick={removeFirst}>Remove first</button>
      {items.map(item => <input key={item.id} defaultValue={item.text} />)}
    </>
  );
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**

### Exercise 13: Build a `useFetch` hook

🔴 Advanced

**Requirements:** `const { data, error, loading } = useFetch(url)`; re-fetch when `url` changes; cancel stale requests; reset state at the start of each request.

<details>
<summary>💡 Show solution</summary>

```jsx
function useFetch(url) {
  const [state, setState] = useState({ data: null, error: null, loading: true });

  useEffect(() => {
    const controller = new AbortController();
    setState({ data: null, error: null, loading: true });

    fetch(url, { signal: controller.signal })
      .then(res => {
        if (!res.ok) throw new Error(`HTTP ${res.status}`);
        return res.json();
      })
      .then(data => setState({ data, error: null, loading: false }))
      .catch(error => {
        if (error.name !== 'AbortError') setState({ data: null, error, loading: false });
      });

    return () => controller.abort();
  }, [url]);

  return state;
}
```

</details>

**[⬆ Back to Top](#table-of-contents)**


## 📅 Suggested 2-Week Study Plan

| Days | Focus |
| ---- | ----- |
| 1–2 | Core Concepts (JSX, props, state, keys, controlled inputs) |
| 3–4 | Hooks (`useState`, `useEffect`, `useRef`, `useMemo`, custom hooks) |
| 5–6 | Rendering & Performance, then Predict the Output |
| 7–8 | State Management & Data Fetching |
| 9 | Events, Forms & Routing |
| 10 | Advanced Patterns |
| 11 | Modern React (18/19), Server Components, Testing, a11y |
| 12–14 | Coding Exercises (timed, 20–30 min each) + Rapid-Fire Round |

## 🤝 Contributing

Found a mistake or want to add a question? Open an issue or a pull request. Please keep answers short, correct, and include a small code sample where it helps.

## 📄 License

MIT
