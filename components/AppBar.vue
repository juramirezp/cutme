<script setup></script>

<template class="font-normal">
	<div class="fixed top-0 w-full bg-white z-10">
		<div class="container mx-auto flex justify-between py-3">
			<NuxtLink to="/" class="">
				<h2 class="font-bold text-2xl font-raleway">Cut Me</h2>
			</NuxtLink>
			<div class="flex gap-4 items-center">
				<NuxtLink
					to="dashboard"
					class="font-normal font-400 transition-all duration-[10ms] ease-in cursor-pointer delay-0 hover:underline"
				>
					Dashboard
				</NuxtLink>
				<NuxtLink
					to="signup"
					class="font-normal font-400 bg-slate-900 text-white px-3 py-1 text-[14px] hover:shadow-sm hover:shadow-gray-600 transition-all duration-[10ms] ease-in cursor-pointer delay-0"
				>
					Login
				</NuxtLink>
			</div>
		</div>
	</div>
</template>
