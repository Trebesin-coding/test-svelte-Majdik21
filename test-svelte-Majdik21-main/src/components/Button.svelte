<script>
    import { pocitadlo } from '$lib/shared.svelte'

    let { message } = $props()

    function increment(){
        pocitadlo++
    }

</script>

<div>
    <button onclick={increment}>{message}</button>
</div>

