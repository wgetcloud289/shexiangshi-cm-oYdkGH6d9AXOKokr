[合集 \- manim(39\)](https://github.com)[1\.【manim动画教程】\-\- 安装2023\-03\-28](https://github.com/wang_yb/p/17264724.html)[2\.【manim动画教程】\-\- 基本图形2023\-03\-29](https://github.com/wang_yb/p/17269340.html)[3\.【manim动画教程】\-\- 坐标系2023\-04\-10](https://github.com/wang_yb/p/17301528.html)[4\.【manim动画教程】\-\- 文本样式2023\-04\-07](https://github.com/wang_yb/p/17294918.html)[5\.【manim动画教程】\-\- 文字和公式2023\-04\-04](https://github.com/wang_yb/p/17285467.html)[6\.【manim动画教程】\-\- 图形样式2023\-03\-31](https://github.com/wang_yb/p/17275154.html)[7\.【manim动画教程】\-\-相机2023\-04\-19](https://github.com/wang_yb/p/17334029.html)[8\.【manim动画教程】\-\-高级动画效果2023\-04\-14](https://github.com/wang_yb/p/17317576.html)[9\.【manim动画教程】\-\-常用动画效果2023\-04\-12](https://github.com/wang_yb/p/17309865.html)[10\.【manim】之滚动字幕2022\-12\-06](https://github.com/wang_yb/p/16955924.html)[11\.【manim】之圆规动画2023\-01\-31](https://github.com/wang_yb/p/17079903.html)[12\.【manim】之目录动画2023\-02\-28](https://github.com/wang_yb/p/17163051.html)[13\.manim边学边做\-\-DecimalNumber06\-12](https://github.com/wang_yb/p/18243662)[14\.manim边学边做\-\-Integer06\-13](https://github.com/wang_yb/p/18245670)[15\.manim边学边做\-\-Variable06\-14](https://github.com/wang_yb/p/18248823)[16\.manim边学边做\-\-Title06\-20](https://github.com/wang_yb/p/18258229)[17\.manim边学边做\-\-BulletedList06\-21](https://github.com/wang_yb/p/18261017)[18\.manim边学边做\-\-SingleStringMathTex06\-23](https://github.com/wang_yb/p/18264154)[19\.manim边学边做\-\-MathTex06\-28](https://github.com/wang_yb/p/18272507)[20\.manim边学边做\-\-Tex07\-01](https://github.com/wang_yb/p/18278554):[悠兔机场](https://xinnongbo.com)[21\.manim边学边做\-\-Text07\-04](https://github.com/wang_yb/p/18284013)[22\.manim边学边做\-\-Paragraph07\-09](https://github.com/wang_yb/p/18291657)[23\.manim边学边做\-\-MarkupText07\-10](https://github.com/wang_yb/p/18294000)[24\.manim边学边做\-\-Code07\-16](https://github.com/wang_yb/p/18304450)[25\.manim边学边做\-\-Matrix07\-17](https://github.com/wang_yb/p/18307871)[26\.manim边学边做\-\-Table07\-25](https://github.com/wang_yb/p/18322456)[27\.manim边学边做\-\-点08\-09](https://github.com/wang_yb/p/18351279)[28\.manim边学边做\-\-圆形类08\-15](https://github.com/wang_yb/p/18361469)[29\.manim边学边做\-\-圆弧形08\-20](https://github.com/wang_yb/p/18368851)[30\.manim边学边做\-\-直线类08\-22](https://github.com/wang_yb/p/18374417)[31\.manim边学边做\-\-带箭头直线09\-02](https://github.com/wang_yb/p/18392446)[32\.manim边学边做\-\-曲线类09\-04](https://github.com/wang_yb/p/18396028)[33\.manim边学边做\-\-角度标记09\-07](https://github.com/wang_yb/p/18401449)[34\.manim边学边做\-\-常用多边形09\-10](https://github.com/wang_yb/p/18406455)[35\.manim边学边做\-\-通用多边形09\-13](https://github.com/wang_yb/p/18411587)[36\.manim边学边做\-\-弧形多边形09\-15](https://github.com/wang_yb/p/18415355)[37\.manim边学边做\-\-空心多边形09\-21](https://github.com/wang_yb/p/18423746)[38\.manim边学边做\-\-图形间集合关系09\-27](https://github.com/wang_yb/p/18435447)39\.manim边学边做\-\-形状匹配10\-01收起
`manim`中有几个特殊的用于**形状匹配**的对象，它们的作用是标记和注释已有的对象，本身一般不单独使用。


**形状匹配**对象一共有4种：


1. `BackgroundRectangle`：为已有的对象提供一个矩形的背景
2. `Cross`：用交叉线标记已有对象
3. `SurroundingRectangle`：用矩形框围住某个对象
4. `Underline`：为某个对象添加一条下划线


**形状匹配**的作用就是在动画中突出标记一些对象，便于更好的表达动画中的内容。


# 1\. 主要参数


`BackgroundRectangle`的主要参数有：




| **参数名称** | **类型** | **说明** |
| --- | --- | --- |
| mobject | Mobject | 被添加背景的对象 |
| color | Color | 背景的颜色 |
| stroke\_width | float | 背景边框的粗细程度 |
| stroke\_opacity | float | 背景边框的透明度 |
| fill\_opacity | float | 背景的透明度 |
| buff | float | 背景的大小，buff越大，背景的范围越大 |


背景默认是没有边框的，通过`stroke_width`参数添加边框。


`Cross`的主要参数有：




| **参数名称** | **类型** | **说明** |
| --- | --- | --- |
| mobject | Mobject | 被添加交叉标记的对象 |
| stroke\_color | Color | 交叉线的颜色 |
| stroke\_width | float | 交叉线的粗细程度 |
| scale\_factor | float | 交叉线的长度 |


`SurroundingRectangle`的主要参数有：




| **参数名称** | **类型** | **说明** |
| --- | --- | --- |
| mobject | Mobject | 矩形框所维的对象 |
| color | Color | 矩形框的颜色 |
| buff | float | 矩形框与其中内容之间的间隔 |
| corner\_radius | float | 矩形框尖角的曲率 |


`Underline`的主要参数有：




| **参数名称** | **类型** | **说明** |
| --- | --- | --- |
| mobject | Mobject | 添加下划线的对象 |
| buff | float | 下划线与对象之间的间隔 |


# 2\. 使用示例


**形状匹配**的对象总体来看都比较简单，它们的多用在一些辅助显示其他主要对象的场景中。


下面通过一些示例看看它们的作用。


## 2\.1\. 矩形背景示例


`manim`中的动画默认是黑色背景的，可以通过`BackgroundRectangle`给某个对象添加一个其他颜色的矩形背景。


用来突出显示或着重表现某个对象。



```
# 红色背景
c = Circle()
BackgroundRectangle(c, color=RED)

# 红色背景+透明度0.2
c = Circle()
BackgroundRectangle(c, color=RED, fill_opacity=0.2)

# 背景加边框
c = Circle()
BackgroundRectangle(
    c,
    color=RED,
    fill_opacity=0.2,
    stroke_width=1,
    stroke_opacity=1,
)

# 背景旋转
c = Circle()
b = BackgroundRectangle(
    c,
    color=RED,
    fill_opacity=0.2,
).rotate(PI / 4)

```

![](https://img2024.cnblogs.com/blog/83005/202410/83005-20241001180757319-166469286.gif)


## 2\.2\. 交叉标记示例


交叉标记的交点就是被标记对象的中心，标记的颜色，粗细和长短都可以调整。



```
# 标记的颜色
c1 = Circle(color=GREEN)
Cross(c1, stroke_color=RED)

c2 = Circle(color=YELLOW)
Cross(c2, stroke_color=BLUE)

c3 = Circle(color=BLUE)
Cross(c3, stroke_color=GREEN)

# 标记的粗细
c1 = Circle(color=GREEN)
Cross(c1, stroke_width=2)

c2 = Circle(color=YELLOW)
Cross(c2, stroke_width=5)

c3 = Circle(color=BLUE)
Cross(c3, stroke_width=10)

# 标记的长短
c1 = Circle(color=GREEN)
Cross(c1, scale_factor=0.5)

c2 = Circle(color=YELLOW)
Cross(c2, scale_factor=1)

c3 = Circle(color=BLUE)
Cross(c3, scale_factor=2)

```

![](https://img2024.cnblogs.com/blog/83005/202410/83005-20241001180757267-1134467670.gif)


## 2\.3\. 矩形边框示例


矩形边框一般用来突出显示某些文字，边框的尖角和与文字的间距都可以调整。



```
# 边框的间隔
fu1 = Text("福")
SurroundingRectangle(fu1, buff=0.1)

fu2 = Text("福")
SurroundingRectangle(fu2, buff=0.3)

fu3 = Text("福")
SurroundingRectangle(fu3, buff=0.6)

# 边框的圆角
fu1 = Text("福")
SurroundingRectangle(fu1, corner_radius=0.1)

fu2 = Text("福")
SurroundingRectangle(fu2, corner_radius=0.3)

fu3 = Text("福")
SurroundingRectangle(fu3, corner_radius=0.8)

```

![](https://img2024.cnblogs.com/blog/83005/202410/83005-20241001180757334-2008421876.gif)


## 2\.4\. 下划线示例


下划线是最简单的一种标记，不仅仅是中英文字，它也可以加在公式和图形的下面。



```
# 文字的下划线
t1 = Text("English")
Underline(t1, color=GREEN)

t2 = Text("中文")
Underline(t2, color=BLUE)

t3 = Tex("$a^2+b^2=c^2$")
Underline(t3, color=YELLOW)

# 图形的下划线
t1 = Square(side_length=1)
Underline(t1, color=GREEN)

t2 = Circle(radius=0.5)
Underline(t2, color=BLUE)

t3 = Star(outer_radius=0.6)
Underline(t3, color=YELLOW)

```

![](https://img2024.cnblogs.com/blog/83005/202410/83005-20241001180757414-1976181939.gif)


# 3\. 附件


文中完整的代码放在网盘中了（`shape_matcher.py`），


下载地址: [完整代码](https://github.com) (访问密码: 6872\)


