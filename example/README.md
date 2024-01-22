# /example/lib/main.dart

```dart
import 'package:flutter/material.dart';
import 'package:typing_text/typing_text.dart'; // Ensure this package is imported

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Typing Text Demo',
      theme: ThemeData(
        primarySwatch: Colors.blue,
      ),
      home: const TypingTextDemo(),
    );
  }
}

class TypingTextDemo extends StatefulWidget {
  const TypingTextDemo({super.key});

  @override
  State<TypingTextDemo> createState() => _TypingTextDemoState();
}

class _TypingTextDemoState extends State<TypingTextDemo> {
  // Define the list of words to be displayed
  final List<String> _words = [
    'Just',
    "can't",
    'stop',
    'typing!',
  ];

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Padding(
        padding: const EdgeInsets.all(32),
        child: Center(
          child: TypingText(
            words: _words,
            letterSpeed: const Duration(milliseconds: 100),
            wordSpeed: const Duration(milliseconds: 1000),
            style: const TextStyle(
              fontSize: 24,
              fontWeight: FontWeight.bold,
            ),
          ),
        ),
      ),
    );
  }
}
```
