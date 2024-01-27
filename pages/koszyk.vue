<script setup>
definePageMeta({
	layout: "second",
});

useHead({
	title: "Kompuland - Koszyk",
	meta: [{ name: "description", content: "moja stronka" }],
});
</script>

<template>
	<h1>Koszyk</h1>
	<h2>Twoje produkty w koszyku:</h2>
	<div class="columns" style="width: 100vw; text-align: center">
		<div class="column">
			<img src="./img/ip15.png" width="184" />
			<div><strong>iPhone 15 128GB Czarny</strong></div>
			<div>4 199,00 zł</div>
		</div>
		<div class="column">
			<img src="./img/s24.png" width="200" />
			<div><strong>Samsung Galaxy S24 256GB Szary</strong></div>
			<div>4 199,00 zł</div>
		</div>
		<div class="column">
			<img src="./img/ip15.png" width="184" />
			<div><strong>iPhone 15 256GB Czarny</strong></div>
			<div>4 799,00 zł</div>
		</div>
		<div class="column">
			<img src="./img/s24.png" width="200" />
			<div><strong>Samsung Galaxy S24 512GB Szary</strong></div>
			<div>4 999,00 zł</div>
		</div>
	</div>
	<button class="button is-medium is-link">Zamów i zapłać</button>
</template>
