<template>
	<div class="flex items-center">
		<img src="https://github.com/HerbertSousa.png" alt="Herbert" class="mr-6 w-20 h-20 rounded-full">
		<div class="flex flex-col w-full">
			<strong class="text-title text-2xl">Herbert</strong>
			<p class="flex items-center">
				<img src="icons/level.svg" alt="levelup" class="mr-2">
				<span class="text-base">Level {{ level }}</span>
			</p>
		</div>
	</div>
</template>

<script lang="ts">
import Vue from 'vue';
import { mapState } from 'vuex';

export default Vue.extend({
	computed: mapState('Challenges', ['level']),
});
</script>
