<script setup>
definePageMeta({
	layout: "default",
});

useHead({
	title: "Kompuland - Laptopy i komputery",
	meta: [{ name: "description", content: "moja stronka" }],
});
</script>

<template>
	<h1>Laptopy i komputery</h1>
<h2>Polecamy:</h2>
	<div class="columns" style="width: 100vw; text-align: center">
		<div class="column">
			<img src="./img/mbp14.png" width="222" />
			<div><strong>MacBook Pro M3 18GB/512</strong></div>
			<div>11 499,00 zł</div>
		</div>
		<div class="column">
			<img src="./img/mb13.png" width="238" />
			<div><strong>MacBook Air M2 16GB/256</strong></div>
			<div>4 199,00 zł</div>
		</div>
		<div class="column">
			<img src="./img/mb13.png" width="238" />
			<div><strong>MacBook Air M2 16GB/512</strong></div>
			<div>4 699,00 zł</div>
		</div>
	</div>
	<hr>
	<h2>Kategorie:</h2>
	<div class="columns" style="width: 100vw; text-align: center">
		<div class="column">
			<img src="./img/mbp14.png" width="222" />
			<div><strong>Laptopy (1230)</strong></div>
			
		</div>
		<div class="column">
			<img src="./img/pc.png" width="272" />
			<div><strong>Komputery PC (469)</strong></div>
			
		</div>
		
	</div>
</template>
