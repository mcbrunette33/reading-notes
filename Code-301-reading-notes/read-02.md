## Read 03

- React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

- Mounting: When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

- Render: Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders.

- componentDidMount: This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here.

- mounting---> constructor---->render--->componentDIDMount or render---.componentDIDUpdate // unmounting---->componentWillUnmount

- Passing through props: Initial count inside, title, subtitle, 

- Props VS State : The key difference between props and state is that state is internal and controlled by the component itself while props are external and controlled by whatever renders the component.State is handled inside. props are handled outside

- React re-renders a component when you call the setState function to change the state . As a result, the child components only update when the parent component's state changes with one of those functions.

- using react when we are working with any data, we always use state for storing that data which may be a string , number or any complex object .
