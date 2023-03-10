### Mobile Automation with Appium for iOS and Android apps

## The purpose of this project was to get practical experience in mobile testing and its basic functionality

## Apps being tested ColorNote (Android) & MVCTodo (iOS)

# Tools:

1. Webdriver I/O
2. Appium
3. Android Studio
4. Xcode
5. Babel (to take advantage of late js functions)
6. Eslint plugin
7. Browser Stack (cloud testing infrastructure)
8. Appium Inspector
9. Dotenv
10. GitHub Actions (run test automatically on push command on github and browser stack)

# MacOS machine setup for Android Test

- Install Node JS
- Install Java JDK (set JAVA_HOME path)
- Install Android Studio (set ANDROID_HOME path)
- Setup Android Emulator (Pixel 3 for example)
- Install Appium Inspector
- Install Appium
- Install appium-doctor and run `appium-doctor --android`
- Install driver `appium driver install uiautomator2`

# MacOS machine setup for iOS Test (Assuming that Android setup finished successfully)

- Install Xcode from AppStore
- Install dependencies: `Xcode-select --install` and `brew install carthage`
- Install driver `appium driver install xcuitest`
- Run `appium-doctor --ios`

# Setup

- clone this repo
- run `npm install`

# To run a test (to run a specific test add --spec flag plus test file path)

1. Run iOS test suite `npm run test-ios`
2. Run android test suite `npm run test-android`
3. Run the android test suite via browser stack `npm run test-ios-bs` (have to add credentials first)
4. Run ios test suite via browser stack `npm run test-android-bs` (have to add credentials first)
