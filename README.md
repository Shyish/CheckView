# Check View [![](https://jitpack.io/v/Shyish/CheckView.svg)](https://jitpack.io/#Shyish/CheckView) [![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-CheckView-green.svg?style=true)](https://android-arsenal.com/details/1/3968) <a href="http://www.methodscount.com/?lib=com.github.Shyish%3ACheckView%3A%2B"><img src="https://img.shields.io/badge/Methods and size-102 | 10 KB-e91e63.svg"/></a>


![Sample](https://github.com/Shyish/CheckView/blob/master/gifs/checkview.gif?raw=true)

## Usage
   
Add a CheckView to your layout
```xml
    <com.zdvdev.checkview.CheckView
        android:id="@+id/checkView"
        android:layout_width="48dp"
        android:layout_height="48dp"
        app:cvlineColor="#ff00" />
```

// Note that you can define the color with `lineColor`

Toggle is done **automatically by default**, if you want to change that, just:

```java
    checkView.setAutoToggle(false);
```

or by xml:

```xml
    app:cvautoToggle="false"
```

You can also set a state directly:
```java
    checkView.plus();
```
```java
    checkView.check();
```

## Extra

Optionally supply an animation duration in milliseconds:

```java
    checkView.check(0L);
```

```java
    checkView.toggle(150L);
```

```java
    checkView.plus(200L);
```

Or pass a custom stroke width:

```xml
    app:cvstrokeWidth="8dp"
```

## Download

Easy as:

```gradle
repositories {
    maven { url "https://jitpack.io" }
}

dependencies {
    compile 'com.github.Shyish:CheckView:1.X.X'
}
```

## Based on

[CrossView from Collin Flynn (cdflynn)](https://github.com/cdflynn/crossview)
