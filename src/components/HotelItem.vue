<template>
	<div class="post">
		<router-link>
			<img
				class="post__photo"
				src="@/assets/hotel.jpg"
				alt="" />
		</router-link>
		<div class="post__footer">
			<h3>Lorem ipsum dolor sit amet</h3>
			<div class="post__price">
				<span>Price:</span>
				<span class="price"> $456</span>
				<span class="specific"> (Room per day)</span>
			</div>
			<div class="post__btns">
				<router-link class="details">
					<span> Details </span>
				</router-link>
				<button
					class="like"
					type="button">
					<img
						src="@/assets/heart.png"
						alt="Like" />
				</button>
			</div>
		</div>
	</div>
</template>

<script></script>

<style lang="scss" scoped>
	@import "@/style/variables";

	h3 {
		color: $c-dark-blue;
		text-transform: uppercase;
	}

	.post {
		background-color: $c-white;
		height: 500px;
		padding: 5px;

		&:hover {
			transform: scale(1.03);
		}

		&__photo {
			margin: 0 auto;
			height: 50%;
		}

		&__footer {
			justify-content: space-around;
			flex-direction: column;
			display: flex;
			padding: 10px;
			height: 50%;
		}

		&__price > span:first-child {
			color: $c-dark-blue;
		}

		&__btns {
			display: flex;
			align-items: center;
			justify-content: space-between;
		}
	}

	.price {
		margin-left: 15px;
		font-weight: 600;
		color: $c-red;
	}

	.specific {
		color: rgba($color: $c-dark-blue, $alpha: 0.5);
		font-size: $fs-base - 4px;
		margin-left: 5px;
	}

	.details {
		background-color: $c-blue;
		text-transform: uppercase;
		justify-content: center;
		font-size: $fs-base;
		align-items: center;
		color: $c-yellow;
		display: flex;
		width: 140px;
		border: none;
		height: 40px;

		&:hover {
			transform: scale(1.03);
		}
	}

	.like {
		background-color: transparent;
		border: none;
		width: 40px;

		&:hover {
			transform: scale(1.1);
		}
	}
</style>
