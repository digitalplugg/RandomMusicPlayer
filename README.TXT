Project: RandomMusicPlayer: Imported from Android Samples.
Archive for the original exists at: Oscar/Documents/AndroidStuff.

This version tested on Android Studio version 0.5.8
with the following settings:

// Top-level build file where you can add configuration options common to all sub-projects/modules.
buildscript {
    repositories {
        mavenCentral()
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:0.9.+'
    }
}

allprojects {
    repositories {
        mavenCentral()
    }
}

// App level build file configuration settings exclusive for the RandomMusicPlayer app.
apply plugin: 'android'

android {
    compileSdkVersion 19
    buildToolsVersion "19.0.1"

    defaultConfig {
        minSdkVersion 7
        targetSdkVersion 17
    }

    buildTypes {
        release {
            runProguard false
            proguardFiles getDefaultProguardFile('proguard-android.txt'), 'proguard-rules.txt'
        }
    }
}
This app demonstrates the basics for an interactive app. The app uses:

