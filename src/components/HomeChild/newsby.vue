<template>
	<div>
		<div class="row">


			<div class="col-lg-5 col-md-6 col-sm-6 col-xs-12">
				<swiper :options="swiperOption" id="containers">
					<swiper-slide><a class="items" href="#"><img src="../../../static/img/a1.jpg" /></a></swiper-slide>
					<swiper-slide><a class="items" href="#"><img src="../../../static/img/a2.jpg" /></a></swiper-slide>
					<swiper-slide><a class="items" href="#"><img src="../../../static/img/a3.jpg" /></a></swiper-slide>
					<swiper-slide><a class="items" href="#"><img src="../../../static/img/a4.jpg" /></a></swiper-slide>
					<swiper-slide><a class="items" href="#"><img src="../../../static/img/a5.jpg" /></a></swiper-slide>
					<div class="swiper-pagination" slot="pagination"></div>
					<!-- <div class="swiper-button-prev" slot="button-prev"></div>
					<div class="swiper-button-next" slot="button-next"></div> -->
				</swiper>
			</div>
			
				
			

			<!-- 轮播图 -->


			<div class=" col-lg-7 col-md-6 col-sm-6 col-xs-12">
				<!-- <div class="_box-tent col-md-12 col-ms-12 col-xs-12" v-for="(item,index) in news.data" v-if='index<=4' :key="item.id">
						<h4><a :href="item.url">{{item.author_name}}</a></h4>
						<small><p>{{item.title}}</p></small>
						<hr style="background-color: #999999;" />
					</div> -->
				<div class="_box-tent col-md-12 col-ms-12 col-xs-12">
					<h4><a>你哈</a></h4>
					<small>
						<p>难受吗 你是什么东西啊</p>
					</small>
					<hr style="background-color: #999999;" />
				</div>
				<div class="_box-tent col-md-12 col-ms-12 col-xs-12">
					<h4><a>你哈</a></h4>
					<small>
						<p>难受吗 你是什么东西啊</p>
					</small>
					<hr style="background-color: #999999;" />
				</div>
				<div class="_box-tent col-md-12 col-ms-12 col-xs-12">
					<h4><a>你哈</a></h4>
					<small>
						<p>难受吗 你是什么东西啊</p>
					</small>
					<hr style="background-color: #999999;" />
				</div>
				<div class="_box-tent col-md-12 col-ms-12 col-xs-12">
					<h4><a>你哈</a></h4>
					<small>
						<p>难受吗 你是什么东西啊</p>
					</small>
					<hr style="background-color: #999999;" />
				</div>
				<div class="_box-tent col-md-12 col-ms-12 col-xs-12">
					<h4><a>你哈</a></h4>
					<small>
						<p>难受吗 你是什么东西啊</p>
					</small>
					<hr style="background-color: #999999;" />
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				swiperOption: {
					spaceBetween: 30,
					centeredSlides: true,
					autoplay: {
						delay: 2500,
						disableOnInteraction: false
					},
					pagination: {
						el: '.swiper-pagination',
						clickable: true
					},
					navigation: {
						nextEl: '.swiper-button-next',
						prevEl: '.swiper-button-prev'
					}
				}

			}
		}
	}
</script>

<style scoped>
	._box-tent h4 a {
		text-decoration: none;
		color: #000000;
	}

	._box-tent h4 a:hover {
		color: #337AB7;
	}

	._box-tent p {}

	.btns {
		position: absolute;
		top: 45%;
		margin-top: -35px;
		width: 40px;
		height: 70px;
		color: #d6d3d5;
		font-size: 36px;
		line-height: 70px;
		text-align: center;
		cursor: pointer;
	}

	.btns:hover {
		background: rgba(127, 120, 125, 0.8);
	}

	.items {
		position: absolute;

	}

	.items img {
		height: 420px;
	}

	#containers {
		width: 350px;
		height: 460px;
		position: relative;
		overflow: hidden;
	}
</style>
