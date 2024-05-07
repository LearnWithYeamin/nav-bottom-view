<p align="center">
<p align="center">
  <a href="https://github.com/i-rin-eam">
    <img src="https://avatars.githubusercontent.com/u/154800878?s=400&u=5d18880cc28646190a19a971bfcdbc54644eab07&v=4" alt="Logo" width="100" height="100">
  </a> 
<h1 align='center'>Navigation Drawer + BottomNaviagtionView</h1>
<h3 align='center'>
   Visit my youtube channel <a href="https://www.youtube.com/@LearnWithYeamin">Learn With Yeamin</a>
</h3>
</p>

## Step 1: Here is `activity_main.xml` code.
```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.drawerlayout.widget.DrawerLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/drawerLayout"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#FFFFFF"
    android:fitsSystemWindows="true"
    tools:context=".MainActivity"
    tools:openDrawer="end">

    <androidx.coordinatorlayout.widget.CoordinatorLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent">

        <com.google.android.material.appbar.AppBarLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">

            <com.google.android.material.appbar.MaterialToolbar
                android:id="@+id/materialToolbar"
                android:layout_width="match_parent"
                android:layout_height="?attr/actionBarSize"
                android:background="#FF5722"
                android:theme="@style/ThemeOverlay.MaterialComponents.Toolbar.Primary"
                app:navigationIcon="@drawable/ic_navigation"
                app:title="@string/app_name"
                app:titleTextColor="#FFFFFF">

            </com.google.android.material.appbar.MaterialToolbar>
        </com.google.android.material.appbar.AppBarLayout>

        <RelativeLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_marginTop="?attr/actionBarSize">

            <FrameLayout
                android:id="@+id/frameLayout"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:layout_above="@id/bottom_navigation"
                android:layout_alignParentTop="true" />


            <com.google.android.material.bottomnavigation.BottomNavigationView
                android:id="@+id/bottom_navigation"
                style="@style/Widget.MaterialComponents.BottomNavigationView"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_alignParentBottom="true"
                app:itemIconTint="#00BCD4"
                app:itemTextColor="#03A9F4"
                app:labelVisibilityMode="labeled"
                app:menu="@menu/bottom_navigation_menu" />


        </RelativeLayout>


    </androidx.coordinatorlayout.widget.CoordinatorLayout>

    <com.google.android.material.navigation.NavigationView
        android:id="@+id/navigationView"
        android:layout_width="wrap_content"
        android:layout_height="match_parent"
        android:layout_gravity="start"
        android:background="#FFFFFF"
        app:headerLayout="@layout/nav_header"
        app:itemIconTint="#00BCD4"
        app:itemTextColor="#03A9F4"
        app:menu="@menu/nav_menu" />

</androidx.drawerlayout.widget.DrawerLayout>
```
## Authors

**MD YEAMIN** - Android Software Developer <a href="https://www.youtube.com/@LearnWithYeamin">**(Learn With Yeamin)**</a> 

<h1 align="center">Thank You ❤️</h1>
