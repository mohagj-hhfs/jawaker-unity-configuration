# Android Setup

## Android SDK

In order to be able to build APKs from our project, we need to have the android sdk installed:
```bash
brew cask install android-sdk
brew cask info android-sdk # You will see the path in which the sdk is installed (copy it)
```

Then we'll have to link to our ~/.bash_profile, open it and paste the following code:
```bash
export ANDROID_HOME=/usr/local/Caskroom/android-sdk/3859397 # Here paste the path you got from the previous step
export PATH=$ANDROID_HOME/tools:$PATH
export PATH=$ANDROID_HOME/platform-tools:$PATH
```

Then we have to install the API level 28 build tools
```bash
yes | sdkmanager "build-tools;28.0.3" "extras;android;m2repository" "extras;google;google_play_services" "extras;google;m2repository" "platforms;android-28" "platform-tools"
```

## SDKMAN
SDKMAN is a package manager for alot of sdks, and we'll use it to install a couple of tools we need

```bash
curl -s "https://get.sdkman.io" | bash # Follow the instruction it will give you
source "$HOME/.sdkman/bin/sdkman-init.sh"
```

## Gradle
Gradle is the tool used to actually build our android project to an apk
```bash
sdk install gradle 4.6
```

## JDK
We need the jdk(java development kit) as well
```bash
sdk install java 8.0.242.j9-adpt
```

## Android NDK
Android NDK is required if we want to build our android apk using IL2CPP instead of mono(which we have to use when uploading to GooglePlay as we need 64-bit support).
Download the ndk from [here](https://developer.android.com/ndk/downloads/older_releases) and be sure to install the 16rb version

- If you have to build using IL2CPP on MacOS Catalina, it will fail because the 16rb version is not signed, follow the instructions [here](https://www.imore.com/how-open-apps-anywhere-macos-catalina-and-mojave) to overcome this
