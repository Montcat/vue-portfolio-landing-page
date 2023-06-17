<template>
	<div class="app-container">
		<div class="header-wrapper">
			<TheHeader />
		</div>

		<main class="content-wrapper">
			<TheHome />
		</main>
	</div>
</template>

<script setup>
	import TheHeader from "./components/TheHeader.vue";
	import TheHome from "./components/TheHome.vue";
</script>

<style lang="scss" scoped></style>
