# DragLlistView 
<br/>
可以拖动排序的ListView ，同时支持侧滑 ，基于“yuyidong”的开源项目的修改，主要优化了适配器数据更新方式、自定用于滑动时
跟随手指移动阴影图像、以及当ListView中ItemView 大小不一致时，将一个小点的视图放置到较大视图上时的闪烁问题。
<br/>
![](https://github.com/zhangguoning/DragLlistView/raw/master/wwwwww.gif)
<br/>
一个封装好的图片选择器模块，可以使用多选模式和单选模式两种，单选模式调用系统的图片选择功能，
多选模式则调用自己定义的选择功能，再次选择时可以选择是否记录前面已选择过的图片。
```java
  // OnDragListViewDragingListener
 @Override
    public void onDragStart(int position) {
        Log.i("onDragStart()","position = " + position);
    }

    @Override
    public void onDragMoving(int position) {
        Log.i("onDragMoving()","position = " + position);
    }

    @Override
    public void onDragEnd(int position) {
        Log.i("onDragEnd()","position = " + position);
    }
    
 // 设置滑动时跟随手指移动的影像
 public void setDragShadowView(View view){
        dragShadowView = view ;
    }

```
