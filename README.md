# PickTime
原项目地址：https://github.com/codbking/PickTime

由于原作者一直没有更新修复该项目,因此鄙人不才打算接替维护这个项目

更新项目地址：https://github.com/geekxingyun/PickTime

V1.0.2 更新说明: 原项目地址不支持只显示年月,这个仓库添加了年月的显示

## 日期选择控件 ##

[![](https://jitpack.io/v/codbking/PickTime.svg)](https://jitpack.io/#codbking/PickTime)

 [**apk下载**](https://raw.githubusercontent.com/codbking/PickTime/master/app-debug.apk)

### 截图
------------------

|TYPE_ALL|TYPE_YMDHM|TYPE_YMDH|TYPE_YMD|TYPE_HM|
|:--:|:--:|:--:|:--:|:--:|
|![Alt text](image/all.jpg)|![Alt text](image/ymdhm.jpg)|![Alt text](image/ymdh.jpg)|![Alt text](image/ymd.jpg)|![Alt text](image/hm.jpg)|
<!--<img src="image/all.jpg" height="320" width="180" style="margin-left:100"/>-->
<!--<img src="image/ymdhm.jpg" height="320" width="180" style="margin-left:100"/>-->
<!--<img src="image/ymdh.jpg" height="320" width="180" style="margin-left:100"/>-->
<!--<img src="image/ymd.jpg" height="320" width="180" style="margin-left:100"/>-->
<!--<img src="image/hm.jpg" height="320" width="180" style="margin-left:100"/>-->

### DateType

- TYPE_ALL--年、月、日、星期、时、分
- TYPE_YMDHM--年、月、日、时、分
- TYPE_YMDH--年、月、日、时
- TYPE_YMD--年、月、日
- TYPE_HM--时、分
- TYPE_YM--年、月

### how to use

 - **Add it in your root build.gradle at the end of repositories:**

```
	    allprojects {
		   repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	    }
```

 -  **Add the dependency**
```sh
	dependencies {
	        implementation 'com.github.geekxingyun:PickTime:v1.0.2'
	}
```

 -  **java**
```java
        DatePickDialog dialog = new DatePickDialog(this);
        //设置上下年分限制
        dialog.setYearLimt(5);
        //设置标题
        dialog.setTitle("选择时间");
        //设置类型
        dialog.setType(DateType.TYPE_ALL);
        //设置消息体的显示格式，日期格式
        dialog.setMessageFormat("yyyy-MM-dd HH:mm");
        //设置选择回调
        dialog.setOnChangeLisener(null);
        //设置点击确定按钮回调
        dialog.setOnSureLisener(null);
        dialog.show();
```




