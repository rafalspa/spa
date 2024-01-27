<template>
	<div>
		<TopNav />
		<div style="width: 100vw">
			<div class="szukajka">
				<input
					class="input is-normal"
					type="text"
					placeholder="Czego szukasz?"
				/>
				<button class="button is-link"><svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-search" width="52" height="52" viewBox="0 0 24 24" stroke-width="2" stroke="#ffffff" fill="none" stroke-linecap="round" stroke-linejoin="round">
  <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
  <path d="M10 10m-7 0a7 7 0 1 0 14 0a7 7 0 1 0 -14 0" />
  <path d="M21 21l-6 -6" />
</svg></button>
			</div>
		</div>
		<slot />

		<div class="stopka">
			Kompuland | Projekt WSB 2024 | by <strong>Rafał Spaleniak</strong>
		</div>
	</div>
</template>
