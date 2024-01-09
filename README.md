# auto_scrolling_image
make an assets folder in root of the project:

|<img width="241" alt="image" src="https://github.com/johnhcolani/auto_scrolling_image/assets/91166301/5ff98268-2aa2-4b44-8327-948532177673">|


Add two items to pubspec.yaml
- add auto_scroll_image to the dependencies
- open assets path
  
```
dependencies:
  flutter:
    sdk: flutter

  cupertino_icons: ^1.0.6
  auto_scroll_image: ^0.2.2-dev

assets:
  - assets/

dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^3.0.0
flutter:
  uses-material-design: true

```
import :
```
import 'package:auto_scroll_image/auto_scroll_image.dart';
```

then add AutoScrollImage to your class:
```
home: Scaffold(
        appBar: AppBar(
          title: Text('Your App'),
        ),
        body: const Column(
          mainAxisAlignment: MainAxisAlignment.center,
          crossAxisAlignment: CrossAxisAlignment.center,
          children: [
            // Your other widgets can go here

            // Example usage of AutoScrollImage
            AutoScrollImage(
              itemCount: 10, // Customize itemCount
              itemWidth: 50.0, // Customize itemWidth
              autoScrollDuration: Duration(seconds: 2), // Customize autoScrollDuration
              timerInterval: Duration(seconds: 2), // Customize timerInterval
            ),

            // More of your widgets can follow here
          ],
        ),
      ),
```
<img width="342" alt="image" src="https://github.com/johnhcolani/auto_scrolling_image/assets/91166301/738441ad-f38c-4cbc-ad40-bf073ed056a4">



<img width="1196" alt="image" src="https://github.com/johnhcolani/auto_scrolling_image/assets/91166301/62b9e6d2-c5ef-4266-85ed-484f6156cc52">
