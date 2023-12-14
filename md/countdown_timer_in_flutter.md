One of the reasons I created this package is that I often see displays on Tokopedia, an Indonesian e-commerce app, that show the remaining time of an item's promo. These displays are very useful and beautiful, and I wanted to make it easy for other developers to create similar ones in Flutter. So, let's jump into the code!

#### Tokopedia UI We Wanted to Clone: Countdown Timer

![Tokodepia Countdown Timer][i1]

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

**Output**

![Default SlideCountdown][i2]

But that's not what we're looking for. Let's further customize the SlideCountdown with leading icon

```dart
SlideCountdown(
  duration: Duration(hours: 2),
  icon: Padding(
    padding: EdgeInsets.only(right: 4),
    child: Icon(
      Icons.alarm,
      size: 20,
    ),
  ),
)
```

**Output**

![SlideCountdown with leading icon][i3]

Great, that's similar to what we want.

💡 Pro Tips.

> [SlideCountdown][pubdev] has property onDone, it will called when the countdown is finish, add function to refresh content or any thing you want!

[pubdev]: https://pub.dev/packages/slide_countdown
[i1]: https://raw.githubusercontent.com/farhanfadila1717/portofolio-data/main/images/b-1-1.png
[i2]: https://raw.githubusercontent.com/farhanfadila1717/portofolio-data/main/images/b-1-2.png
[i3]: https://raw.githubusercontent.com/farhanfadila1717/portofolio-data/main/images/b-1-3.png
