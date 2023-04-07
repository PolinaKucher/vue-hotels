<template>
	<header class="header">
		<div class="wrapper">
			<router-link>
				<img
					src="../assets/vacanteer.png"
					alt="Logo" />
			</router-link>

			<div>
				<form class="search">
					<input
						class="search__input"
						type="text"
						name="search"
						placeholder="Going to:" />
					<button
						type="submit"
						class="search__btn">
						<img
							src="@/assets/search.png"
							alt="search"
							class="search__icon" />
					</button>
				</form>
			</div>

			<router-link class="link">My choice</router-link>
		</div>
	</header>
</template>

<script>
	// export default {
	// 	name: "v-header",
	// };
</script>

<style lang="scss" scoped>
	@import "@/style/variables";

	form {
		width: 300px;
	}

	.search {
		display: flex;
		align-items: center;
		width: 100%;

		&__btn {
			background-color: $c-white;
			padding: 5px 10px;
			height: 40px;
			border: none;

      &:hover,:focus,:focus-visible {
        outline: 2px solid $c-yellow;
      }
		}

		&__icon {
			width: 20px;
			height: 20px;
		}

		&__input {
			padding: 5px 10px;
			height: 40px;
			border: none;
			width: 400px;
			background-color: $c-white;

			&::placeholder {
				color: rgba($color: $c-blue, $alpha: 0.3);
				text-transform: uppercase;
			}

			&:focus-visible {
				outline: 2px solid $c-yellow;
			}
		}
	}
	.header {
		background-color: $c-blue;
		border-bottom: 2px solid rgba($color: #fff, $alpha: 0.2);
		position: fixed;
		height: 80px;
		bottom: 0;
		right: 0;
		left: 0;
		top: 0;
	}

	.wrapper {
		height: 100%;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	img {
		height: 75px;
	}

	.link {
		color: $c-yellow;
		text-transform: uppercase;
		font-size: 22px;

		&:hover {
			transform: scale(1.03);
		}
	}
</style>
