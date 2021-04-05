<script lang="ts">
	import Auth from "./auth/Auth.svelte";
	import firebase from "firebase/app";
	import * as creds from "../creds.json";
	import Menu from "./menu/Menu.svelte";

	firebase.initializeApp(creds);

</script>

<main>
	<Menu/>
	<Auth/>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
