<!-- logo IMG -->
<p align="center">
    <img width="340" src="github/dash.gif" alt="Vite logo">
  </a>
</p>

<!-- - --- --- --- Create -- --- --- ---  -->
## Create / Export 💙
**🐥 Create App Flutter**
1. Type these command for crete flutter project in CMD 

- `flutter create name_app`
  <details>

    >- `flutter create name_app`
    >- `flutter create --platforms ios,android name_app`

    > **Warning**
    > Use FVM only you installed .

    >- `fvm flutter create name_app`
    >- `fvm flutter create --platforms ios,android name_app`
  </details>

<!-- - --- --- --- Export -- --- --- ---  -->
**🐲 Export App Flutter**

1. If you want to export for Android

- `flutter build apk`
  <details>

    > **Warning**
    > Use for KEY in Android .

    ```
         storePassword=<password_de_clave>
         keyPassword=<password_de_alias>
         keyAlias=<name_de_alias>
         storeFile=<name_de_clave>.keystore
    ```
    >- `flutter build apk --release`
    >- `flutter build apk --target-platform android-arm,android-arm64`
  </details>


2. If you want to export for iOS

- `flutter build ios`
  <details>

    > **Warning**
    > Use foe KEY in iOS .
    >- `open ios/Runner.xcworkspace`
  </details>

<!-- logo IMG -->
## Flutter Setting  🌱

>An open source application built using the new router, server components and everything new in Flutter.

**Artificial Intelligence 🦄** 
<!-- -- --- -- -- -- logo IMG -- --- -- --- --->
- [x] AI [Leonardo.AI](asdasd)

  <details>

    > **Warning**
    > Use FVM only you installed .

    >- `fvm flutter create name_app`
    >- `fvm flutter create --platforms ios,android name_app`
  </details>

<!-- -- --- -- -- -- logo IMG -- --- -- --- --->
- [x] AI [Lexica.art](asdasd)

  <details>

    > **Warning**
    > Use FVM only you installed .

    >- `fvm flutter create name_app`
    >- `fvm flutter create --platforms ios,android name_app`
  </details>

<!-- -- --- -- -- -- logo IMG -- --- -- --- --->
- [x] AI [Chat GPT](asdasd)

  <details>

    > **Warning**
    > Use FVM only you installed .

    >- `fvm flutter create name_app`
    >- `fvm flutter create --platforms ios,android name_app`
  </details>

**App Settings 🦄** 
<!-- -- --- -- -- -- logo IMG -- --- -- --- --->
- [x] AI [Icon.kitchen](https://icon.kitchen/)

  <details>

    > **Warning**
    > Use FVM only you installed .

    >- `fvm flutter create name_app`
    >- `fvm flutter create --platforms ios,android name_app`
  </details>

<!-- -- --- -- -- -- logo IMG -- --- -- --- --->
- [x] AI [lottiefiles.com](asdasd)

  <details>

    > **Warning**
    > Use FVM only you installed .

    >- `fvm flutter create name_app`
    >- `fvm flutter create --platforms ios,android name_app`
  </details>

<!-- -- --- -- -- -- logo IMG -- --- -- --- --->
- [x] AI [Iconscout.com](asdasd)

  <details>

    > **Warning**
    > Use FVM only you installed .

    >- `fvm flutter create name_app`
    >- `fvm flutter create --platforms ios,android name_app`
  </details>


## Setting Flutter 🌱
<!-- we use your livery -->
<!-- we use your livery -->
<!-- we use your livery --> 

```dart
import 'package:shared_preferences/shared_preferences.dart';

class Preferences {
  static late SharedPreferences _prefs;

  static String _name = '';
  static bool _isDarkMode = false;
  static int _gender = 1;

  static Future init() async {
    _prefs = await SharedPreferences.getInstance();
  }

  // -- -- -- -- Name Preferences
  static String get name {
    return _prefs.getString('nick') ?? _name;
  }
  static set name(String name) {
    _name = name;
    _prefs.setString('name', name);
  }

  // -- -- -- -- isDarkMode
  static bool get darkMode {
    return _prefs.getBool('isDarkMode') ?? _isDarkMode;
  }

  static set darkMode(bool value) {
    _isDarkMode = value;
    _prefs.setBool('isDarkMode', value);
  }

  // -- -- -- -- Gender
  static int get gender {
    return _prefs.getInt('gender') ?? _gender;
  }

  static set gender(int value) {
    _gender = value;
    _prefs.setInt('gender', value);
  }
}

```