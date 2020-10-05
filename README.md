一：线性布局

代码：

```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
android:layout_width="match_parent"
android:layout_height="match_parent"
android:orientation="vertical" >

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
            <Button
                android:id="@+id/btnSunInvisbile"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="@string/one_one" />

            <Button
                android:id="@+id/btnSunGone"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="@string/one_two" />

            <Button
                android:id="@+id/btnSunVisible"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="@string/one_three" />

            <Button
                android:id="@+id/btnSunToFlower"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="@string/one_four" />
        </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:id="@+id/btnSunInvisbile1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/two_one" />

        <Button
            android:id="@+id/btnSunGone1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/two_two" />

        <Button
            android:id="@+id/btnSunVisible1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/two_three" />

        <Button
            android:id="@+id/btnSunToFlower1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/two_four" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:id="@+id/btnSunInvisbile2"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="three_one" />

        <Button
            android:id="@+id/btnSunGone2"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="three_two" />

        <Button
            android:id="@+id/btnSunVisible2"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="three_three" />

        <Button
            android:id="@+id/btnSunToFlower2"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="three_four" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:id="@+id/btnSunInvisbile3"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="four_one" />

        <Button
            android:id="@+id/btnSunGone3"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="four_two" />

        <Button
            android:id="@+id/btnSunVisible3"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="four_three" />

        <Button
            android:id="@+id/btnSunToFlower3"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="four_four" />
    </LinearLayout>
    </LinearLayout>
```

实验截图：

![QQ截图20201006004208](C:\Users\ASUS\Desktop\图片\QQ截图20201006004208.png)

二：约束布局

代码：

```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TextView
        android:id="@+id/textView4"
        android:layout_width="60dp"
        android:layout_height="40dp"
        android:background="#F80707"
        android:gravity="center"
        android:text="red"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView5"

        android:layout_width="60dp"
        android:layout_height="40dp"

        android:background="#FF9800"
        android:gravity="center"
        android:text="orange"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.0" />

    <TextView
        android:id="@+id/textView6"
        android:layout_width="60dp"
        android:layout_height="40dp"
        android:background="#FFEB3B"
        android:gravity="center"
        android:text="yellow"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView7"
        android:layout_width="60dp"
        android:layout_height="40dp"
        android:layout_marginTop="280dp"
        android:background="#2196F3"
        android:gravity="center"
        android:text="blue"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView8"
        android:layout_width="60dp"
        android:layout_height="40dp"
        android:layout_marginStart="60dp"
        android:layout_marginTop="280dp"
        android:background="#85F107"
        android:gravity="center"
        android:text="green"
        app:layout_constraintEnd_toStartOf="@+id/textView7"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView9"
        android:layout_width="60dp"
        android:layout_height="40dp"
        android:layout_marginTop="280dp"
        android:layout_marginEnd="60dp"
        android:background="#673AB7"
        android:gravity="center"
        android:text="indgio"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@+id/textView7"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView10"
        android:layout_width="410dp"
        android:layout_height="40dp"
        android:background="#D806FB"
        android:gravity="center"
        android:text="violet"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="1.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView7"
        app:layout_constraintVertical_bias="0.522" />

</androidx.constraintlayout.widget.ConstraintLayout>

```

实验截图：

![QQ截图20201006004255](C:\Users\ASUS\Desktop\图片\QQ截图20201006004255.png)



三：表格布局

代码：

```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
<TableLayout
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:shrinkColumns="0">
    <Button
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:text="open...                                                               ctrl+o"
        android:gravity="left"

        >

    </Button>
    <Button
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:text="save...                                                               ctrl+s"
        android:gravity="left"
        android:layout_marginTop="-11dp"
        >

    </Button>
    <Button
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:text="save As...                                                       ctrl+shift+s"
        android:gravity="left"
        android:layout_marginTop="-11dp"
        >

    </Button>
    <View  android:layout_height="2px"
        android:layout_width="match_parent"
        android:background="#000000"
        android:layout_marginTop="-3dp"
></View>
    <Button
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:text="Import..."
        android:gravity="left"
        android:layout_marginTop="-4dp"
        >
    </Button>
    <Button
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:text="Export...                                                              ctrl+e"
        android:gravity="left"
        android:layout_marginTop="-11dp"
        >
    </Button>
    <View  android:layout_height="2px"
        android:layout_width="match_parent"
        android:background="#000000"
        android:layout_marginTop="-3dp"
        ></View>
    <Button
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:text="quilt..."
        android:gravity="left"
        android:layout_marginTop="-4dp"
        >
    </Button>
</TableLayout>
</LinearLayout>

```

实验截图：

![QQ截图20201006005300](C:\Users\ASUS\Desktop\图片\QQ截图20201006005300.png)

