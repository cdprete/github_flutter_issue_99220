# demo_routing_issue

A Flutter project demoing https://github.com/flutter/flutter/issues/99220

## Getting Started

1. Start the application in Chrome
2. Press the `settings` icon
3. Observe that it's still possible to go back from the browser history even if 
    ```dart
    Navigator.pushNamedAndRemoveUntil(context, SettingsView.routeName, (route) => false)
    ```
    has been used.