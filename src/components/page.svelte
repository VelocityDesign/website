<script lang="ts">
	import Cover from '../components/cover.svelte';
	import Bar from '../components/bar.svelte';
	import Footer from '../components/footer.svelte';
	export let pageTitle: string;
</script>

<Bar />

<div id = "content">
    <slot name="cover">
        <Cover title={pageTitle} />
    </slot>

    <slot name="content" />

    <Footer />
</div>