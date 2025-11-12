# 📸 react-native-lite-camera

A lightweight, fast, and easy-to-use React Native Camera module.
Perfect for developers who need simple camera functionality without heavy dependencies or complex setup.

🚀 Features
* 📷 Capture photos and videos effortlessly
* ⚡ Lightweight — minimal native code, fast startup
* 🔁 Live camera preview with customizable props
* 🎛️ Simple, declarative React Native interface
* 🧩 Compatible with both Android and iOS
* 🔒 Built with TypeScript for better DX and safety

## Installation

```sh
npm install react-native-lite-camera
```

## 📲 Usage Example

```js
import React from 'react';
import { View, Button } from 'react-native';
import { LiteCamera, useCamera } from 'react-native-lite-camera';

export default function App() {
  const { takePhoto, isRecording, startRecording, stopRecording } = useCamera();

  return (
    <View style={{ flex: 1 }}>
      <LiteCamera style={{ flex: 1 }} />
      <Button title="Take Photo" onPress={takePhoto} />
      <Button
        title={isRecording ? 'Stop Recording' : 'Start Recording'}
        onPress={isRecording ? stopRecording : startRecording}
      />
    </View>
  );
}
```

## Contributing

See the [contributing guide](CONTRIBUTING.md) to learn how to contribute to the repository and the development workflow.

## License

MIT
