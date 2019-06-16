
# Install Cordova and Android SDK on Arch Linux

## 1. Install Cordova and

    npm install -g cordova
    yaourt --noconfirm gradle
  
## 2. Install JAVA and Android SDK 
```
yaourt --noconfirm jdk8-openjdk

yaourt --noconfirm android-udev
yaourt --noconfirm android-sdk
yaourt --noconfirm android-sdk-platform-tools
yaourt --noconfirm android-sdk-build-tools
```

## 3. Accept Android SDK Licence

    sudo chown -R <user>:<group> /opt/android-sdk

## 4. Create global variables on system

`nano ~/.bashrc`
```
export ANDROID_SDK_ROOT=/opt/android-sdk
export ANDROID_HOME=$ANDROID_SDK_ROOT
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

Apply Config
    source ~/.bashrc

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTg2Mjk4MTk4OCwxMTQ2Mzg3MTE3LDExMT
IxMjExMTNdfQ==
-->