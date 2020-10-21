![banner](https://raw.githubusercontent.com/sungbin5304/TagableRoundImageView/master/banner.png)

-----

# Download
You can download at [this](https://github.com/sungbin5304/AndroidUtils/blob/master/README.md#tagableroundimageview-more-guide) page.

# Usage
## xml
```xml
<com.sungbin.androidutils.ui.TagableRoundImageView
        android:id="@+id/image"
        android:layout_width="200dp"
        android:layout_height="200dp"
        android:src="@drawable/doraemon"
        app:triv_imageRadius="16dp"
        app:triv_tagText="gif"
        app:triv_tagPadding="8dp"
        app:triv_tagGravity="end|bottom" />
```

## all attribute
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

## method
```kotlin
set(text: String, tagBackgroundColor: Int = Color.WHITE,
      tagTextSize: Int = 15dp, tagTextPadding: Int = 8dp,
      tagTextStyle: Int = Typeface.NORMAL, tagRadius: Int = 2dp,
      imageRadius: Int = 16dp)
      
updateRadius(imageRadius: Int)
```

## tip
1. `TagableRoundImageView` is supported GIF images.<br>
You can set GIF image from [Glide](https://github.com/bumptech/glide) library.

2. If you not set `triv_tagText` parameter, `TagableRoundImageView` will be only rounding image.

#### `TagableRoundImageView` is based on [`Android-BadgedImageView`](https://github.com/klinker24/Android-BadgedImageView).

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
