<script setup>
const open2 = ref(false);
const toggle2 = () => (
	(open2.value = !open2.value),
	(textButton2.value = open2.value ? "Hide modal" : "Show modal")
);
const textButton2 = ref("Show modal");
</script>

<template>
	<div>
		<NuxtLayout>
			<div class="body-content"><NuxtPage /></div>
			<div v-if="open">to jest ukryty tekst</div>
			<div v-if="open2" class="okienko">
				to jest okno chatu <button @click="toggle2">X</button>
				<input type="text" />
			</div>
			<div class="kolko" @click="toggle2"><img src="./img/kolko.png" /></div>
		</NuxtLayout>
	</div>
</template>
