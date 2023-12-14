One of the reasons I created this package is that I often see displays on Tokopedia, an Indonesian e-commerce app, that show the remaining time of an item's promo. These displays are very useful and beautiful, and I wanted to make it easy for other developers to create similar ones in Flutter. So, let's jump into the code!

Tokopedia UI We Wanted to Clone: Countdown Timer
<br>
<img src="https://raw.githubusercontent.com/farhanfadila1717/portofolio-data/main/images/b-1-1.png" alt="Tokopedia Countdown Timer" width="400"/>
<br>
<br>
Before we started please like [SlideCountdown][pubdev] package it's one of my os package 👍.

First add [SlideCountdown][pubdev] to `pubscpec.yaml` or you can run

```shell
flutter pub add slide_countdown
```

The basic example use [SlideCountdown][pubdev] package is

```dart
SlideCountdown(
  duration: const Duration(days: 2),
),
```

Output
[image]
<br>
But that's not what we're looking for. Let's further customize the SlideCountdown with leading icon
<br>

```dart
SlideCountdown(
  icon: Icon(
     Icons.alarm,
     color: Colors.white
  ),
  duration: const Duration(days: 2),
),
```

output
[image]

Great, that's similar to what we want.

💡 Pro Tips.

> [SlideCountdown][pubdev] has property onDone, it will called when the countdown is finish, add function to refresh content or any thing you want!

[pubdev]: https://pub.dev/packages/slide_countdown
