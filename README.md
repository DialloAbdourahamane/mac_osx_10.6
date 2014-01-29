mac_osx_10.6
============
If you get the "check dependencies error: There is no SDK with 
the name or path '/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX10.6.sdk'" 
error, the following steps should help:

Download the MacOSX 10.6 SDK
Extract the zip file
Put the resulting folder in /Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/
Then fix the Build Settings for yourProject.xcodeproj and the openFrameworksLib.xcodeproj to have the Base SDK pointing at 10.6
Restart XCode and compile again
Now it should work!

