# Watch Face Format Boilerplate Project
This is a mostly-empty template for [Google-Samsung Watch Face Format (WFF)](https://developer.android.com/training/wearables/wff) projects. You can use it as a basis for new WFF projects.

## Usage

The files in this project should build and install as is. However, this will give you a watch face called 'Boilerplate'. Customise the project as follows:

* project directory name ('boilerplate'): change

* `watchface\build.gradle.kts`: change `namespace` and `applicationId`

* `settings.gradle.kts`: change `rootProject.name`

* `watchface\src\main\res\values\strings.xml`: change `watch_face_name`

* `watchface\src\main\res\raw\watchface.xml`: remove the `<PartDraw>` (which is only present to verify that the boilerplate project runs).

* `watchface\src\main\res\drawable\preview.png`: replace with a screenshot of your completed watch face.

You can now add your own WFF XML elements, resources and other customisation.

## Issues

When you first build your project, you'll probably get 'Invalid Gradle JDK configuration found', because this repository does not contain `.gradle` files. Gradle can usually configure itself after this if you've got a suitable build environment installed (such as *Android Studio*). Alternatively, you can try copying and adapting `.gradle` files from [here](https://github.com/android/wear-os-samples/tree/main/WatchFaceFormat).

Gradle is updated regularly, so you may need to upgrade your project accordingly.

## Acknowledgement

This repository is based on [Google's Watch Face Format Sample repository](https://github.com/android/wear-os-samples/tree/main/WatchFaceFormat).

## Links

[Google's Watch Face Format site](https://developer.android.com/training/wearables/wff): brief(!!) instructions on WFF project setup and building; WFF XML reference.

[Samsung Watch Face Studio:](https://developer.samsung.com/watch-face-studio/overview.html) the easiest way to design WFF watchfaces, but is less flexible than WFF XML.

[Watch Face Format Sample:](https://github.com/android/wear-os-samples/tree/main/WatchFaceFormat) Google samples demonstrating the structure of WFF watch faces.

[XML Preprocessor:](https://github.com/gondwanasoft/xml-preprocessor) a tool that can help with WFF XML development.