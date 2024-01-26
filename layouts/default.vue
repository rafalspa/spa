<template>
	<div>
		<TopNav />
		<div style="width: 100vw">
			<div style="display: flex; gap: 10px; width: 70%; margin: auto auto">
				<input
					class="input is-normal"
					type="text"
					placeholder="Czego szukasz?"
				/>
				<button class="button is-link">Szukaj</button>
			</div>
		</div>
		<slot />

		<div class="stopka">
			Kompuland | Projekt WSB 2024 | by <strong>Rafał Spaleniak</strong> | logo
			by app.logo.com
		</div>
	</div>
</template>
