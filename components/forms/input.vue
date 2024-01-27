<script setup>
const props = defineProps({
	name: { type: String, default: "123" },
	valInput: { type: String, default: "123" },
});
const emit = defineEmits(["sendValue"]);
const valueDef = ref(props.valInput);

watch(valueDef, (newVal, oldVal) => {
	console.log(newVal, oldVal);
});
</script>

<template>
	{{ name }}
	<input v-model="valueDef" /><br />
</template>

<style scoped></style>
