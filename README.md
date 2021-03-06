
# react-native-sound-playerview
[![npm](https://img.shields.io/npm/v/react-native-sound-playerview.svg)](https://npmjs.com/package/react-native-sound-playerview) [![npm](https://img.shields.io/npm/dm/react-native-sound-playerview.svg)](https://npmjs.com/package/react-native-sound-playerview)

audio player view for iOS/Android using with [react-native-sound](https://github.com/zmxv/react-native-sound) and `react-navigation`

<img src="https://github.com/benevbright/react-native-sound-playerview/blob/master/docs/demo.gif?raw=true">

## Install

```shell
npm i --save git+https://github.com/lichmac/react-native-sound-playerview.git
```

Then install the dependencies

```shell
npm install @react-native-community/slider --save
npm install react-native-sound --save

### Step 1. Register Screen with `react-navigation`

```
import {StackNavigator} from 'react-navigation';
import PlayerScreen from 'react-native-sound-playerview'

...

const Navigation = StackNavigator({
    ...
    player:{screen:PlayerScreen},
    ...
})

...
```

### Step 2. Navigate to 'react-native-sound-playerview'
```
this.props.navigation.navigate('player', {title:__TITLE__, filepath:__AUDIO_FILEPATH__});
```
*NOTE: `filepath` should be a full file path.
