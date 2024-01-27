<script setup>
const getData = (e) => {
	console.log("info z dziecka", e);
};
</script>
<template>
	<h1>Kontakt:</h1>
	<FormsInput
		:name="'Podaj imie'"
		:valInput="''"
		@sendValue="getData($event)"
	/>
	<FormsInput
		:name="'Podaj nawisko'"
		:valInput="''"
		@sendValue="getData($event)"
	/>
</template>

<style scoped lang="scss"></style>
