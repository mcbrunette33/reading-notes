##Read 34

- You prepare the application for release. During the preparation step you build a release version of your application, which users can download and install on their Android-powered devices.

- You release the application to users. During the release step you publicize, sell, and distribute the release version of your application to users.

### Prepare for release

1) Configuring your application for release.
At a minimum you need to remove Log calls and remove the android:debuggable attribute from your manifest file. You should also provide values for the android:versionCode and android:versionName attributes, which are located in the <manifest> element. You may also have to configure several other settings to meet Google Play requirements or accommodate whatever method you're using to release your application.

2) If you are using Gradle build files, you can use the release build type to set your build settings for the published version of your app.

3) Building and signing a release version of your application.
You can use the Gradle build files with the release build type to build and sign a release version of your application. See Building and Running from Android Studio.

4) Testing the release version of your application.
Before you distribute your application, you should thoroughly test the release version on at least one target handset device and one target tablet device.

5) Updating application resources for release.
You need to be sure that all application resources such as multimedia files and graphics are updated and included with your application or staged on the proper production servers.

6) Preparing remote servers and services that your application depends on.
If your application depends on external servers or services, you need to be sure they are secure and production ready.

- You can release your Android applications several ways. Usually, you release applications through an application marketplace such as Google Play, but you can also release applications on your own website or by sending an application directly to a user.

- Google Play is a robust publishing platform that helps you publicize, sell, and distribute your Android applications to users around the world. When you release your applications through Google Play you have access to a suite of developer tools that let you analyze your sales, identify market trends, and control who your applications are being distributed to.

- If you do not want to release your app on a marketplace like Google Play, you can make the app available for download on your own website or server, including on a private or enterprise server. To do this, you must first prepare your application for release in the normal way. Then all you need to do is host the release-ready APK file on your website and provide a download link to users.
