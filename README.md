# MaterialLoadingProgressBar

MaterialLoadingProgressBar provide a styled ProgressBar which looks  like SwipeRefreshLayout's loading indicator(support-v4  v21+)

![ProgressBar](https://github.com/lsjwzh/MaterialLoadingProgressBar/blob/master/screen.gif)
## Usage

### xml:

```
<com.runtai.materialloadingprogressbar.materialloadingprogressbar.CircleProgressBar
        android:id="@+id/progressBar"
        android:layout_width="60dp"
        android:layout_height="60dp"/>
```
### options:

```
<com.runtai.materialloadingprogressbar.materialloadingprogressbar.CircleProgressBar
        android:id="@+id/progressBar"

        app:mlpb_show_arrow="true"
        app:mlpb_arrow_height="5dp"
        app:mlpb_arrow_width="10dp"
        app:mlpb_enable_circle_background="true"

        app:mlpb_progress_stoke_width="5dp"
        app:mlpb_progress_text_visibility="visible"
        android:layout_width="60dp"
        android:layout_height="60dp"/>
```

### java api:
#### show arrow
'CircleProgressBar' will not show arrow by default.
You can enable arrow drawing like this:
```
    circleProgressBar.setShowArrow(true);
```

#### Disable circle background
There is a white circle background on drawing 'CircleProgressBar' by default.
If you need hide the circle background,you can add a xml item

```
    app:mlpb_enable_circle_background="false"
```

or set it by java code
```
   circleProgressBar.setCircleBackgroundEnabled(false);
```