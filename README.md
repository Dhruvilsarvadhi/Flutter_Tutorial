
># <center/> **Flutter Tutorial** #

>## [What is Flutter?](https://www.geeksforgeeks.org/what-is-flutter/)

>>Flutter is an open source mobile application development framework created by Google. It is used to create locally compiled applications for mobile, web and desktop from a single code base.

>>One of the most important features of Flutter is its fast development cycle. Flutter’s ”reinstall while running” feature allows developers to quickly and easily test changes to their code by updating the application in real time without having to manually rebuild and deploy it.

> ---

>## [What is the purpose of the runApp function in Flutter?](https://www.codepur.dev/what-is-runapp-in-flutter/#:~:text=n%20Flutter%2C%20the%20runApp(),be%20rendered%20on%20the%20screen.)
 
>> The runApp() method is used to initialize and run the app. It takes in a Widget as its argument, which is typically the root of the app's widget hierarchy. This widget is then passed to the FlutterEngine to be rendered on the screen.

>>The runApp() method is typically called in the main() function of a Flutter app, which is the starting point of the app's execution. The main() function is the entry point of the app and it is the first method that is executed when the app starts.

> ---

>## [What is Materialapp in Flutter?](https://medium.com/flutterfly-tech/introduction-to-flutter-getting-started-with-materialapp-scaffold-fccacb9631a9)

>>MaterialApp is a widget that introduces the Navigator and Theme widgets required to create a material design app. Scaffold Widget is a MaterialApp component that provides numerous fundamental features such as AppBar, BottomNavigationBar, Drawer, FloatingActionButton,etc.

> ---

>## [What is StatelessWidget in Flutter?](https://medium.com/@milankathiriya/what-is-statelesswidget-in-flutter-4932bb11e498)

>>A stateless widget cannot change its state during the runtime of a Flutter application. That means a stateless widget cannot be redrawn while the app is in action. For that reason, the appearance and properties remain unchanged throughout the lifetime of the widget.

> ---

>## [What is StatelessWidget in Flutter?](https://medium.com/@milankathiriya/what-is-statefulwidget-in-flutter-6e043c4cbda9)

>>A stateful widget is used when some part of the UI must change dynamically during runtime. Stateful widgets can redraw themselves multiple times while the app is running.

> ---

>## [Stateless vs Stateful widget lifecycle in Flutter](https://anmol-gupta.medium.com/stateless-vs-stateful-widget-in-flutter-b0a25ccd0707)

>>Stateless widget
```
   import 'package:flutter/material.dart';
     void main() => runApp(MyApp());
        class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Container();
  }
}
```
>>Stateful widget
```
class DemoWidget extends StatefulWidget {
  @override
  _DemoWidgetState createState() => _DemoWidgetState();
}
class _DemoWidgetState extends State<DemoWidget> {
  @override
  void initState() {
    // TODO: implement initState
    super.initState();
  }
  @override
  void didChangeDependencies() {
    // TODO: implement didChangeDependencies
    super.didChangeDependencies();
  }
  @override
  void didUpdateWidget(covariant DemoWidget oldWidget) {
    // TODO: implement didUpdateWidget
    super.didUpdateWidget(oldWidget);
  }
  @override
  // TODO: implement mounted
  bool get mounted => super.mounted;
  @override
  void dispose() {
    // TODO: implement dispose
    super.dispose();
  }
  @override
  void deactivate() {
    // TODO: implement deactivate
    super.deactivate();
  }
  String text = "Stateful widget example";
  @override
  Widget build(BuildContext context) {
    return InkWell(
      onTap: () {
        setState(() {
          text = "Stateful widget with setState example";
});
      },
      child: Text(text),
    );
  }
}
```

> ---

>## [What is the concept of Widgets in Flutter?](https://medium.com/jay-tillu/4-what-is-widget-in-flutter-lets-clear-the-basics-first-82f501c8d0f0)

>>Each element on a screen of the Flutter app is a widget. The view of the screen completely depends upon the choice and sequence of the widgets used to build the apps. And the structure of the code of an apps is a tree of widgets. [click here](https://www.geeksforgeeks.org/what-is-widgets-in-flutter/)

> ---

>## [What is the column and row?](https://medium.flutterdevs.com/know-your-widgets-row-and-column-7315d32cb07d)

>>So, the next widget in our series is not just a single widget, in fact, we would be covering two different widgets in this blog, namely Row and Column. The reason behind integrating two widgets together is the fact these two widgets have similar properties which will help you understand them efficiently.

> ---

>## [How is the Scaffold widget used in Flutter?](https://medium.flutterdevs.com/know-your-widgets-scaffold-in-flutter-292b8bc1281)

>>The Scaffold is a widget in Flutter used to implements the basic material design visual layout structure. It is quick enough to create a general-purpose mobile application and contains almost everything we need to create a functional and responsive Flutter apps. This widget is able to occupy the whole device screen.

> ---

>## [How can third-party packages be integrated into a Flutter project?](https://medium.com/@jessanirahim/integrating-native-third-party-sdk-in-flutter-8aab03afa9da)

>>Flutter is an SDK developed by the giant Google for building expressive and flexible native apps for iOS and Android from a single codebase.
Flutter shows high-performance, high-fidelity, and fast development. The flexible and expressive nature of UI components which helps it gain a lot of wows by app developers in little span of time.

> ---

>## [How can images and fonts be added to the project's assets in Flutter?](https://zubairehman.medium.com/how-to-use-custom-fonts-images-in-flutter-package-c2d9d4bfd47a)

```
name: my_flutter_app
description: A new Flutter application.

dependencies:
  flutter:
    sdk: flutter

  cupertino_icons: ^0.1.2

dev_dependencies:
  flutter_test:
    sdk: flutter

flutter:
  uses-material-design: true,
  assets:
    - images/lake.jpg
```   

> ---

>## [What is a constructor in Flutter?](https://medium.flutterdevs.com/exploring-dart-constructors-345398a0e4c5#:~:text=The%20constructor%20is%20called%20when,characterize%20its%20very%20own%20constructor.)

>>In object-oriented programming when an object is made, it is naturally called the constructor. All classes have their default constructor which is made by the compiler when the class is called, besides one can likewise characterize its very own constructor. Yet, you should take note that if you do such, the default constructor won’t be made and will be overlooked.

> ---

>## [What is state management in Flutter and what are some methods used for it?](https://medium.com/flutter-community/a-list-of-state-management-approaches-in-flutter-1481ba522a51)

>>This type of programming requires state management to handle such a situation to improve performance. It is because every time you make a change or update the same, the state gets refreshed. In Flutter, the state management categorizes into two conceptual types, which are given below: Ephemeral State. [click here](https://medium.com/@milankathiriya/what-is-state-in-flutter-describe-types-of-states-in-detail-22af620ba7d5)
```
 * Provider
 * Riverpod
 * setState
 * InheritedWidget & InheritedModel
 * Redux
 * Fish-Redux
 * BLoC / Rx
 * GetIt
 * MobX
 * Flutter Commands
 * Binder
 * GetX
 * states_rebuilder
 * Triple Pattern (Segmented State Pattern)
 * solidart
 * flutter_reactive_value
```

> ---

>## [What is the Flutter lifecycle?](https://medium.com/flutter-community/a-list-of-state-management-approaches-in-flutter-1481ba522a51)

>>Types of Lifecycle\
  (1) [Flutter App lifecycle](https://medium.com/pharos-production/flutter-app-lifecycle-4b0ab4a4211a)\
  (2) [Flutter Widget lifecycle](https://medium.flutterdevs.com/app-lifecycle-in-flutter-c248d894b830#:~:text=The%20lifecycle%20of%20the%20Flutter,think%20about%20Widgets%20in%20Flutter.)

> ---

>## [What is the significance of code structure in Flutter?](https://medium.com/flutter-community/scalable-folder-structure-for-flutter-applications-183746bdc320#:~:text=Selecting%20the%20right%20folder%20structure,when%20working%20with%20a%20team.)

>>Selecting the right folder structure for your Flutter application is an important decision and will directly affect the maintainability, scalability, and ease of use when working with a team
```
--lib
  |--screens
  |--widgets
  |--services
  |--view_models
  |--services
```