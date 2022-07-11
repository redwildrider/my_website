---
layout: posts
title:  "[WIP:] Adding multiple FlutterViews to Android app"
---

## Introduction
<!-- TODO: maybe add TL;DR paragraph -->
Last month, as a mobile developer at [Nutrilize](https://nutrilize.app/), I had to find a way to combine our iOS and Android app in order to simplify and speed up the development of new features in the future. In my opinion, [Flutter](https://flutter.dev/) clearly is the best option to accomplish this task nowadays. You only have one source code for basically all platforms you can think of, backed up by a great community, plenty of nice plugins and the dart programming language, which I really enjoy working with.

The challenge I had was the fact that there already are two huge repositories - one for the iOS app, the other one for the Android app - and it would have taken way too long to rewrite the whole code in Flutter. Hence, we decided to replace the code incrementally - feature by feature, which should be no problem as Flutter already features [add-to-app](https://docs.flutter.dev/development/add-to-app) support. However, the real problem here is that some features can still be considered *experimental* and the Flutter website did not document them as well as most other parts of its website. Especially when the project is more complex and you want to integrate various functionalities in flutter to multiple parts of your native Android app (iOS support will be coming soon, hopefully).

Therefore, the purpose of this blog entry was born - to improve the Flutter add-to-app documentation and lower the hurdle for you when you want to accomplish the same thing i did. You will learn to add FlutterViews to your Android app, connect them with the according Flutter code you wrote and finally establish communication between Flutter and Android code with the help of method channels.

NOTE: the following tutorial is one way to do this. There are definitely other ways to accomplish the task too. However, in my experience I find this to be the most promising one at the moment.

## Integration of Flutter into the Android app

You can find the Android app [here](https://github.com/redwildrider/add_flutter_views_to_android/tree/main/android). It simply consists of one Activity and two Fragments. At the end of the tutorial, each fragment should show include a different FlutterView.

In order to integrate your Flutter module into your Android project, simply follow the [official tutorial](https://docs.flutter.dev/development/add-to-app/android/project-setup). I prefer to use the manual Integration using *Option B - Depend on the module’s source code*.

## Flutter app

## Adding FlutterView

## Communication via method channel

## Conclusion