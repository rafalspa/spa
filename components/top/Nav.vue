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
		<div v-if="open" class="mobilnemenu">
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
				<li>
					<NuxtLink to="/kontakt">Kontakt</NuxtLink>
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
						<a class="navbar-item" href="/laptopy-i-komputery">
							Laptopy/notebooki/ultrabooki
						</a>
						<a class="navbar-item" href="/laptopy-i-komputery">
							Laptopy 2 w 1
						</a>
						<a class="navbar-item" href="/laptopy-i-komputery">
							Laptopy gamingowe
						</a>
						<hr class="navbar-divider" />
						<a class="navbar-item" href="/laptopy-i-komputery">
							Komputery PC
						</a>
						<a class="navbar-item" href="/laptopy-i-komputery">
							Komputery gamingowe
						</a>
						<a class="navbar-item" href="/laptopy-i-komputery">
							Komputery all-in-one
						</a>
					</div>
				</div>

				<div class="navbar-item has-dropdown is-hoverable">
					<a class="navbar-link" href="/smartfony-i-telefony">
						Smartfony i telefony
					</a>

					<div class="navbar-dropdown">
						<a class="navbar-item" href="/smartfony-i-telefony"> Apple </a>
						<a class="navbar-item" href="/smartfony-i-telefony"> Samsung </a>
						<a class="navbar-item" href="/smartfony-i-telefony"> Xiaomi </a>
						<a class="navbar-item" href="/smartfony-i-telefony"> OnePlus </a>
						<hr class="navbar-divider" />
						<a class="navbar-item" href="/smartfony-i-telefony">
							Telefony komórkowe
						</a>
					</div>
				</div>

				<div class="navbar-item has-dropdown is-hoverable">
					<a class="navbar-link" href="/podzespoly-komputerowe">
						Podzespoły komputerowe
					</a>

					<div class="navbar-dropdown">
						<a class="navbar-item" href="/podzespoly-komputerowe">
							Procesory
						</a>
						<a class="navbar-item" href="/podzespoly-komputerowe">
							Karty graficzne
						</a>
						<a class="navbar-item" href="/podzespoly-komputerowe">
							Płyty główne
						</a>
						<a class="navbar-item" href="/podzespoly-komputerowe">
							Pamięci RAM
						</a>
						<a class="navbar-item" href="/podzespoly-komputerowe">
							Dyski twarde SSD i HDD
						</a>
						<a class="navbar-item" href="/podzespoly-komputerowe">
							Zasilacze
						</a>
					</div>
				</div>

				<div class="navbar-item is-hoverable">
					<a class="navbar-item" href="/kontakt"> Kontakt </a>
				</div>
			</div>

			<div class="navbar-end">
				<div class="navbar-item">
					<div class="buttons">
						<button class="button is-info is-light">Twoje konto</button>
						<a href="/koszyk"
							><button class="button is-info is-light">Koszyk</button></a
						>
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
