# perso-tht-intro-to-react
Project for ReactJS official tutorial

## Notes
- To collect data from multiple children, or to have two child components communicate with each other, you need to declare the shared state in their parent component instead. The parent component can pass the state back down to the children by using props; this keeps the child components in sync with each other and with the parent component.
- Change the state without mutation. It helps react to determine when to re-render.
- Functional components have no state and render using properties only.
- To add item to array, use concat() instead of push() to avoid mutation.
- 'key' is a special and reserved property in React. It’s strongly recommended that you assign proper keys whenever you build dynamic lists. Keys do not need to be globally unique. Keys only needs to be unique between components and their siblings. When a list is re-rendered, React takes each list item’s key and searches the previous list’s items for a matching key. If the current list has a key that does not exist in the previous list, React creates a component. If the current list is missing a key that exists in the previous list, React destroys a component. Keys tell React about the identity of each component which allows React to maintain state between re-renders. If a component’s key changes, the component will be destroyed and re-created with a new state. Using the array index as a key is problematic when trying to re-order a list’s items or inserting/removing list items.