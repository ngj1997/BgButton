# BgButton
圆角按键

[![](https://jitpack.io/v/cc0819/BgButton.svg)](https://jitpack.io/#cc0819/BgButton)

![image](https://github.com/cc0819/BgButton/blob/master/art/gitshow.gif)

V1.2.0
增加了可以控制点击后的背景、文字、框颜色的设置




Gradle

  	repositories { 
   		 maven { url "https://jitpack.io" }
	} 
  
	dependencies {
	        compile 'com.github.cc0819:BgButton:1.2.0'
	}
 


Usage

属性

    <declare-styleable name="BgButton">
        <!--背景颜色-->
        <attr name="bgColor" format="color|reference"/>
        <!--边框颜色-->
        <attr name="cornerRadiusColor" format="color"/>
        <!-- 边框厚度 -->
        <attr name="borderWidth" format="dimension"/>
        <!--圆角半径-->
        <attr name="cornerRadius" format="dimension" />
        <attr name="topLeftRadius" format="dimension"></attr>
        <attr name="topRightRadius" format="dimension"></attr>
        <attr name="bottomLeftRadius" format="dimension"></attr>
        <attr name="bottomRightRadius" format="dimension"></attr>
        <!--形状-->
        <attr name="shapeType" format="enum">
            <enum name="rectangle" value="0"></enum>
            <enum name="oval" value="1"></enum>
        </attr>
        <!-- 虚线长度 -->
        <attr name="borderDashLength" format="dimension"/>
        <!-- 虚线间隙小点长度 -->
        <attr name="borderDashGapSmall" format="dimension"/>
        <!-- 虚线间隙 -->
        <attr name="borderDashGap" format="dimension"/>

        <!-- 点击状态 -->
         <attr name="isChick" format="boolean"/>

         <!--点击后背景颜色-->
         <attr name="clickedBgColor" format="color"/>
         <!--点击后边框颜色-->
         <attr name="clickedCornerRadiusColor" format="color"/>
         <!--点击后字体颜色-->
          <attr name="clickedTextColor" format="color"/>



    </declare-styleable>


    
XML

    <com.cheng.cc.library.BgButton
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center_horizontal"
        android:layout_marginTop="10dp"
        android:padding="10dp"
        android:text="哈哈哈哈哈"
        android:textColor="#f21"
        app:bgColor="@color/colorPrimaryDark"
        app:cornerRadius="5dp"
        app:borderWidth="2dp"
        app:cornerRadiusColor="@color/colorAccent"
        />


     <com.cheng.cc.library.BgButton
           android:layout_width="wrap_content"
           android:layout_height="wrap_content"
           android:layout_gravity="center_horizontal"
           android:layout_marginTop="10dp"
           android:padding="10dp"
           android:text="哈哈哈哈哈"
           android:textColor="#f21"
           app:bgColor="@color/colorPrimaryDark"
           app:cornerRadius="5dp"
           app:borderWidth="2dp"
           app:cornerRadiusColor="@color/colorAccent"

           app:clickedBgColor="@color/green"
           app:clickedCornerRadiusColor="@color/yellow"
           app:clickedTextColor="@color/purple"
           />


    <com.cheng.cc.library.BgButton
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center_horizontal"
        android:layout_marginTop="10dp"
        android:padding="10dp"
        android:text="哈哈哈哈哈"
        android:textColor="#f21"
        app:borderWidth="1dp"
        app:cornerRadiusColor="@color/colorAccent"
        app:shapeType="oval"/>



