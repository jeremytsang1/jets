+++
title = "OSU CS 467: Blog Post # 2"
author = ["Jeremy Tsang"]
categories = ["CS 467"]
draft = true
+++

## Overview {#overview}

The project I am working on is the [Forest Wellness Checkup App](https://eecs.engineering.oregonstate.edu/capstone/submission/pages/viewSingleProject.php?id=g8UDl6xlaVI8s16E), which is a
cross platform mobile app designed to aid forestry professionals in the
field. At the time of this writing we are about half way into the capstone
course however we are only just finished in the second week of development. As
such, our team has not yet gotten into the nitty gritty of all the other
technologies we will use for our project including libraries for PDF
manipulation, DOCX manipulation, stylus control, and digital ink
recognition. In contrast, we have been very involved in the initial layout of
the mobile and getting more and more familiar with the Flutter and Dart
SDKs. There have been some pain points (mainly learning curve) but so far the
Flutter/Dart SDKs have been my favorite technology mainly due to three things:
Flutter's built-in widgets, cross platform development, and developer
experience. Personally I believe the pros outweigh the cons for this project.


## Learning Curve {#learning-curve}

First, lets start with the bad: outside of Flutter, Dart is rarely seen in the
wild. For this reason there is a high chance that if a developer has not worked
on a Flutter app, said developer probably is not familiar with Dart. This leads
to the inevitable challenge that is simultaneously learning a new language and
as well as a framework which can be a tall order. Our team,of course, had to
take some time to work through this during our first week of
development. Despite both my team members having no prior experience with Dart
they were both able to get up to speed due to its similarities with other
languages. Flutter, on the other hand has been, a bit more challenging in that
layouts are a bit different than what one is used to when developing for web.


## Built-in Widgets {#built-in-widgets}

However, this is where the benefits start coming in handy namely the
declarative widget system that Flutter employs. There are a myriad of widgets
to do nearly any layout task we can imagine. Further if there are layouts that
they do no exactly cover we can create our own through composition. This has
been great to avoid re-inventing the wheel for many common layouts we needed
for our app. Moreover the built-in widgets are documented in great detail at
[flutter.dev](https://docs.flutter.dev/) in addition to videos on many common widgets as well as cookbooks
for frequently used tasks. In regards to styling, these widgets do not need a
separate language (like CSS for React) which allows a single language for
layout, styling, and logic.


## Cross Platform {#cross-platform}

Another benefit that helps mitigate the time sink into the learning curve is
the fact that Flutter is inherently cross platform. As Flutter can build apps
for Android, iOS, web, Desktop we can just keep a single codebase for the
entire project. Comparing this to Native apps where we would need both Kotlin
and Swift this reduces the amount of work we have to do as a mere three person
team. Unfortunately one limitation here is that to build/test iOS apps one must
still use Xcode and hence have access to a macOS device or appropriate
virtualization tools.


## Developer Experience {#developer-experience}

Finally, Flutter toolchain makes the developer experience very pleasant. Since
the Dart SDK comes bundled with linter ([dart analyze](https://dart.dev/tools/dart-analyze)), formatter ([dart format](https://dart.dev/tools/dart-format)),
and even [language server](https://github.com/dart-lang/sdk/tree/main/pkg/analysis_server) (one less thing to install for Emacs and Vim users)
just having the Dart SDK provides quite a few development tools out of the
box. This saves developers new to the framework from having to hunt down and
install these tools. Further, the language server provides access to another
useful development tool [dart fix](https://dart.dev/tools/dart-fix) so when developing, ones editor/IDE can make
suggestions and even perform refactoring based off the results of the
linter. For example if one wanted to change a widget from [stateless](https://api.flutter.dev/flutter/widgets/StatelessWidget-class.html) to
[stateful](https://api.flutter.dev/flutter/widgets/StatefulWidget-class.html), one need only consult their editor/IDE and choose the appropriate
"code action" instead of rewriting the entire class by hand (which would be
more error prone). Other code actions work directly on the widget tree by
wrapping widgets, removing them, or even extracting them to separate
variables/methods/classes. In addition to the aforementioned tools there are
also Flutter specific tools like hot reload/start (saves a huge amount of time
instead of recompiling each time) and the Flutter dev tools (widget inspector,
profiler, and friends) that provide even more help out of the box.


## Closing Remarks {#closing-remarks}

Despite the initial learning curve I believe that the Flutter/Dart SDK is the
right choice for this project. It saves a huge amount of time being cross
platform but also makes the process of actually writing the app pleasant and
quick as well. This app does not need a large number of esoteric features so I
think the more mature ecosystem of a framework like React Native is
unwarranted. I'm happy with Flutter and Dart so far.
