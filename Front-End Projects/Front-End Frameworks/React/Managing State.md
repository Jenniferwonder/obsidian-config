---
title: Managing State
tags: Coding/React
started: 2023-02-14 Tue
due:
modified: 2023-02-14 Tue
status:
---
#### 1. [Reacting to Input with State • React](https://beta.reactjs.org/learn/reacting-to-input-with-state)
1.  **Identify** your component’s different visual states
2.  **Determine** what triggers those state changes (Human/ computer input)
3.  **Represent** the state in memory using `useState`
4.  **Remove** any non-essential state variables
5.  **Connect** the event handlers to set the state
#### 2. [Choosing the State Structure • React](https://beta.reactjs.org/learn/choosing-the-state-structure)
-   When to use a single vs multiple state variables
-   What to avoid when organizing state
-   How to fix common issues with the state structure
#### 3. [Sharing State Between Components • React](https://beta.reactjs.org/learn/sharing-state-between-components#recap)
-   When you want to coordinate two components, move their state to their common parent.
-   Then pass the information down through props from their common parent.
-   Finally, pass the event handlers down so that the children can change the parent’s state.
-   It’s useful to consider components as “controlled” (driven by props) or “uncontrolled” (driven by state).
#### 4. [Preserving and Resetting State • React](https://beta.reactjs.org/learn/preserving-and-resetting-state)
-   How React “sees” component structures
-   When React chooses to preserve or reset the state
-   How to force React to reset component’s state
-   How keys and types affect whether the state is preserved
#### 5. [Extracting State Logic into a Reducer • React](https://beta.reactjs.org/learn/extracting-state-logic-into-a-reducer)