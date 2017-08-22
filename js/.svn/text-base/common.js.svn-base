window.onload = function(){
	// 用户头像高度控制（宽高等比例）
	var user_w = $('.icon_user').width();
	$('.icon_user').height(user_w);
	// 刷新文字点击范围等高
	var fresh_h = $('.img_yz').height();
	$('.img_yz').css('line-height',fresh_h +'px');
	//点击获取验证码
	$('.btn_yz').on('touchend',function(){
		var $_this = $(this);
		$_this.css('background-color','#bebdbd');
		$_this.html('5秒后重新发送');
		setTimeout(function(){
			$_this.css('background-color','#b3d465');
			$_this.html('获取验证码');
		},5000)
	});
	// 确认领取
	$('#lq_sure').on('touchend',function(){
		var html = "<div class=\"f17 white alert_black txt_c border-radius10 dispBox hvCenter\">恭喜您<br />领取成功！</div>";
		var page = $('.page_merchant_lq');
		page.append(html);
		setTimeout(function(){
			page.find('.alert_black').remove();
			location.href = "share_out_succ.html";
		},1500)
	});
	// 发送手机
	$('#send_tel').on('touchend',function(){
		var html = "<div class=\"layer\"><div class=\"alert_white txt_c border-radius10\"><div class=\"hvCenter dispBox alert_white_top\"><div class=\"\"><p class=\"f17 bold\">http://www.51vtuilm.cn</p><p class=\"f13\">发送成功！</p></div></div><div class=\"hvCenter dispBox alert_white_btn lineTop\"><a href=\"javascript:void(0);\"class=\"color_blue f17 d_block\">好</a></div></div></div>";
		var page = $('.page_lq_succ');
		page.append(html);
	});
	$('.page_lq_succ').on('touchend','.alert_white_btn',function(){
		$(this).parents('.layer').hide();
	});
	//android input height
	var w_w = $(window).width(),w_h = $(window).height();
	var reg_box_h = w_h * 0.52, pwd_box_h = w_h * 0.23;
	$('.reg_box').height(reg_box_h);
	$('.pwd_box').height(pwd_box_h);
	
}
