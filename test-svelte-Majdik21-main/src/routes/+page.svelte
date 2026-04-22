<script>
    import Button from '../components/Button.svelte'
	import ButtonE from '../components/ButtonE.svelte';
// Až vytvoříš komponent, nezapomeň jej importovat
// Emoji se vytváří pomocí windows + . nebo je můžeš zkopírovat odsud 🙂 😢
</script>

<div class="headings">
    <!-- Sem patří komponenty s nadpisy -->
    <Heading headingText={"svelte"} />
    <Heading headingText={"je"} />
    <Heading headingText={"brnkacka"} />
</div>

<div class="container">
    <p>počet kliknutí: {pocitadlo}</p>
    <div class="buttons">
        <!-- Sem patří komponenty s tlačítky -->
        <Button message={"+"} />
        <ButtonE message={"🙂"} />
    </div>
</div>








<style>

    /* CSS není potřeba upravovat */

* {
    font-family: monospace;
}

.container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    gap: 10px;
}

.container > p {
    font-size: 2em;
}

.buttons > button{
    border: 1px solid black;
    border-radius: 50000px;
    padding: 10px 20px;
    background-color: lightblue;
    font-size: 1.5em;
}

.buttons > button:nth-of-type(1) {
    background-color: lightblue;
}

.buttons > button:nth-of-type(2) {
    background-color: lightcoral;
}

.headings {
    position: absolute;
}

:global(.headings > h2) {
	position: absolute;
    font-size: 3em;

}

:global(.headings > h2:nth-child(1)) {
	left: 300px;
	top: 50px;
}

:global(.headings > h2:nth-child(2)) {
	left: 200px;
	top: 200px;
}

:global(.headings > h2:nth-child(3)) {
	left: 300px;
	top: 350px;
}


</style>