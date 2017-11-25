# React Native Timer Countdown
A customizable countdown component for React Native.

## Install

```sh
npm install --save react-native-timer-countdown`
```

or

```sh
yarn add react-native-timer-countdown
```

## Usage

```javascript
import TimerCountdown from 'react-native-timer-countdown'

render() {
    return (
        <TimerCountdown
            initialSecondsRemaining={360}
            onTick={() => console.log('tick')}
            onTimeElapsed={() => console.log('complete')}
            allowFontScaling={true}
            style={{ fontSize: 20 }}
        />
    )
}
```

## Props
| Name | Description | Type | Required | Default Value |
| :--- | :----- | :--- | :---: | :---: |
| initialSecondsRemaining | The time remaining for the countdown (in ms) | number | ✓ |  |
| interval | The time between timer ticks (in ms). | number | ✓ | 1000ms |
| allowFontScaling | to allow font scaling | bool |  | false |
| style | The custom styling which will be applied to the Text component | style |  |  |
| formatFunc | A function that formats the secondsRemaining | func | | |
| onTick | A function to call each tick | func | | |
| onTimeElapsed | A function to call when the countdown completes | func |  | |

## Author

Avid21

## License

MIT