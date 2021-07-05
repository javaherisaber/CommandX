# Android

## Check signature of APK file
```bat
keytool -printcert -jarfile app.apk
```

## Check signature of AAB file
```bat
keytool -printcert -jarfile app.aab
```

## Check signature of Keystore file
```bat
keytool -list -v -keystore release.jks
```