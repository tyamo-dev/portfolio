<template>
	<div id="main-content-container">
		<Title />
	</div>
</template>

<script lang="ts">
import Vue from 'vue'
import Title from '@/views/Title.vue';
import { Component } from "vue-property-decorator";

@Component({
	components: {
		Title
	}
})
export default class MainContents extends Vue {
	

}
</script>

<style lang="less">

</style>