<template>
	<div class="container mx-auto grid grid-cols-[auto_300px] min-h-[calc(100vh-55px)]">
		<div class="">
			<h1 class="font-700 text-6 pl-2 text-gray-600 border-l-[6px] border-gray-500 leading-2 my-6">Dashboard</h1>
			<section class="overflow-scroll max-h-[calc(100vh-130px)] pr-4">
				<ShortLinkDetail v-for="link in 15" />
			</section>
		</div>
		<NewUrl />
	</div>
</template>
