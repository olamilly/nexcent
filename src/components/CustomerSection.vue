<template>
	<div class="containery">
		<div class="illustration">
			<TeslaLogo class="logo" />
		</div>
		<div class="frame6-container">
			<div class="frame6">
				<h5>
					Maecenas dignissim justo eget nulla rutrum molestie. Maecenas lobortis
					sem dui, vel rutrum risus tincidunt ullamcorper. Proin eu enim metus.
					Vivamus sed libero ornare, tristique quam in, gravida enim. Nullam ut
					molestie arcu, at hendrerit elit. Morbi laoreet elit at ligula
					molestie, nec molestie mi blandit. Suspendisse cursus tellus sed augue
					ultrices, quis tristique nulla sodales. Suspendisse eget lorem eu
					turpis vestibulum pretium. Suspendisse potenti. Quisque malesuada enim
					sapien, vitae placerat ante feugiat eget. Quisque vulputate odio
					neque, eget efficitur libero condimentum id. Curabitur id nibh id sem
					dignissim finibus ac sit amet magna.
				</h5>
				<div class="customer">
					<h5 id="name" class="mt-2">Elon Musk</h5>
					<p id="position">CEO, Tesla inc.</p>
				</div>
				<div class="brands">
					<div class="brand-icons">
						<Brand1Logo />
						<Brand2Logo />
						<Brand3Logo />
						<Brand5Logo />
						<Brand6Logo />
					</div>
					<div
						style="
							display: flex;
							align-items: center;
							cursor: pointer;
							width: 100%;
							justify-content: center;
						"
					>
						<h5 id="name" style="margin-top: 0px">Meet all customers</h5>
						<svg
							width="18"
							height="21"
							viewBox="0 0 6 7"
							fill="none"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M4.42153 4.5177L5.24609 3.69314C5.34388 3.59535 5.34388 3.4368 5.24609 3.33901L4.42153 2.51445M5.17274 3.51607L1.50012 3.51607"
								stroke="#4CAF4F"
								stroke-width="0.367253"
								stroke-linecap="round"
							/>
						</svg>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>
<script setup lang="ts">
	import Brand1Logo from "@/assets/brand1Logo.vue";
	import Brand2Logo from "@/assets/brand2Logo.vue";
	import Brand3Logo from "@/assets/brand3Logo.vue";
	import Brand5Logo from "@/assets/brand5Logo.vue";
	import Brand6Logo from "@/assets/brand6Logo.vue";
	import TeslaLogo from "@/assets/TeslaLogo.vue";
</script>
<style scoped>
	.containery {
		display: flex;
		align-items: center;
		margin-bottom: 3rem;
	}
	@media (max-width: 767.98px) {
		.illustration {
			position: absolute;
			width: 100%;
			z-index: -1;
		}
		.logo {
			opacity: 0.2;
		}
		.frame6,
		.frame6-container {
			width: 100%;
		}
	}
	@media (max-width: 820px) {
		.brands {
			display: flex;
			flex-direction: column;
		}
	}
	@media (max-width: 301px) {
		.illustration {
			display: none;
		}
	}
	.illustration {
		width: 30%;
		margin-left: 1.5rem;
		margin-right: 1.5rem;
	}
	.frame6-container {
		display: flex;
		justify-content: center;
		align-items: flex-start;
	}
	.frame6 {
		width: 80%;
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: flex-start;
		text-align: left;
	}
	h2 {
		color: #4d4d4d;
		font-size: 2.4rem;
		margin: 0px;
	}
	p {
		color: #717171;
		font-size: 0.8rem;
	}
	#name {
		color: #4caf4f;
	}
	h5 {
		margin-bottom: 0px;
		color: #717171;
		font-size: 1rem;
	}
	.brands {
		width: 100%;
		display: flex;
		align-items: center;
	}
	.brand-icons {
		width: 100%;
		display: flex;
		justify-content: space-around;
		align-items: center;
	}
</style>
