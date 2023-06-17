<template>
	<section class="home">
		<div class="home-image">
			<img :src="HomeImage" alt="image" />
		</div>

		<div class="home-content">
			<h1>Hi, I'm Chosen Oliver</h1>
			<h3>Frontend Developer</h3>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore
				obcaecati fugiat laudantium ipsum.
			</p>
			<div class="home-sci">
				<a href="#"><IconFacebook /></a>
				<a href="#"><IconTwitter /></a>
				<a href="#"><IconInstagram /></a>
				<a href="#"><IconLinkedIn /></a>
			</div>

			<a href="#" class="btn">Download CV</a>
		</div>
	</section>
</template>

<script setup>
	import IconFacebook from "@/components/icons/IconFacebook.vue";
	import IconTwitter from "@/components/icons/IconTwitter.vue";
	import IconInstagram from "@/components/icons/IconInstagram.vue";
	import IconLinkedIn from "@/components/icons/IconLinkedIn.vue";
	import HomeImage from "@/assets/images/image.png";
</script>

<style lang="scss" scoped>
	.home {
		height: 100vh;
		background: linear-gradient(-90deg, #031540 65%, #fff 35%);
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 0 10%;
	}

	.home-image {
		display: flex;
		justify-content: center;
		align-items: center;
		width: 400px;
		height: 400px;
		background: #031540;
		border-radius: 50%;
		border: 25px solid #fff;
		outline: 25px solid #031540;
	}

	.home-image img {
		border-radius: 50%;
		object-fit: fill;
		bottom: 40px;
		max-width: 290px;
	}

	.home-content {
		max-width: 600px;
		color: #fff;
		text-align: right;

		h1 {
			font-size: 44px;
			line-height: 1.2;
		}

		h3 {
			font-size: 40px;
			color: transparent;
			-webkit-text-stroke: 0.5px #fff;
			background-image: linear-gradient(#00abf0, #00abf0);
			background-repeat: no-repeat;
			background-clip: text;
			-webkit-background-clip: text;
			background-position: -405px 0;
			animation: animateText 6s linear infinite;
		}

		@keyframes animateText {
			0%,
			95%,
			100% {
				background-position: -410px 0;
			}
			65%,
			85% {
				background-position: 0 0;
			}
		}

		p {
			font-size: 1rem;
			margin-top: 20px;
		}
	}

	.home-sci {
		margin: 25px 0 40px;
	}

	.home-sci a {
		display: inline-flex;
		justify-content: center;
		align-items: center;
		width: 40px;
		height: 40px;
		background: transparent;
		border: 2px solid #fff;
		border-radius: 50%;
		font-size: 20px;
		color: #00abf0;
		text-decoration: none;
		margin-left: 12px;
		transition: 0.5s;
	}

	.home-sci a:hover {
		background: #00abf0;
		color: #fff;
		border-color: #00abf0;
		box-shadow: 0 0 10px #00abf0;

		svg {
			fill: #031540;
		}
	}
	.btn {
		padding: 12px 35px;
		background: #00abf0;
		border-radius: 40px;
		font-size: 17px;
		color: #fff;
		text-decoration: none;
		font-weight: 600;
		letter-spacing: 1px;
		box-shadow: 0 0 10px #00abf0;
		transition: 0.5s;
	}

	.btn:hover {
		box-shadow: none;
	}
</style>
