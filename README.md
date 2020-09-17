# YinshiIntent
隠式启动
设置<intent-filter…/><intent-filter…/>通常包括以下几个子元素：
action:0到多个，组件支持的动作
category：0到多个，组件支持的类别
data：0个或1个，组件支持的数据。

<intent-filter>             
   <action android:name=“startAnotherActivity"/>      
   <category android:name="android.intent.category.DEFAULT"/>    
</intent-filter>

Intent intent=new Intent();
intent.setAction("anotherActivity");         
intent.addCategory("android.intent.category.DEFAULT");     
startActivity(intent);
