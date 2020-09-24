# How it works in known frameworks?

`State` is the essence of frameworks. It's what **changes** in applications.

Each `state` modification will make the concerned component to `re-render` its template with the according `state` new values.

## State in Vuejs

```javascript
const component = new View({
  data() {
    // initial state
    return { firstName: "Ashutosh" };
  },
  methods: {
    changeName() {
      // modifying the state
      this.firstName = "Singh";
    }
  }
});
```

## State in Angular

```javascript
// initial state
this.firstName = "Ashutosh";

// modifying the state
handleClick() {
	this.firstName = "Singh";
}
```

## State in React

```jsx
// initial state
this.state = { firstName: "Ashutosh" };

// modifying the state
this.setState({ firstName: "Singh" });
```
