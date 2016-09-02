# DragLlistView 
<br/>
可以拖动排序的ListView ，同时支持侧滑 ，基于“yuyidong”的开源项目的修改，主要优化了适配器数据更新方式、自定用于滑动时
跟随手指移动阴影图像、以及当ListView中ItemView 大小不一致时，将一个小点的视图放置到较大视图上时的闪烁问题。
<br/>
![](https://github.com/zhangguoning/DragLlistView/raw/master/wwwwww.gif)
<br/>
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
