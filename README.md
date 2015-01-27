picsy
=====
Picsy is a lightweight photo capture library that simplifies capturing 1:1 aspect ratio photos. Features include:
- Customisable UI that captures photos and manages various camera features
- Captured photos are cropped and resizes to a 1:1 aspect ratio
- Toggle flash modes
- Auto focus
- Grid overlay

How to use
=====
To include the library in your main project, clone it in of your project's directories then within your `settings.gradle` add the following line:

    include ':DIRWHEREPICSYISCLONED:picsy:memtrip-picsy'

You will also want to add it to your `build.gradle` under the dependencies section like so:

	dependencies {
	    ...
		compile project(':DIRWHEREPICSYISCLONED:picsy:memtrip-picsy')
	}

Depending on which components of the library you're using you may need to add the following features and permissions to your AndroidManifest.xml

    <uses-permission android:name="android.permission.CAMERA" />
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
    <uses-feature android:name="android.hardware.camera" />
    <uses-feature android:name="android.hardware.camera.autofocus" />

Please note, not all features of this lib need access to those permissions & features so include only if necessary.


