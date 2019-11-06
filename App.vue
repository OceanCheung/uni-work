<script>
	export default {
		onLaunch: function() {
			console.log('当uni-app初始化完成时触发，全局只触发一次')
		},
		onShow: function() {
			console.log('当 uni-app 启动，或从后台进入前台显示(app显示)')
		},
		onHide: function() {
			console.log('当 uni-app 从前台进入后台（app隐藏）')
		},
		onError:function(){
			console.log("报错啦...")
		}
	}
</script>

<style>
	/*每个页面公共css */
</style>
