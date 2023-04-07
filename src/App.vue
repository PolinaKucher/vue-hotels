<template>
	<Header />

	<div class="wrapper">
		<div class="hotels">
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
			<HotelItem></HotelItem>
		</div>
	</div>
</template>

<script>
	import Header from "@/components/Header.vue";
	import HotelItem from "@/components/HotelItem.vue";

	export default {
		components: {
			Header,
			HotelItem,
		},
	};
</script>

<style lang="scss">
	@import url("https://fonts.googleapis.com/css2?family=Raleway:wght@200;400;600&display=swap");
	@import "@/style/variables";

	* {
		box-sizing: border-box;
		transition: $t-normal;
		margin: 0;
		padding: 0;
	}

	body {
		font-family: "Raleway", sans-serif;
		background-color: $c-blue;
		font-size: $fs-base;
	}

	h1,
	h2,
	h3,
	h4,
	h5,
	h6 {
		padding: 0;
		margin: 0;
	}

	img {
		width: 100%;
	}

	router-link {
		cursor: pointer;
	}

	.wrapper {
		width: 100%;
		margin: 0 auto;
		max-width: 1360px;
		padding-left: 40px;
		padding-right: 40px;
	}

	.hotels {
		margin-top: 120px;
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		gap: 40px 20px;
	}
</style>
