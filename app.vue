<script setup>
const open2 = ref(false);
const toggle2 = () => (
	(open2.value = !open2.value),
	(textButton2.value = open2.value ? "Hide modal" : "Show modal")
);
const textButton2 = ref("Show modal");
</script>

<template>
	<div>
		<NuxtLayout>
			<div class="body-content"><NuxtPage /></div>
			<div v-if="open">to jest ukryty tekst</div>
			<div v-if="open2" class="okienko">
				Wyślij nam wiadomość
				<button @click="toggle2" class="zamknij">X</button>
				<div class="zawartosc">
					<!-- avatar na czacie-->
					<svg
						xmlns="http://www.w3.org/2000/svg"
						class="icon icon-tabler icon-tabler-user-circle"
						width="52"
						height="52"
						viewBox="0 0 24 24"
						stroke-width="2"
						stroke="#000000"
						fill="none"
						stroke-linecap="round"
						stroke-linejoin="round"
					>
						<path stroke="none" d="M0 0h24v24H0z" fill="none" />
						<path d="M12 12m-9 0a9 9 0 1 0 18 0a9 9 0 1 0 -18 0" />
						<path d="M12 10m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0" />
						<path
							d="M6.168 18.849a4 4 0 0 1 3.832 -2.849h4a4 4 0 0 1 3.834 2.855"
						/>
					</svg>
					<div class="wiadomosc">
						Witaj! Jestem botem Kompuland 🤖👋 Jak mogę Ci pomóc?
					</div>
					<div class="data">09:18</div>
				</div>

				<input type="text" class="chat" placeholder="Napisz wiadomość..." />

				<!-- przycisk wyslij-->
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="icon icon-tabler icon-tabler-send-2 wyslij"
					width="52"
					height="52"
					viewBox="0 0 24 24"
					stroke-width="2"
					stroke="#000000"
					fill="none"
					stroke-linecap="round"
					stroke-linejoin="round"
				>
					<path stroke="none" d="M0 0h24v24H0z" fill="none" />
					<path
						d="M4.698 4.034l16.302 7.966l-16.302 7.966a.503 .503 0 0 1 -.546 -.124a.555 .555 0 0 1 -.12 -.568l2.468 -7.274l-2.468 -7.274a.555 .555 0 0 1 .12 -.568a.503 .503 0 0 1 .546 -.124z"
					/>
					<path d="M6.5 12h14.5" />
				</svg>
			</div>
			<div class="kolko" @click="toggle2">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="icon icon-tabler icon-tabler-message-circle"
					width="64"
					height="64"
					viewBox="1 2 22 22"
					stroke-width="2"
					stroke="#ffffff"
					fill="none"
					stroke-linecap="round"
					stroke-linejoin="round"
				>
					<path stroke="none" d="M0 0h24v24H0z" fill="none" />
					<path
						d="M3 20l1.3 -3.9c-2.324 -3.437 -1.426 -7.872 2.1 -10.374c3.526 -2.501 8.59 -2.296 11.845 .48c3.255 2.777 3.695 7.266 1.029 10.501c-2.666 3.235 -7.615 4.215 -11.574 2.293l-4.7 1"
					/>
				</svg>
			</div>
		</NuxtLayout>
	</div>
</template>
