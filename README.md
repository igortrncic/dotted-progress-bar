Dotted Progress Bar  [![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-dotted--progress--bar-green.svg?style=flat)](https://android-arsenal.com/details/1/2012)
===============

Dotted progress bar. Use custom drawable or color to configure dots.

![dotted-progress-bar](https://raw.github.com/igortrncic/dotted-progress-bar/master/progress.gif)

Gradle
------
```
dependencies {
    ...
    compile 'com.github.igortrncic.dotted-progress-bar:library:1.0.0'
}
```

Usage
-----
Use color or drawable for inactiveDot and activeDot.
```xml
<com.trncic.library.DottedProgressBar
    android:id="@+id/progress"
    android:layout_width="match_parent"
    android:layout_height="0dp"
    android:padding="30dp"
    app:activeDot="@drawable/active_dot"
    app:dotSize="29dp"
    app:inactiveDot="@drawable/inactive_dot"
    app:jumpingSpeed="670"
    app:spacing="15dp" />
```
```java
DottedProgressBar progressBar = (DottedProgressBar) findViewById(R.id.progress);
progressBar.startProgress();
progressBar.stopProgress();
```


Limitations
-----------
* layout_height is sum of paddingTop, paddingBottom and dotSize, it is irrelevant.

Changelog
---------
* **1.0.0**
    * Initial release

License
-------

    Copyright 2015 Igor Trncic

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.