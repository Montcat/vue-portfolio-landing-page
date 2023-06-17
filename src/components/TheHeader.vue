<template>
	<header class="header">
		<a href="#" class="logo">C. Oliver</a>

		<nav class="navbar">
			<a href="#" class="active">Home</a>
			<a href="#">About</a>
			<a href="#">Services</a>
			<a href="#">Portfolio</a>
			<a href="#">Contact</a>
		</nav>
	</header>
</template>

<script setup></script>

<style scoped>
	.header {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		padding: 20px 10%;
		background-color: transparent;
		display: flex;
		justify-content: space-between;
		align-items: center;
		z-index: 100;
	}

	.logo {
		font-size: 25px;
		color: #031540;
		text-decoration: none;
		font-weight: 700;
	}

	.navbar a {
		font-size: 18px;
		color: #fff;
		text-decoration: none;
		font-weight: 500;
		margin-left: 35px;
		transition: 0.3s;
	}

	.navbar a:hover,
	.navbar a.active {
		color: #00abf0;
	}
</style>
