# Full-screen-switching
全屏切换效果

<br>

<h3>DEMO</h3>
http://moerj.com/Full-screen-switching/

<br>

<h3>Getting Started</h3>
	<!-- 引入jQuery -->
	<script src="jquery-1.11.2.min.js"></script>
	
	<!-- 引入全屏切换 -->
	<script src="pageswitch.js"></script>

<br>
<h3>HTML</h3>

	<div id="container">
		<div class="section active" id="section0">
		页面1内容
		</div>
		<div class="section" id="section1">
		页面2内容
		</div>
		<div class="section" id="section2">
		页面3内容
		</div>
		<div class="section" id="section3">
		页面4内容
		</div>
	</div>


<br>
<h3>default options</h3>
	$("#container").switchPage({
		'container' : '#container',//容器
		'sections' : '.section',//子容器
		'easing' : 'ease',//特效方式，ease-in,ease-out,linear
		'duration' : 1000,//每次动画执行的时间
		'pagination' : true,//是否显示分页
		'loop' : true,//是否循环
		'keyboard' : true,//是否支持键盘
		'direction' : 'vertical',//滑动的方向 horizontal,vertical
		'onpageSwitch' : true//允许点击分页按钮切换到对于页面
	});
