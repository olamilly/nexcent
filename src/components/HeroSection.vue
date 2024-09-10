<template>
	<div class="containery">
		<div class="frame-container">
			<div class="frame">
				<h1 id="large-text">
					<span style="color: #4d4d4d">Lessons and Insights</span>
					<br />
					<span style="color: #4caf4f"> from 8 years</span>
				</h1>
				<p id="small-text">
					Where to grow your business as a photographer: site or social media?
				</p>
				<button class="medium">Register</button>
			</div>
		</div>
		<div class="illustration">
			<illustration />
		</div>
	</div>
</template>
<script setup lang="ts">
	import illustration from "../assets/HeroIllustation.vue";
</script>
<style scoped>
	@media (max-width: 767.98px) {
		.frame-container {
			margin-top: 0px;
		}
	}
	/* @media (max-height: 300px) {
		.containery {
			margin-top: 60%;
		}
	} */
	.containery {
		background-color: #f5f7fa;
		width: 100%;
		height: 100dvh;
		display: flex;
		/* position: absolute; */
		/* top: 20%; */
	}
	.frame {
		text-align: left;
		width: 85%;
	}
	.frame-container {
		margin-top: -3rem;
		padding: 1.3rem;
		justify-content: flex-end;
		width: 60%;
	}
	.illustration {
		justify-content: center;
		width: 40%;
	}
	.illustration,
	.frame-container {
		display: flex;
		align-items: center;
	}
	#large-text {
		font-weight: bold;
		font-size: 3.5rem;
		margin-bottom: 0.7rem;
	}
	#small-text {
		color: #717171;
		margin: 0px;
		font-size: 0.8rem;
		margin-bottom: 0.7rem;
	}
</style>
