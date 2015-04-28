# AndroidSegmentControl

## Introduction
A android custom view works like SegmentControl in IOS

## Usage

* Add the below code in you layout xml file
``` XML
<com.huibin.androidsegmentcontrol.SegmentControl
        xmlns:segmentcontrol="http://schemas.android.com/apk/res-auto"
        android:id="@+id/segment_control"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="15sp"
        segmentcontrol:texts="未签到|全部|已签到" <!--标签的内容-->
        segmentcontrol:colors="#e00032"
        segmentcontrol:cornerRadius="5dip"
        segmentcontrol:direction="horizon" <!--标签的显示的方向-->
        segmentcontrol:verticalGap="8dip"
        segmentcontrol:horizonGap="8dip"
        segmentcontrol:selectedIndex="1"/><!--默认选中哪个标签,默认是0,当大于标签的个数就默认选中为最后一个标签-->
```
* Then add these code

``` Java
SegmentControl segmentControl = (SegmentControl) findViewById(R.id.segment_control);
segmentControl.setmOnSegmentControlClickListener(new SegmentControl.OnSegmentControlClickListener() {
    @Override 
    public void onSegmentControlClick(int index) {
        //处理点击标签的事件
    } 
}); 
```
* Enjoy yourself

## Screen snapshot
![snapshot](https://github.com/liuhuibin/AndroidSegmentControl/blob/master/.raw/snapshot.jpg)
