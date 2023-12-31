# SVG Clicklistener| Flutter Package

[Flutter][flutter_dev_link] package for set clicklistener on elements inside svg. The package has been written solely in [Dart][dart_dev_link] language.

<div align="center">

[![animated_svg][build_status_badge]][workflow_link]
![coverage][coverage_badge]
[![style: very good analysis][very_good_analysis_badge]][very_good_analysis_link]
[![License: MIT][license_badge]][license_link]

</div>


## Features

A powerful and fully customizable widget. With this package, you can click on SVG  elements

## Getting started

Let's take a look at how to implement `flutter_svg_click_listener`

First, add the following line to `pubspec.yaml`:
```yaml
flutter_svg_click_listener: ^0.0.7
```

Second, import `flutter_svg_click_listener`:
```dart
import 'package:flutter_svg_click_listener/flutter_svg_click_listener.dart';
```

## Usage

Basic usage example: 

`main.dart`
```dart
// Define svgString
late final String svgString;

@override
void initState() {
    // Initialize svgString
    svgString = await loadSvgStringFromAssets("assets/svg/sample.svg");
    super.initState();
}

@override
Widget build(BuildContext context) {
    // Call the SvgImage widget anywhere in your widget tree.
    return SvgImage(
            onElementClick: (val) {
              print("element id is $val")
            },
            svgString: document != null ? document.toString() : "");
}
```

## Example

More examples can be found in `/example` folder on [GitHub][animated_svg_github_link]. 

## Additional information

This package has been written solely in Dart Language yet it has the [flutter_svg][flutter_svg_link] as a dependency.

For more information please visit [GitHub][flutter_svg_click_listener].

## Feature requests and bugs

Please file feature requests and bugs at the [issue tracker][animated_svg_issue_link].
