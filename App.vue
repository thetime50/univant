<script>
	import checkUpdate from '@/uni_modules/uni-upgrade-center-app/utils/check-update';
	export default {
		onLaunch: function() {
			console.log('App Launch')
			checkUpdate()//更新升级
		},
		mounted() {
			// #ifdef H5
			//const VConsole = require('@/common/js/vconsole.min.js')
			//new VConsole()
			// #endif
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	@import "/wxcomponents/vant/define.wxss";
	@import "/wxcomponents/vant/common/index.wxss";
	/*每个页面公共css */
	/* #ifndef APP-NVUE */
	view{
		box-sizing: border-box;
	}
	@font-face {
	    font-family: "iconfont";
	    src: url('https://at.alicdn.com/t/font_2354462_s00xh8caffp.ttf');
	}
	.ico{
		font-family: iconfont;
	}
	/* #endif */
	
	.test123{
		display: flex;
		flex: 0 0 auto;
		transform: translate(10,10);
	}
</style>
