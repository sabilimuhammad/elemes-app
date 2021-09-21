<template>
	<div class="container bg-white sm:bg-transparent md:bg-transparent lg:bg-transparent mx-auto flex justify-between items-center">
		<div class="my-2">
			<nuxt-link to="/">
				<img class="logo" src="@/assets/images/icons/logo.svg">
			</nuxt-link>
		</div>
		<div class="hidden sm:flex md:flex lg:flex">
			<p>Home</p>
			<p class="mx-8">About</p>
			<p>Promotions</p>
			<p class="mx-8">Blogs</p>
			<p>Contact Us</p>
		</div>
		<div class="flex">
			<button class="md:items-center lg:items-center mr-8" type="text">Masuk</button>
			<button class="h-12 w-12 btn bg-primary rounded-3xl" type="button">Daftar Sekarang</button>
		</div>
	</div>
</template>

<script>
	export default {

	}
</script>
