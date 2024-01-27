<script setup>
const props = defineProps({
	name: { type: String, default: "123" },
	valInput: { type: String, default: "123" },
});
const emit = defineEmits(["sendValue"]);
const valueDef = ref(props.valInput);

watch(valueDef, (newVal, oldVal) => {
	console.log(newVal, oldVal);
	emit("sendValue", newVal);
});
</script>

<template>
	{{ name }}

	<input
		class="input is-primary"
		type="text"
		placeholder="Wprowadz tekst"
		v-model="valueDef"
	/><br />
</template>

<style scoped></style>
