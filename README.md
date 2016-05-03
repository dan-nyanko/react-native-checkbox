WARNING: This is significantly modified fork of `react-native-checkbox` that allows
for any custom component to be used as the checked and unchecked state.

# react-native-checkbox
Checkbox component for React native

## Installation:

Add the following to your package.json

```
"react-native-checkbox": "https://github.com/dan-nyanko/react-native-checkbox#master",
```


## Simple example using react-native-vector-icons:
```jsx
<CheckBox
  label='Label'
  checked={true}
  onChange={(checked) => console.log('I am checked', checked)}
  uncheckedComponent={<Icon name='circle-o' size={28} color='#FEABAB' />}
  checkedComponent={<Icon name='check-circle' size={28} color='#BDE3A7' />}
/>
```

## Props:

- `label` : text that will be displayed along the checkbox
- `labelBefore` : position the label before the checkbox (boolean). The default
value is false
- `checkedComponent` : component that will be used as the checked state
- `uncheckedComponent` : component that will be used for the unchecked state
- `labelStyle` : style object that will be applied to the label
- `checked` : initial checked value
- `onChange` : callback function that will be invoked with the toggled checked property as argument.
