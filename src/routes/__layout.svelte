<script lang="ts">
	import '../app.css';

	let showMobile = false;
</script>

<nav class="bg-stone-500">
	<div class="px-8 lg:max-w-6xl mx-auto">
		<div class="flex justify-between">
			<div class="flex space-x-4">
				<!-- Logo -->
				<div>
					<a href="/" class="flex items-center py-5 px-2 text-stone-700 hover:text-stone-900"
						><svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-6 w-6 mr-1"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M8 14v3m4-3v3m4-3v3M3 21h18M3 10h18M3 7l9-4 9 4M4 10h16v11H4V10z"
							/>
						</svg>
						<span class="font-bold">Lex Arcana</span>
					</a>
				</div>

				<!-- primary nav -->
				<div class="hidden md:flex items-center space-x-1">
					<div class="float-left overflow-hidden">
						<a class="py-5 px-3 text-stone-700 hover:text-stone-900 peer" href="/custodes">
							Custodes
						</a>
						<div
							class="hidden hover:flex peer-hover:flex absolute space-x-4 py-5 px-3 bg-stone-500 text-stone-700 w-auto items-center"
						>
							<a class="float-left hover:text-stone-900" href="/custodes/hintergrund">
								Hintergrund
							</a>
							<a class="float-left hover:text-stone-900" href="/custodes/officium">Officium</a>
							<a class="float-left hover:text-stone-900" href="/custodes/attribute">Attribute</a>
							<a class="float-left hover:text-stone-900" href="/custodes/lebenspunkte">
								Lebenspunkte
							</a>
							<a class="float-left hover:text-stone-900" href="/custodes/ausruestung">Ausrüstung</a>
						</div>
					</div>
					<a class="py-5 px-3 text-stone-700 hover:text-stone-900 peer" href="/spielablauf">
						Spielablauf
					</a>
					<a class="py-5 px-3 text-stone-700 hover:text-stone-900 peer" href="/kampf">Kampf</a>
					<a class="py-5 px-3 text-stone-700 hover:text-stone-900 peer" href="/roemische_magie">
						Römische Magie
					</a>
					<a
						class="py-5 px-3 text-stone-700 hover:text-stone-900 peer"
						href="/der_wille_der_goetter"
					>
						Der Wille der Götter
					</a>
					<div class="float-left overflow-hidden">
						<a class="py-5 px-3 text-stone-700 hover:text-stone-900 peer" href="/charaktere">
							Charaktere
						</a>
						<div
							class="hidden hover:flex peer-hover:flex absolute space-x-4  py-5 px-3 bg-stone-500 text-stone-700 w-auto items-center"
						>
							<a class="float-left hover:text-stone-900" href="/charaktere/aulus_antilochus">
								Aulus Antilochus
							</a>
							<a class="float-left hover:text-stone-900" href="/charaktere/elektra_ziais">
								Elektra Ziais
							</a>
							<a class="float-left hover:text-stone-900" href="/charaktere/gaius_valerius">
								Gaius Valerius
							</a>
							<a class="float-left hover:text-stone-900" href="/charaktere/pendaran_mab_elad">
								Pendaran mab Elad
							</a>
							<a class="float-left hover:text-stone-900" href="/charaktere/zenobia_euergetes">
								Zenobia Euergetes
							</a>
						</div>
					</div>
					<a class="py-5 px-3 text-stone-700 hover:text-stone-900 peer" href="/impressum">
						Impressum
					</a>
				</div>
			</div>

			<!-- mobile button goes here -->
			<div class="md:hidden flex items-center">
				<button class="mobile-menu-button" on:click={() => (showMobile = !showMobile)}>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						class="h-6 w-6"
						fill="none"
						viewBox="0 0 24 24"
						stroke="currentColor"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M4 6h16M4 12h16M4 18h16"
						/>
					</svg>
				</button>
			</div>
		</div>
	</div>

	<!-- mobile menu -->
	{#if showMobile}
		<div class="md:hidden">
			<a href="/custodes" class="block py-2 px-4 text-sm hover:text-stone-900 font-bold">
				Custodes</a
			>
			<a href="/custodes/hintergrund" class="block py-2 pl-8 text-sm hover:text-stone-900">
				Hintergrund
			</a>
			<a href="/custodes/officium" class="block py-2 pl-8 text-sm hover:text-stone-900">Officium</a>
			<a href="/custodes/attribute" class="block py-2  pl-8 text-sm hover:text-stone-900">
				Attribute
			</a>
			<a href="/custodes/lebenspunkte" class="block py-2  pl-8 text-sm hover:text-stone-900">
				Lebenspunkte
			</a>
			<a href="/custodes/ausruestung" class="block py-2  pl-8 text-sm hover:text-stone-900">
				Ausrüstung
			</a>
			<div class="w-full mb-4">
				<div class="h-1 mx-auto bg-white w-1/6 opacity-25 my-0 py-0 rounded-t" />
			</div>
			<a href="/spielablauf" class="block py-2 px-4 text-sm hover:text-stone-900">Spielablauf</a>
			<a href="/kampf" class="block py-2 px-4 text-sm hover:text-stone-900">Kampf</a>
			<a href="/roemische_magie" class="block py-2 px-4 text-sm hover:text-stone-900">
				Römische Magie
			</a>
			<a href="/der_wille_der_goetter" class="block py-2 px-4 text-sm hover:text-stone-900">
				Der Wille der Götter
			</a>
			<div class="w-full mb-4">
				<div class="h-1 mx-auto bg-white w-1/6 opacity-25 my-0 py-0 rounded-t" />
			</div>
			<a href="/charaktere" class="block py-2 px-4 text-sm hover:text-stone-900 font-bold">
				Charaktere
			</a>
			<a href="/charaktere/aulus_antilochus" class="block py-2 pl-8 text-sm hover:text-stone-900">
				Aulus Antilochus
			</a>
			<a href="/charaktere/elektra_ziais" class="block py-2 pl-8 text-sm hover:text-stone-900">
				Elektra Ziais
			</a>
			<a href="/charaktere/gaius_valerius" class="block py-2 pl-8 text-sm hover:text-stone-900">
				Gaius Valerius
			</a>
			<a href="/charaktere/pendaran_mab_elad" class="block py-2 pl-8 text-sm hover:text-stone-900">
				Pendaran mab Elad
			</a>
			<a href="/charaktere/zenobia_euergetes" class="block py-2 pl-8 text-sm hover:text-stone-900">
				Zenobia Euergetes
			</a>
			<div class="w-full mb-4">
				<div class="h-1 mx-auto bg-white w-1/6 opacity-25 my-0 py-0 rounded-t" />
			</div>
			<a href="/impressum" class="block py-2 px-4 text-sm hover:text-stone-900">Imressum</a>
		</div>
	{/if}
</nav>

<slot />
