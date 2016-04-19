# flex


一、Flex布局是什么

	1.Flex是Flexible Box的缩写，意为“弹性布局”，可以为布局带来很大的灵活性。可以很快的实现css的简单布局。

	2.在使用Flex的时候需要指定一个容器为Flex布局。
	  行内元素和块元素都可以指定为Flex容器。
	  块元素为：display:flex;
	  行内元素为：display:inline-flex;

	3.兼容：Flex的兼容需要加上相应的浏览器前缀。

二、Flex需要设置在容器上的几个属性

	属性：flex-direction、flex-wrap、flex-flow、justify-countent
	align-items、align-content

		1.flex-direction：元素的排列方向
			 属性值：row（默认）水平方向，起点在左端
 					 row-reverse水平方向，起点在右端
 					 column垂直方向，起点在上方
                   	 column-reverse垂直方向，起点在下方

		2.flex-wrap：关于元素的换行
			 属性值：nowrap（默认）不换行
				     wrap换行，从上方开始排列
				     wrap-reverse换行，从下方开始排列

		3.flex-flow：可以同时设置flex-direction和flex-wrap，其中默认值是row
				     nowrap

		 4.justify-content：规定了一组元素的对齐方式
			 属性值：flex-start（默认）左对齐
					  flex-end右对齐
					  center居中对齐
					  space-between两端对齐，元素之间间隔相同
					  space-around元素之间的间隔是元素到边框距离的2倍

		5.align-items在y轴的对齐方式
			 属性值：flex-start在容器的顶端对齐
					  flex-end在容器的底端对齐
					  center  y轴的中间对齐
					  baseline以容器内第一行文字的基线对齐 
					  stretch（默认值）如果项目未设置高度或设为auto将占满容器高度

		 6.align-center设置多行元素的对齐方式，对单行元素不起作用
			 属性值：flex-start在x，y的起点对齐
					  flex-end在x，y的末端对齐
					  center在y轴的中点对齐
					  space-between在y轴的上下端对齐其余的居中
					 space-around在每根轴线两侧的间隔都相等。所以，轴线之间的间隔比轴线与边框的间隔大一倍。