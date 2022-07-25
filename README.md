# Android Kotlin WebView Boilerplate

## Using a remote Source

If you want to create an app that simply displays the contents of a remote website

Uncomment **line 23** in `MainActivity.kt` and change `https://www.dincerdegre.com/` to match your remote source

    ```
	webView.loadUrl("https://www.dincerdegre.com/")
	```

## Refactor to Package Name

Project panel, click on the little **gear** icon, Uncheck the **Compact Empty Middle Packages** option, Your package directory will now be broken up into individual directories. Individually select each directory you want to rename and:

* Right-click it

* Select Refactor

* Click on Rename

* In the pop-up dialog, click on Rename Package instead of Rename Directory

* Enter the new name and hit Refactor

* Click Do Refactor in the bottom

* Allow a minute to let Android Studio update all changes

Note: When renaming com in Android Studio, it might give a warning. In such case, select Rename All

Now open your Gradle Build File (build.gradle - Usually app or mobile). Update the applicationId in the defaultConfig to your new Package Name and Sync Gradle, if it hasn't already been updated automatically:

* You may need to change the package= attribute in your manifest.

* Clean and Rebuild.

* This should help you with your doubt. 