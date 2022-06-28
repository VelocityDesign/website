<script lang="ts">
    import Cover from "../components/cover.svelte"
    export let pageTitle: string;
</script>
<slot name="cover">
    <Cover title="{pageTitle}" />
</slot>