# flutter
flutter setup and running.

Go throught the flutter docs

download flutter_windows_1.22.1-stable.zip
unzip this file a flutter folder will be generated.
create a folder naming src and copy this flutter folder in  c: other than program folder
example C:\Users\abhigang\src
Next step is to upadate your path.
The document says 
From the Start search bar, enter ‘env’ and select Edit environment variables for your account.
Under User variables check if there is an entry called Path:
If the entry exists, append the full path to flutter\bin using ; as a separator from existing values.
If the entry doesn’t exist, create a new user variable named Path with the full path to flutter\bin as its value.
BUT THIS DID NOT work for me 
add the same path in system variable just below the User variable BOX.
add the path till flutter\bin 
C:\Users\abhigang\src\flutter\bin
INSTALL Andriod studio add flutter plugin to it using setting -> plugin -> search flutter
It will also add dart plugin.

check for flutter doctor command in CMD
==========================================
C:\Users\abhigang>flutter doctor
Doctor summary (to see all details, run flutter doctor -v):
[√] Flutter (Channel stable, 1.22.1, on Microsoft Windows [Version 10.0.18363.1139], locale en-US)

[!] Android toolchain - develop for Android devices (Android SDK version 30.0.2)
    X Android license status unknown.
      Run `flutter doctor --android-licenses` to accept the SDK licenses.
      See https://flutter.dev/docs/get-started/install/windows#android-setup for more details.
[!] Android Studio
    X Flutter plugin not installed; this adds Flutter specific functionality.
    X Dart plugin not installed; this adds Dart specific functionality.
    X android-studio-dir = C:\Program
    X Android Studio not found at C:\Program
[√] VS Code (version 1.50.0)
[!] Connected device
    ! No devices available

! Doctor found issues in 3 categories.
================================================================
X android-studio-dir = C:\Program 
X Android Studio not found at C:\Program
The above error can be mitigate using the 
flutter config --android-studio-dir="C:\Program Files\Android\Android Studio"
SEE the "" in the path
use flutter doctor -v more vorbose output

==================================================================

This error

[!] Android toolchain - develop for Android devices (Android SDK version 30.0.2)
    X Android license status unknown.
      Run `flutter doctor --android-licenses` to accept the SDK licenses.
      See https://flutter.dev/docs/get-started/install/windows#android-setup for more details.

can be mitigate using 
flutter doctor --android-licenses
and press y multiple time
Plugin erros can be ignored.

=====================================================================
[!] Connected device
    ! No devices available
This error will also go once u add a device in andriod studio from tools -> ADV Manager -> select any device.

then run the tutorial app.


    


