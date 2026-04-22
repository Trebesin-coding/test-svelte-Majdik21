<script>
    import { pocitadlo } from '$lib/shared.svelte'

    let { message } = $props()

    function increment(){
            message = "😢"
            pocitadlo++
    }
    function decrease(){
            message = "🙂"
            pocitadlo--
    }
       
        

</script>
<div>
    {#if message === "🙂"}
        <button onclick={increment}>{message}</button>
    {:else if message === "😢"}
        <button onclick={decrease}>{message}</button>
    {/if}
</div>

