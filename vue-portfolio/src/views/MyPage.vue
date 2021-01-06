<template>
	<div id="whole-container">
		<!-- call components -->
		<Menu id="menu-component"/>
	</div>
</template>

<script lang="ts">
import Vue from 'vue';
import Menu from '@/views/Menu.vue';
import { Component } from 'vue-property-decorator';

@Component ({
	components: {
		Menu
	}
})
export default class MyPage extends Vue {
	
}
</script>

<style lang="less">

#menu-component {
	width: 20vw;
	height: 100%;
}
</style>