<script setup>
const getData = (e) => {
	console.log("info z dziecka", e);
};

useHead({
	title: "Kompuland - Kontakt",
	meta: [{ name: "description", content: "moja stronka" }],
});
</script>
<template>
	<h1>Kontakt:</h1>
	<FormsInput
		:name="'Podaj imie'"
		:valInput="''"
		@sendValue="getData($event)"
	/>
	<FormsInput
		:name="'Podaj nazwisko'"
		:valInput="''"
		@sendValue="getData($event)"
	/>
	<FormsInput
		:name="'Podaj e-mail'"
		:valInput="''"
		@sendValue="getData($event)"
	/>
	<FormsInput
		:name="'Podaj nr telefonu'"
		:valInput="''"
		@sendValue="getData($event)"
	/>
	<FormsInput :name="'Temat'" :valInput="''" @sendValue="getData($event)" />
	<FormsInput
		:name="'Tresc wiadomosci'"
		:valInput="''"
		@sendValue="getData($event)"
	/>
</template>

<style scoped lang="scss"></style>
