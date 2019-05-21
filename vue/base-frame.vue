<template>
	<!DOCTYPE html>
	<html>
		<head>
			<meta charset="utf-8" />
			<title>{{title}}|寒梅公益</title>
			<link rel="stylesheet" href="css/main.css" />
			<slot name="css"></slot>
		</head>
		<body>
			<div class="banner">
				<div class="logo wapper">		
				</div>
			</div>
			<div class="nav">
				<div class="items wapper inline">
					<a href="index.html" class="item active">首页</a>
					<a href="index.html" class="item">听见你的声音</a>
					<a href="index.html" class="item">慈善新闻</a>
					<a href="index.html" class="item">信息公布</a>
					<a href="index.html" class="item">志愿者</a>
					<a href="index.html" class="item last-item">关于我们</a>
				</div>
			</div>
			<div class="main-content wapper">
				<slot name="content"></slot>
			</div>
			<div class="footer">
				<div class="content wapper">
					<div class="slice">
						<div class="title">成都寒梅公益服务中心</div>
						<div>成都市民政局正式核准的民办非盈利企业组织，服务范围包括帮扶残障儿童教育，支持贫苦学生，关爱弱势群体等。</div>
					</div>
					
					<div class="slice">
						<div class="title">友情链接</div>
						<div>
							<ul>
								<li>浙江新华爱心教育基金会</li>
								<li>中国公益慈善总会</li>
								<li>腾讯公益</li>
							</ul>
						</div>
					</div>
					<div class="slice focus">
						<div class="title">关注我们</div>
						<div>
							<ul class="items">
							<li><img src="img/1542784580.png" width="100px" height="100px"/><div>微信</div></li>
							<li><img src="img/1542784580.png" width="100px" height="100px"/><div>微博</div></li>
						</ul>
						</div>
					</div>
					
					<div class="copy">
						&copy;<a href="index.html">成都寒梅公益服务中心</a> · <a href="copy.html">版权与使用限制</a> · <a href="private.html">隐私政策</a> · 蜀ICP7893412-1
					</div>
				</div>
			</div>
			<slot name="js"></slot>
			<script language="JavaScript">
				var _footer = document.getElementsByClassName("footer")[0];
				if(_footer.offsetHeight+_footer.offsetTop<window.innerHeight){
					_footer.style.position='absolute';
				}
			</script>
		</body>
	</html>
</template>

<script>
	export default{
		data(){
			return {
				title:'模板'
			}
		}
	}
</script>

<style>
</style>