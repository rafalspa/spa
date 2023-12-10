<script setup>
const open = ref(false);
const toggle = () => (
	(open.value = !open.value),
	(textButton.value = open.value ? "Hide modal" : "Show modal")
);
const textButton = ref("Show modal");
</script>

<template>
	<h3>To jest strona glowna</h3>
	<button @click="toggle">{{ textButton }}</button>
	<div v-if="open">to jest ukryty tekst</div>
</template>
