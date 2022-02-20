<script setup lang="ts">
</script>

<template>
	<div id="head" class="py-12 " md="flex gap-12 justify-center items-center">
		<h1 md="w-1/2" class="font-bold font-serif pb-6 text-4xl">The creative crew</h1>
    <div md="w-1/2" >
	  <h2 font="sans semibold" class="bg-transparent text-lg mb-2"
			>Who we are
		</h2>
		<p class="font-sans text-sm mr-6"
			>We are team of creatively diverse. driven. innovative individuals
			working in various locations from the world.</p
		>
</div>
	</div>
	<div id="body" class="mt-6 grid gap-3 grid-cols-2 md:grid-cols-3">
		<div class="w-full pr-6 relative" v-for="x in [1,2,3,4,5,6]" :key="x" :class="{'<sm:mt-18': ! (x%2) , 'mt-18': x == 2 || x == 5 }" >
			<img :src="`/img/photo${x}.png` "  class="mr-4" alt="" />
			<h2
				class="
					font-serif
					text-xs
					ml-6
					transform
					origin-bottom-right
					top-16
					right-5 rotate-90 absolute
				">
				Product owner
			</h2>

			<h3 class="font-sans font-semibold mt-4 text-sm">Bill Mahoney</h3>
		</div>
	</div>

	<div id="footor" class="flex my-8 text-[#A9A9A9] justify-center items-center">
		<p >created by theSwordBreaker - devChallenges.io</p>
	</div>
</template>
<style>
  .font-mono {
  	font-family: "Montserrat", sans-serif;
  }
  .font-sans {
  	font-family: "Poppins", sans-serif;
  }
  .font-serif {
  	font-family: "PT Serif", serif;
  }
</style>


<route lang="yaml">
meta:
  layout: home
</route>
