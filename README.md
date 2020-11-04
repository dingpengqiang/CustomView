# CustomView



2020-11-03:开始总结自定义view


## 自定义属性的值

1.reference:参考某一资源ID
    <ImageView android:background = "@drawable/图片ID"/>

2.color:颜色值
    <TextView android:textColor = "#00FF00" />

3.boolean:布尔值
    <Button android:focusable = "true"/>

4.dimension:尺寸值
    <Button android:layout_width = "42dp"/>

5.string:字符串
    <TextView android:text = "我是文本"/>

6.enum:枚举值
    <LinearLayout  android:orientation = "vertical"/>

7.float:浮点值
    <alpha android:fromAlpha = "1.0"/>

8.integer:整型值
    <animated-rotate android:framesCount = "12"/>

9.fraction:百分数
    <rotate android:pivotX = "200%"/>

10.flag:位或运算
    <TextView android:gravity="bottom|left"/>

11.混合型
    <ImageView android:background = "@drawable/图片ID" />

    <ImageView android:background = "#00FF00" />

## 绘制
### 1.绘制文字
  基线算法：
  `
    public static float getBaseline(Paint p) {
        Paint.FontMetrics fontMetrics = p.getFontMetrics();
        return (fontMetrics.descent - fontMetrics.ascent) / 2 -fontMetrics.descent;
    }
  `

