<template>
	<div>
			<div class="col-md-12 col-xs-12 col-sm-12 text-center _res" v-if="isShow">
				<h3>你的知音都在这里</h3>
				<p>表达网民立场，记录个人生活，聚集意见领袖，众多草根精英，以我们的观点影响社会的进程 。</p>
				<hr>
				<button type="button" class="btn btn-primary">注册博客</button>
				<button type="button" class="btn btn-primary" @click="show"><span class="glyphicon glyphicon-refresh"></span></button>
			</div>
			
			<div class="col-md-12 col-xs-12 col-sm-12 _res" v-if="!isShow">
				<form action='#' method='post'>
					<div class="col-lg-12 col-md-12 col-sm-12 col-xs-12">
						
						<div class="text-center">
							<h3>欢迎登录</h3>
						</div>
						
						<div class="form-group">
							<label for="exampleInputEmail1">用户名:</label>
							<input type="text" class="form-control" placeholder="请输入用户名" name='username'>
						</div>
						
						<div class="form-group has-feedback">
							<label for="exampleInputPassword1">用户密码:</label>
							<input id="password" class="form-control" :type="pas" placeholder="请输入密码"  name='pwd'>
							<span :class="btn" class="glyphicon form-control-feedback"></span>
							<p><label><input id="meod" type="checkbox" @click="eye"> 显示密码</label></p>
						</div>
						
						<div class="text-center">
							<button type="button" class="btn btn-primary">登录博客</button>
							<button type="button" class="btn btn-primary" @click="show"><span class="glyphicon glyphicon-refresh"></span></button>
						</div>
						
						
					</div>
				</form>
			</div>
			<p class="_line"></p>
	</div>
	
</template>

<script>
	export default {
		data (){
			return {
				isShow:true,
				eyes:false,
				pas:"password",
				btn:"glyphicon-eye-open"
			}
			
		},
		methods: {
			show(){				
					this.isShow = !this.isShow
					// 登录表单切换
			},
			
			eye (){
				if(this.eyes = !this.eyes){
					console.log(this.eyes)
					this.btn = 'glyphicon-eye-open'
					this.pas = 'text'
				}else{
					this.btn = 'glyphicon-eye-close'
					this.pas = 'password'
				}
				// 密码显示切换
			}
			
		},	
	}
</script>

<style scoped>
	._res {
		background-color: #F6F6F6;
		border-radius: 2px;
		padding-bottom: 10px;
	}
	._line {
		width: 100%;
		height: 5px;
		display: block;
		float: left;
		border-bottom: 1px solid #EAEAEA;
		border-top: 1px solid #EAEAEA;
		margin-top: 6px;
		padding: 0px;
		margin-bottom: -5px;
	}
</style>
