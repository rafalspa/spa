<script setup>
const open = ref(false);
const toggle = () => (
	(open.value = !open.value),
	(textButton.value = open.value ? "Hide modal" : "Show modal")
);
const textButton = ref("Show modal");

useHead({
	title: "Kompuland - Strona główna",
	meta: [{ name: "description", content: "moja stronka" }],
});
</script>

<template>
	<h1>Polecamy</h1>
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
			<img src="./img/mb13.png" width="238" />
			<div><strong>MacBook Air M2 16GB/256</strong></div>
			<div>4 199,00 zł</div>
		</div>
		<div class="column">
			<img src="./img/ps5.png" width="230" />
			<div><strong>PlayStation 5 825GB</strong></div>
			<div>2 699,00 zł</div>
		</div>
	</div>
	<hr>
	<div class="columns" style="width: 100vw; text-align: center">
		<div class="column">
			
			<div><h2><strong>Codziennie losuj 3 zniżki</strong></h2></div>
			<img src="./img/box.png" width="230" />
			<div>W boxach znajdziesz produkty nawet za 1zł</div>
			<button class="button is-link is-medium" style="margin-top: 15px;">Losuj zniżki ></button>
		</div>
		<div class="column">
			<img src="./img/apple.png" width="300" />
			<div><strong>Sprawdź urządzenia Apple</strong></div>
			<div>i skorzystaj z wyjątkowych promocji</div>
		</div>
		<div class="column">
			<img src="./img/samsung.png" width="300" />
			<div><strong>Przedsprzedaż Samsung Galaxy S24</strong></div>
			<div>Zamów i zyskaj w odercie premierowej!</div>
		</div>
	</div>
</template>
