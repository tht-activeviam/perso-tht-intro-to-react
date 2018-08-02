# perso-tht-intro-to-react
Project for ReactJS official tutorial

## Notes
- To collect data from multiple children, or to have two child components communicate with each other, you need to declare the shared state in their parent component instead. The parent component can pass the state back down to the children by using props; this keeps the child components in sync with each other and with the parent component.
- Change the state without mutation. It helps react to determine when to re-render.
- Functional components have no state and render using properties only.