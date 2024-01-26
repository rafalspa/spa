<script setup>
const name = ref("Nawigacja");

const open = ref(false);
const toggle = () => (open.value = !open.value);

useHead({
	title: "Strona glowna",
	meta: [{ name: "description", content: "moja stronka" }],
});
</script>
<template>
	<nav class="navbar" role="navigation" aria-label="main navigation">
		<div class="navbar-brand">
			<a class="navbar-item" href="./">
				<img src="./img/logo.png" width="112" height="28" />
			</a>

			<a
				role="button"
				class="navbar-burger"
				aria-label="menu"
				aria-expanded="false"
				data-target="navbarBasicExample"
				@click="toggle"
			>
				<span aria-hidden="true"></span>
				<span aria-hidden="true"></span>
				<span aria-hidden="true"></span>
			</a>
		</div>

		<!-- Menu dla mobilnego rozmiaru po nacisnieciu burgera -->
		<div v-if="open">
			<ul>
				<li>
					<NuxtLink to="/twoje-konto">Twoje konto</NuxtLink>
				</li>
				<li>
					<NuxtLink to="/koszyk">Koszyk</NuxtLink>
				</li>
				<li>
					<NuxtLink to="/laptopy-i-komputery">Laptopy i komputery</NuxtLink>
				</li>
				<li>
					<NuxtLink to="/smartfony-i-telefony">Smartfony i telefony</NuxtLink>
				</li>
				<li>
					<NuxtLink to="/podzespoly-komputerowe"
						>Podzespoły komputerowe</NuxtLink
					>
				</li>
			</ul>
		</div>

		<!-- Menu dla desktopowego rozmiaru -->
		<div id="navbarBasicExample" class="navbar-menu">
			<div class="navbar-start">
				<div class="navbar-item has-dropdown is-hoverable">
					<a class="navbar-link" href="/laptopy-i-komputery">
						Laptopy i komputery
					</a>

					<div class="navbar-dropdown">
						<a class="navbar-item"> Laptopy/notebooki/ultrabooki </a>
						<a class="navbar-item"> Laptopy 2 w 1 </a>
						<a class="navbar-item"> Laptopy gamingowe </a>
						<hr class="navbar-divider" />
						<a class="navbar-item"> Komputery PC </a>
						<a class="navbar-item"> Komputery gamingowe </a>
						<a class="navbar-item"> Komputery all-in-one </a>
					</div>
				</div>

				<div class="navbar-item has-dropdown is-hoverable">
					<a class="navbar-link" href="/smartfony-i-telefony">
						Smartfony i telefony
					</a>

					<div class="navbar-dropdown">
						<a class="navbar-item"> Apple </a>
						<a class="navbar-item"> Samsung </a>
						<a class="navbar-item"> Xiaomi </a>
						<a class="navbar-item"> OnePlus </a>
						<hr class="navbar-divider" />
						<a class="navbar-item"> Telefony komórkowe </a>
					</div>
				</div>

				<div class="navbar-item has-dropdown is-hoverable">
					<a class="navbar-link" href="/podzespoly-komputerowe">
						Podzespoły komputerowe
					</a>

					<div class="navbar-dropdown">
						<a class="navbar-item"> Procesory </a>
						<a class="navbar-item"> Karty graficzne </a>
						<a class="navbar-item"> Płyty główne </a>
						<a class="navbar-item"> Pamięci RAM </a>
						<a class="navbar-item"> Dyski twarde SSD i HDD </a>
						<a class="navbar-item"> Zasilacze </a>
					</div>
				</div>
			</div>

			<div class="navbar-end">
				<div class="navbar-item">
					<div class="buttons">
						<button class="button is-info is-light">Twoje konto</button>
						<button class="button is-info is-light">Koszyk</button>
					</div>
				</div>
			</div>
		</div>
	</nav>
</template>
<style scoped lang="scss">
h1 {
	color: violet;
}

ul {
	.mpa {
		color: yellow;
	}
}
</style>
