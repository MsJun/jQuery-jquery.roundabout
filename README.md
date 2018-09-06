# jQuery-jquery.roundabout
jQuery3D轮播插件jquery.roundabout.js
  
  
 
      <div class="in exhibition_hall">
	      <div id="" class="roundabout_box">
		    <ul>
			    <li><a href="#"><img src="" alt=""></a></li>
			    <li><a href="#"><img src="" alt=""></a></li>
			    <li><a href="#"><img src="" alt=""></a></li>
			    <li><a href="#"><img src="" alt=""></a></li>
		  </ul>
		  <a href="javascript:void(0)" class="btn_l"><</a>
		  <a href="javascript:void(0)" class="btn_r">></a>
	    </div>
    </div>
    
    
# JS
      $(document).ready(function(){
		    $('.roundabout_box ul').roundabout({
			  duration: 600, // 运动速度
			  autoplay: true, // 自动播放
			  autoplayDuration: 1500,  // 自动播放的时间
			  minOpacity: 0,  //最小的透明度
			  maxOpacity: 1,  //最大的透明度
			  reflect: true,  // 为true时是从左向右移动，为false从右向左移动
			  startingChild: 2,  // 默认的显示第几张图片
			  autoplayInitialDelay: 5000,  // 从第几秒时，开始自动播放（默认毫秒）开始的第一次管用
			  autoplayPauseOnHover: true,  // 鼠标移入元素内是否自动播放，为true不播放，false还自动播放
			  enableDrag: true,  // 在移动端可以拖拽播放
			  btnPrev: ".btn_r", // 右按钮
    		btnNext: ".btn_l", // 左按钮
		  });
	  });
# 插件的其余参数

    bearing: 0.0,						
		tilt: 0.0,							// 倾斜度 正值向上倾, -值向下
		minZ: 100,							// 最小的层级
		maxZ: 280,							// 最大的层级
		minOpacity: 0.4,					// 最小透明度
		maxOpacity: 1.0,					// 最大透明度
		minScale: 0.4,						// 最小缩放值
		maxScale: 1.0,						// 最大缩放值
		duration: 600,						// 运动速度
		btnNext: null,						// 下一个按钮
		btnNextCallback: function() {},		// 下一个按钮 回调
		btnPrev: null,						// 上一个按钮
		btnPrevCallback: function() {},		// 上一个按钮回调
		btnToggleAutoplay: null,			// 按钮点击开启自动播放或关闭
		btnStartAutoplay: null,				// 按钮点击开启自动播放
		btnStopAutoplay: null,				// 按钮点击关闭自动播放
		easing: "swing",					// 移动的动画效果 swing流畅
		clickToFocus: true,					// 点击当前轮播设为焦点
		clickToFocusCallback: function() {},// 点击当前轮播设为焦点回调
		focusBearing: 0.0,					// 修改焦点的位置 360度的位置
		shape: "lazySusan",
		debug: false,
		childSelector: "li",				// 子元素
		startingChild: null,				// 默认的显示第几张图片
		reflect: false,						// 为true时是从左向右移动，为false从右向左移动
		floatComparisonThreshold: 0.001,
		autoplay: false,					// 自动播放
		autoplayDuration: 1000,				// 自动播放的时间
		autoplayPauseOnHover: false,		// 鼠标移入元素内是否自动播放，为true不播放，false还自动播
		autoplayCallback: function() {},	// 自动轮播的回调
		autoplayInitialDelay: 0,			// 从第几秒时，开始自动播放（默认毫秒）开始的第一次管用
		enableDrag: false,					// 在移动端可以拖拽播放
		dropDuration: 600,					// 拖拽的运动速度
		dropEasing: "swing",				// 拖拽的运动动画
		dropAnimateTo: "nearest",			// 拖拽的动画方式
		dropCallback: function() {},		// 拖拽的回调函数
		dragAxis: "x",						// 拖拽的方向x轴方向和y轴方向 切换
		dragFactor: 4,
		triggerFocusEvents: true,			
		triggerBlurEvents: true,
		responsive: false					// 窗口变化响应
