<script lang="ts">
	let value: string | null = $state(null);
	let upper = $derived(value?.toUpperCase());
</script>

{value} becomes {upper}

<button onclick={() => value = 'foo'}>Foo</button>
<button onclick={() => value = 'bar'}>Bar</button>
