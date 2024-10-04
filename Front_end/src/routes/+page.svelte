<script lang="ts">

import Text from "$lib/components/Text/Text.svelte";

const messages = [
    {message: "Hello there", sender: "Liam"},
    {message: "Hey, how's it going?", sender: "Max"},
    {message: "Not much guys!", sender: "Masoud"},
];


</script>


{#each messages as text}
    <Text
            message={text.message}
            sender={text.sender}
    />
{/each}


<style>
    :global(body) {
        margin: 0;
        padding: 0;
    }
</style>