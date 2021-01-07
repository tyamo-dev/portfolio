<template>
	<div id="title-container">
		<div id="my-info">
			<div id="my-job">FRONT-END ENGINEER</div>
			<div id="my-name">Riku Ishikawa</div>
			<div id="site-title">Portofolio</div>
		</div>
	</div>
</template>

<script lang="ts">
import Vue from 'vue'
export default class Title extends Vue {

}
</script>

<style lang="less" scoped>
#title-container {
	position: relative;
	width: 80vw; // 100vh - Menu width
	height: 100vh;
}
#my-info {
	position: absolute;
	top: 50%;
	left: 0;
	transform: translateY(-50%);
	margin-left: 80px;
	text-align: left;
	opacity: 0.7;

	#my-job {
		margin-left: 3px; //氏名に左端を合わせるため
		margin-bottom: 10%;
		font-size: 16px;
		line-height: 16px;
		font-weight: 500;
		opacity: 1;
	}

	#my-name {
		margin-bottom: 4%;
		font-size: 70px;
		font-weight: bold;
		line-height: 82px;
		letter-spacing: 0px;
	}

	#site-title {
		font-size: 30px;
	}
}
</style>