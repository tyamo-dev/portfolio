<template>
	<div id="menu-container">
		<div id="menus">
			<div class="tabs selected">About</div>
			<div class="tabs">Works</div>
			<div class="tabs">Contact</div>
		</div>
	</div>
</template>

<script lang="ts">
import Vue from 'vue';
import { Component } from "vue-property-decorator";

@Component
export default class Menu extends Vue{
	
}
</script>

<style lang="less" scoped>

#menus {
	margin-top: 86px;
	margin-left: 150px;

	.tabs {
		padding: 1px;
		height: 22px;
		font-size: 19px;
		font-weight: 600;
		letter-spacing: 1px;
		color: rgba(255, 255, 255, 0.3);
		margin-bottom: 22px;
	}

	.selected {
		position: relative;
		color: rgba(255, 255, 255, 0.7);
	}

	.selected::before {
		position: absolute;
		content: '';
		top: 50%;
		left: -26px;
		width: 18px;
		border-top: 1px solid white;
		opacity: 0.7;
	}
}
</style>