# React Native Pulser
A simple library to create pulse animation in react native

<!-- ![react native pulse](https://raw.githubusercontent.com/sahlhoff/react-native-pulse/master/pulse-gif.gif) -->

### Installation
```bash
npm install react-native-pulse --save
```

### Example

```js
import Pulser from 'react-native-pulser';

const App = ({}) => (
  <Pulser
    //props
  />
);
```


### API

| Property       | Type          | Default             | Description |
| -------------  |:-------------:|:------------:       | ----------- |
| interval       | number        | 2000                | action buttons visible or not
| size           | number        | 100                 | width and height of the avatar
| pulseMaxSize   | number        | 250                 | maximum size of the pulse in the background
| avatar         | string        | undefined           | **required** avatar url to display
| pressInValue   | number        | 0.8                 | should be between 0 and 1. scale of the avatar, when pressed in
| pressDuration  | number        | 150                 | duration of the scale animation
| pressInEasing  | Easing        | Easing.in           | easing type of the press in animation
| pressOutEasing | Easing        | Easing.out          | easing type of the press out animation
| borderColor    | string        | '#D8335B'           | border color of the pulse
| backgroundColor| string        | '#ED225B55'         | background color of the pulse
| getStyle       | function      | undefined           | override the styling of the pulse. gets as parameter the Animated variable. e.g. (anim) => ({ backgroundColor: 'yellow' })
