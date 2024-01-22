<!--
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages).

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages).
-->

A customizable, animated text widget for Flutter apps, simulating the effect of typing.
This package is ideal for creating engaging text animations, such as typing effects in chatbots, creative text displays in storytelling apps, or any application where text needs to be displayed dynamically and with visual flair.

## Features

* Animated Typing Effect: Simulates a character-by-character text typing animation that cycles between words.
* Customizable Speed: Control the speed of typing and the delay between words.
* Handles State Changes: Seamless transition when rebuilding the widget with a new list of words.

![Typing Text GIF](https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExbW9yczh3Mmx6ZHR6NHgxcmVxNWRvOWdodWg2c3hrazY4M29jbm5sZSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/guGGYsKLCjFiacvLdK/giphy.gif)

## Getting started

To use the typing_text package in your Flutter app, first add the dependency to your pubspec.yaml:

```yaml
dependencies:
  typing_text: ^0.1.0
```

Then, import the package in your Dart file:

```dart
import 'package:typing_text/typing_text.dart';
```

## Usage

```dart
TypingText(
  words: ['Hello', 'World'],
  letterSpeed: Duration(milliseconds: 100),
  wordSpeed: Duration(milliseconds: 1000),
  style: TextStyle(fontSize: 24, fontWeight: FontWeight.bold),
)
```

## Additional information

For more information, bug reports, feature requests, or contributions, please visit the [GitHub repository](https://github.com/CameronMcClymont/typing_text).

Feedback and contributions are welcome!
