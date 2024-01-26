<script setup>
definePageMeta({
	layout: "default",
});

useHead({
	title: "Kompuland - Podzespoły komputerowe",
	meta: [{ name: "description", content: "moja stronka" }],
});
</script>

<template>
	<h1>Podzespoły komputerowe</h1>
<h2>Polecamy:</h2>
	<div class="columns" style="width: 100vw; text-align: center">
		<div class="column">
			<img src="./img/i9.png" width="184" />
			<div><strong>Intel Core i9-14900KF</strong></div>
			<div>2 579,00 zł</div>
		</div>
		<div class="column">
			<img src="./img/rx.png" width="200" />
			<div><strong>AMD Radeon RX 6950 XT 16GB GDDR6</strong></div>
			<div>2 749,00 zł</div>
		</div>
		<div class="column">
			<img src="./img/s2tb.png" width="200" />
			<div><strong>Samsung 2TB M.2 PCIe Gen4 NVMe 980 PRO</strong></div>
			<div>699,00 zł</div>
		</div>
		<div class="column">
			<img src="./img/mobo.png" width="160" />
			<div><strong>MSI B550-A PRO</strong></div>
			<div>469,00 zł</div>
		</div>
	</div>
	<hr />
    <h2>Kategorie:</h2>
	<div class="columns" style="width: 100vw; text-align: center">
		<div class="column">
			<img src="./img/i9.png" width="184" />
			<div><strong>Procesory (148)</strong></div>
		</div>
		<div class="column">
			<img src="./img/rx.png" width="200" />
			<div><strong>Karty graficzne (397)</strong></div>
		</div>
		<div class="column">
			<img src="./img/s2tb.png" width="200" />
			<div><strong>Dyski twarde SSD i HDD (1198)</strong></div>
		</div>
		<div class="column">
			<img src="./img/mobo.png" width="160" />
			<div><strong>Płyty główne (282)</strong></div>
		</div>
	</div>
</template>
