
# Install Cordova and Android SDK on Arch Linux

## 1. Install Cordova and

    npm install -g cordova
    yaourt --noconfirm gradle
  
## 1. Install JAVA and Android SDK 
```
yaourt --noconfirm jdk8-openjdk

yaourt --noconfirm android-udev
yaourt --noconfirm android-sdk
yaourt --noconfirm android-sdk-platform-tools
yaourt --noconfirm android-sdk-build-tools
```
## 2. Create global variables on system

On `~/.bashrc`
```

export ANDROID_HOME=/opt/android-sdk
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

## 3. Restart your console and you are **ready to go.**
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE0NjM4NzExNywxMTEyMTIxMTEzXX0=
-->