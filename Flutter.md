# Flutter
### Flutter Doctor
To know your flutter SDK is set up correctly and compatible with platforms, devices and IDE, type this flutter cli command, it gives you a brief description of tools and devices required for flutter development and then you can configure you flutter project.
    flutter doctor
To know more about these in details type 
    flutter doctor -v
### Flutter Upgrade
To download and update your flutter SDK current branch. You have to upgrade for each flutter channel, if you switch the channel. Run this flutter command
    flutter upgrade
### Flutter Packages Get
This flutter cli command downloads and includes the package used in the flutter project. If the package is already downloaded, it will use offline package stored in flutter SDK.
    flutter packages get
### Create a new project in Flutter
Suppose you want to create flutter project name my_flutter_commands_app , by default flutter create projects to support Android and iOS platform. You can add other platforms also more is given about this in topics below then the flutter command would be:
    flutter create my_flutter_commands_app
### New flutter project with custom package name
Suppose you want to make the package name com.navoki.my_flutter_commands_app , where navoki.com is your organization’s web address. You have to use --org parameter, then cli command would be:
    flutter create --org=com.navoki  my_flutter_commands_app
### Flutter project with different app name and folder name
While creating a new project, you can set specific <app-name> that will appear in flutter package name and in applicationID, while the folder name can be different. You have to use --project-name parameter
    flutter create --org=com.navoki --project-name=navoki my_flutter_commands_app
### Flutter project with platform-specific native language
The native platform Android supports two languages Java and Kotlin (default). The native platform for iOS supports two languages Objective C and Swift (default). If you don’t specify any language, then default languages are selected codes will be generated

Select native language in Android platform use parameter
    flutter create --org=com.navoki --android-language=java my_flutter_commands_app