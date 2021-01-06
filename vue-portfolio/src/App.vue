<template>
	<div id="app">
		<Mypage/>
	</div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Mypage from '@/views/MyPage.vue';

@Component({
	components: {
		Mypage
	},
})
export default class App extends Vue {
	mounted() {
	}
}
</script>

<style lang="less">
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@100&display=swap');
//背景適用時に画像周りに隙間が入ることに対する対応
body,html {
    margin: 0;
    padding: 0;
}

#app {
	//---background css
	width: 100vw;
	height: calc(100vh - 3px);
	background-image: url('assets/Portfolio_background_PC.jpg');
	background-size: cover;
	overflow: hidden;

	//---common css
	//TODO: create main.less & move into file
	font-family: 'Raleway', Regular;
	color: white;
}

</style>
