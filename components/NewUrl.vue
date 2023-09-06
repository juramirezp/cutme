<script setup>
// import {ref} from vue

const active = ref(false);
</script>

<template>
	<aside class="py-6 border-l pl-4">
		<h2 class="font-700 text-4 pl-2 text-gray-600 border-l-[6px] border-gray-500 leading-2 mt-2">New short link</h2>
		<div class="mt-6">
			<label for="url" class="text-2">Url</label>
			<input
				type="text"
				placeholder="Paste or enter long URL"
				class="border px-2 py-1 w-full placeholder:text-2"
				name="url"
			/>
		</div>
		<div class="mt-3">
			<label for="key" class="text-2">Key</label>
			<input type="text" placeholder="Enter a key" class="border px-2 py-1 w-full placeholder:text-2" name="key" />
		</div>
		<div class="flex justify-end">
			<button
				class="border-gray-900 border px-4 py-1 hover:shadow-lg hover:bg-gray-900 hover:text-white transition ease-in duration-70 text-2 mt-3"
			>
				Short
			</button>
		</div>
		<h6
			class="text-1 pl-4 border-l-[6px] border-l-green-600 bg-green-200/50 py-2 mt-4 [&.active]:translate-x-0 translate-x-5 opacity-0 [&.active]:opacity-100 transition-all ease-in duration-75"
			:class="{ active: active }"
		>
			Your url has been successfully shortened
		</h6>
		<h6
			class="text-1 pl-4 border-l-[6px] border-l-red-600 bg-red-200/50 py-2 mt-4 [&.active]:translate-x-0 translate-x-5 opacity-0 [&.active]:opacity-100 transition-all ease-in duration-75"
			:class="{ active: active }"
		>
			Error shortening the url
		</h6>
		<button @click="active = !active">actibve</button>
		{{ active }}
	</aside>
</template>
