<script>
    import { pocitadlo } from '$lib/shared.svelte'
    let { headingText } = $props()
</script>
<div>

    {#if pocitadlo > 5}
        <h2>{headingText}</h2>
    {/if}
    
</div>