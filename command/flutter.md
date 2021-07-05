# Flutter

## clean build
```bat
flutter clean
```

## get dependencies
```bat
flutter pub get
```

## run build_runner to generate codes
```bat
flutter pub run build_runner build
```

## deploy app to device
```bat
flutter run
```

## watch for changes and regenerate
```bat
flutter pub run build_runner watch
```

## run build_runner deleting conflicting outputs
```bat
flutter pub run build_runner build --delete-conflicting-outputs
```

## add flutter to path from a directory
```bat
export PATH="$HOME/Desktop/flutter/bin:$PATH"
```

## add flutter to path from root
```bat
export PATH="$PATH:`pwd`/flutter/bin"
```

## run doctor
```bat
flutter doctor
```

## analyze release apk size for specific platform
```bat
flutter build apk --analyze-size --target-platform android-arm
```

## obfuscating release apk
```bat
flutter build apk --obfuscate --split-debug-info=C:/users/Mahdi/Desktop/symbol
```