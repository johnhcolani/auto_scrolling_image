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
final result would be on Android:
![Screenshot_20240108_213105](https://github.com/johnhcolani/auto_scrolling_image/assets/91166301/ba9e2a51-7554-4cca-8d1d-62ac0d7268b2)

iOS:
![image](https://github.com/johnhcolani/auto_scrolling_image/assets/91166301/0a4b1660-44b0-4416-9945-b1cca952b915)

macOS:
<img width="806" alt="image" src="https://github.com/johnhcolani/auto_scrolling_image/assets/91166301/bd2f408d-91c1-4611-a0dc-000e508d3db7">





<img width="1196" alt="image" src="https://github.com/johnhcolani/auto_scrolling_image/assets/91166301/62b9e6d2-c5ef-4266-85ed-484f6156cc52">
