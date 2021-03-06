Sizes 

```js
initialState = {
  value1: 0,
  value2: 0,
  value3: 0,
};

<React.Fragment>
  <div className="mb5 flex">
    <NumericStepper
      label="Regular"
      value={state.value1}
      onChange={event => setState({ value1: event.value })}
    />
  </div>
  <div className="mb5 flex">
    <NumericStepper
      label="Large"
      size="large"
      value={state.value2}
      onChange={event => setState({ value2: event.value })}
    />
  </div>
  <div className="mb5 flex">
    <NumericStepper
      label="Extra large"
      size="x-large"
      value={state.value3}
      onChange={event => setState({ value3: event.value })}
    />
  </div>
</React.Fragment>
```

Minimum and maximum values
```js
initialState = {
  value1: 1,
  value2: 0,
  value3: 0,
};

<React.Fragment>
  <div className="mb5">
    <NumericStepper
      label="Minimum value = 1"
      minValue={1} 
      value={state.value1}
      onChange={event => setState({ value1: event.value })}
    />
  </div>
  <div className="mb5">
    <NumericStepper
      label="Minimum 2, maximum 6"
      minValue={2}
      maxValue={6}
      value={state.value2}
      onChange={event => setState({ value2: event.value })}
    />
  </div>
  <div className="mb5">
    <NumericStepper
      label="No minimum value (allows negative values)"
      minValue={null}
      value={state.value3}
      onChange={event => setState({ value3: event.value })}
    />
  </div>
</React.Fragment>
```

Box types
```js
<React.Fragment>
  <div className="mb5">
    <NumericStepper
      label="Default"
      size="x-large"
      value={1}
      onChange={()=>{}}
    />
  </div>
  <div className="mb5">
    <NumericStepper
      label="Block"
      size="x-large"
      value={1}
      block
      onChange={()=>{}}
    />
  </div>
</React.Fragment>
```
