![banner](https://raw.githubusercontent.com/sungbin5304/TagableRoundImageView/master/banner.png)

-----

# Download [![version](https://jitpack.io/v/sungbin5304/TagableRoundImageView.svg)](https://jitpack.io/#sungbin5304/TagableRoundImageView)

```Gradle
repositories {
  mavenCentral()
  google()
  maven { 
    url 'https://jitpack.io' 
  }
}

dependencies {
  implementation 'com.github.sungbin5304:TagableRoundImageView:{version}'
}
```

# Usage
## xml
```xml
<com.sungbin.tagable.roundimageview.library.TagableRoundImageView
        android:id="@+id/image"
        android:layout_width="200dp"
        android:layout_height="200dp"
        android:src="@drawable/doraemon"
        app:triv_imageRadius="16dp"
        app:triv_tagText="gif"
        app:triv_tagPadding="8dp"
        app:triv_tagGravity="end|bottom" />
```

## All attribute
| Attribute | Description| Default |
| ------------- | ------------- | ------------- |
| `triv_tagGravity` | Set tag gravity (`top`, `bottom`, `left`, `right`, `start`, `end`) | `Gravity.END` and `Gravity.BOTTOM` |
| `triv_tagTextStyle` | Set tag text style (`italic`, `normal`) | `NORMAL` |
| `triv_imageRadius` | Set imageview radius | `16dp` |
| `triv_tagRadius` | Set tag layout radius | `2dp` |
| `triv_tagPadding` | Set tag layout padding | `8dp` |
| `triv_tagTextSize` | Set tag text size| `15dp` |
| `triv_tagText` | Set tag text | No value |
| `triv_tagBackgroundColor` | Set tag layout background color | `Color.WHITE` |

## All methods
```kotlin
- set(text: String, tagBackgroundColor: Int = Color.WHITE,
      tagTextSize: Int = 15dp, tagTextPadding: Int = 8dp,
      tagTextStyle: Int = Typeface.NORMAL, tagRadius: Int = 2dp,
      imageRadius: Int = 16dp)
```

# License
```
                  Copyright 2020 SungBin

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```
