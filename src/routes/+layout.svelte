<script>
	import { isJsxChild } from 'typescript';
import Header from './Header.svelte';
	import './layout.css';

	/** @type {{children: import('svelte').Snippet}} */
	let { children } = $props();
</script>


{@render children()}

<footer>
	<p>polimi 2026</p>
</footer>

<style>
	:global(p) {
	color: deeppink;
	}
</style>
