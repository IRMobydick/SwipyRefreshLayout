SwipyRefreshLayout
================

A SwipeRefreshLayout extension that allows to swipe in both direction (API 9+)

To include in your project, add this to your build.gradle file:
```
   //SwipyRefreshLayout
   compile 'com.github.orangegangsters:swipy:1.0.0@aar'
```

![Demo](app/src/main/res/raw/github_gif.gif)

========

### Usage

If you want an example on how to use it, you can find an example app in this repo.

```
<com.orangegangsters.github.swipyrefreshlayout.library.SwipyRefreshLayout
        android:id="@+id/swipyrefreshlayout"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:direction="bottom">

        <ListView
            android:id="@+id/listview"
            android:layout_width="match_parent"
            android:layout_height="match_parent" />

</com.orangegangsters.github.swipyrefreshlayout.library.SwipyRefreshLayout>
```

```
mSwipyRefreshLayout.setOnRefreshListener(new SwipyRefreshLayout.OnRefreshListener() {
            @Override
            public void onRefresh() {

            }
});
```

========

### Customization

* XML:
```
app:direction="top"
```
OR
```
app:direction="bottom"
```

* Programmatically:
```
mSwipyRefreshLayout.setDirection(SwipyRefreshLayoutDirection.TOP);
```
OR
```
mSwipyRefreshLayout.setDirection(SwipyRefreshLayoutDirection.BOTTON);
```

========

### TODO

* Handle both direction at the same time (doesn't work yet)

========

### Credits

### By Developers:
[Olivier Goutay](https://github.com/olivierg13) and [Stoyan Dimitrov](https://github.com/StoyanD)


========

### License

```
The MIT License (MIT)

Copyright (c) 2015 OrangeGangsters

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