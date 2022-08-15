# CommandX
Useful commands for every CLI tool

- [JsonPath](#jsonpath)
- [Android](#android)
- [Cmd](#cmd)
- [Flutter](#flutter)
- [Git](#git)
- [Laravel](#laravel)
- [Ubuntu](#ubuntu)
- [Windows Run](#windows-run)
- [Intellij](#intellij)
- [MacOs](#macos)
- [Xcode](#xcode)

---
# JsonPath

## 1. Filter with string value
```bat
$.Data[?(@.Date=='2021-08-21T00:00:00')].FoodMeal[?(@.Title=='افطار')]
```

---
# Android

## 1. Check signature of APK file
```bat
keytool -printcert -jarfile app.apk
```

## 2. Check signature of AAB file
```bat
keytool -printcert -jarfile app.aab
```

## 3. Check signature of Keystore file
```bat
keytool -list -v -keystore release.jks
```

## 4. Check manifest of APK file
make sure to add `build-tools` directory to PATH first
```bat
aapt dump badging myapp.apk
```

---

# Cmd

## 1. List mapped networks
```bat
net use
```

## 2. Remove all mapped networks
```bat
net use * /d
```

## 3. Flush dns
```bat
ipconfig /flushdns
```

---

# Flutter

## 1. Run doctor
```bat
flutter doctor
```

## 2. Clean build
```bat
flutter clean
```

## 3. Get dependencies
```bat
flutter pub get
```

## 4. Run build_runner to generate codes
```bat
flutter pub run build_runner build
```

## 5. Deploy app to device
```bat
flutter run
```

## 6. Watch for changes and regenerate
```bat
flutter pub run build_runner watch
```

## 7. Run build_runner deleting conflicting outputs
```bat
flutter pub run build_runner build --delete-conflicting-outputs
```

## 8. Add flutter to path from a directory
```bat
export PATH="$HOME/Desktop/flutter/bin:$PATH"
```

## 9. Add flutter to path from root
```bat
export PATH="$PATH:`pwd`/flutter/bin"
```

## 10. Analyze release apk size for specific platform
```bat
flutter build apk --analyze-size --target-platform android-arm
```

## 11. Obfuscating release apk
```bat
flutter build apk --obfuscate --split-debug-info=C:/users/Mahdi/Desktop/symbol
```

## 12. Update pod dependencies
```bat
cd ios
pod install --repo-update
```

## 13. Identify out-of-date package dependencies
```bat
flutter pub outdated
```

## 14. Update packages to the latest version with breadking changes
```bat
flutter pub upgrade --major-versions
```

## 15. Build flavor apk
```bat
flutter build apk --flavor website --obfuscate --split-debug-info=C:\Users\Mahdi\Desktop\zireh-symbols
```
---

# Git

## 1. Untrack committed file
```bat
git rm {FileName} --cache
```

## 2. Reorder commits
```bat
git rebase -i HEAD~3
```

## 3. Revert changes made to your working copy
```bat
git checkout .
```

## 4. Revert changes made to the index (i.e., that you have added), do this. 
Warning this will reset all of your unpushed commits to master!
```bat
git reset
```

## 5. Revert a change that you have committed
```bat
git revert <commit 1> <commit 2>
```

## 6. Remove untracked files (e.g., new files, generated files)
```bat
git clean -f
```

## 7. Remove untracked directories (e.g., new or automatically generated directories)
```bat
git clean -fd
```

## 8. Prune remote
```bat
git remote prune origin
```

## 9. Get rid of LF or CRLF empty changes
```bat
git add --renormalize .
```

---

# Laravel

## 1. Rollback last migration
```bat
php artisan migrate:rollback --step=1
```

## 2. Apply changes to .env
```bat
php artisan config:cache

php artisan config:clear
```

## 3. Deploy checklist
```bat
php artisan down

git pull

composer i

npm i

npm run prod

php artisan migrate

php artisan permission:sync

php artisan config:cache

php artisan view:cache

php artisan route:cache

php artisan up
```

## 4. Install composer dependencies ignoring php version difference
```bat
composer install --ignore-platform-reqs
```

## 5. Link storage to public
```bat
php artisan storage:link
```

---

# Ubuntu

## 1. Zip a direcory
```bat
tar -zcvf archive.tar.gz directory/
```

## 2. Open root directory
```bat
cd /home/lighttpd/http
```

## 3. Move file to directory
```bat
mv [file] [directory]
```

## 4. Delete file
```bat
rm [file]
```

## 5. Open dns record file
```bat
nano /etc/bind/db.{domain}.com
```

## 6. Show hidden files
```bat
ls -ad .*
```

## 7. Download file
```bat
wget http://link.to.file
```

## 8. Extract tar.gz
```bat
tar xvzf file.tar.gz
```

## 9. Copy file to direcory
```bat
cp -a file direcory
```

---

# Windows Run

## 1. Open network adapters
```bat
ncpa.cpl
```

---

# Intellij

## 1. Show diagram
```bat
CTRL + ALT + SHIFT + U 
```

## 2. Reformat code
```bat
Ctrl + Alt + L
```

## 3. Refactor or rename target
```bat
Shift + F6
```

## 4. Jump to next/previous context
```bat
Ctrl + Shift + LeftArrow
Ctrl + Shift + RightArrow
```

## 5. Open preferences screen
```bat
Ctrl + Alt + S
```

## 6. Recent locations preview
```bat
Ctrl + Shift + E
```

## 7. Go to declaration (without left click + Ctrl)
```bat
Ctrl + B
```

## 8. Show definition with body
```bat
Ctrl + Shift + i
```

## 9. Search Everywhere
Quickly find any file, action, symbol, tool window, or setting in IntelliJ IDEA, in your project, and in the current Git repository.
```bat
Double Shift
```

## 10. Add/remove line or block comment
```bat
Ctrl + /
```

## 11. Comment out a line or block of code.
```bat
Ctrl + Shift + /
```

## 12. View recent files
```bat
Ctrl + E
```

## 13. Complete Current Statement
Complete Current Statement
Insert any necessary trailing symbols and put the caret where you can start typing the next statement.
```bat
Ctrl + Shift + Enter
```
---

# MacOs

## 1. Take screenshot
```bat
Command + Shift + 4
```

## 2. Open spotlight
```bat
Command + Space
```

## 3. Show/hide hidden files and folders
```bat
Command + Shift + .
```

---

# Xcode

## 1. Show/Hide active pane
```bat
Command + Shift + Y
```
