![banner](https://raw.githubusercontent.com/sungbin5304/TagableRoundImageView/master/banner.png)

-----

# Download
You can download at [this](https://github.com/sungbin5304/AndroidUtils/blob/master/README.md#ui) page.

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
MIT License

Copyright (c) 2020~2021 Sungbin Ji and Luke Klinker

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
