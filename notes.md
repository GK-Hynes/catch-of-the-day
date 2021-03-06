# Props and State

State is where your component's data lives, props are how the date gets where it needs to go.

## \$r

In Chrome and Firefox devtools, `$0` will give you the last element you clikced on. In React devtools, `$r` will do the same thing, giving you information such as props and state.

## Binding

All of the methods that come with React are in the original React.Component. When you make a component that extends that, any methods that you add are not bound by default.

It's difficult to reference a component inside one of its own methods. To solve this, bind the method inside the component's constructor.

Instead of declaring a component, you can declare a property and set it to an arrow function. A property will be bound to the component instance.

## Routing

Since the StorePicker component is a direct child of the Router component, it has access to certain props. This includes `history`. By pushing onto the `history` prop, React Router can route to a different component without reloading the page.

## State

State is essentially an object that lives inside a component and stores all the data that that component and maybe some of its children need.

State is the single source of truth. Instead of updating all the pieces of an app, update state and let React update everything.

Store state at the highets level possible. You can't pass this data up but you can pass it down.

The methods that update state need to live in the same component as state.
