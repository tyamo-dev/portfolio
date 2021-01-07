<template>
	<div id="whole-container">
		<!-- call components -->
		<Menu id="menu-component"/>
		<MainContents />
	</div>
</template>

<script lang="ts">
import Vue from 'vue';
import Menu from '@/views/Menu.vue';
import MainContents from '@/views/MainContents.vue';
import { Component } from 'vue-property-decorator';

@Component ({
	components: {
		Menu,
		MainContents
	}
})
export default class MyPage extends Vue {
	
}
</script>

<style lang="less">

#whole-container {
	display: flex;
}

#menu-component {
	width: 20vw;
	height: 100%;
}
</style>