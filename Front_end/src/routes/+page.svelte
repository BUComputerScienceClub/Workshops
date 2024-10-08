<script lang="ts">

import Text from "$lib/components/Text/Text.svelte";

const messages = [
    {message: "Hello there", sender: "Liam", time:"00:00:00"},
    {message: "Hey, how's it going?", sender: "Max",time:"00:00:10"},
    {message: "pretty good you !", sender: "Liam", time:"00:00:12"},
    {message: "Yeah doing good just trying to get this fkn box to go down and to fix this", sender: "Max",time:"00:01:11"},
    {message: "yeah ? How is that going ?", sender: "Liam",time:"00:01:15"},
    {message: "Hello there", sender: "Liam", time:"00:00:00"},
    {message: "Hey, how's it going?", sender: "Max",time:"00:00:10"},
    {message: "pretty good you !", sender: "Liam", time:"00:00:12"},
    {message: "Yeah doing good just trying to get this fkn box to go down and to fix this", sender: "Max",time:"00:01:11"},
    {message: "yeah ? How is that going ?", sender: "Liam",time:"00:01:15"},
    {message: "Hello there", sender: "Liam", time:"00:00:00"},
    {message: "Hey, how's it going?", sender: "Max",time:"00:00:10"},
    {message: "pretty good you !", sender: "Liam", time:"00:00:12"},
    {message: "Yeah doing good just trying to get this fkn box to go down and to fix this", sender: "Max",time:"00:01:11"},
    {message: "yeah ? How is that going ?", sender: "Liam",time:"00:01:15"},
    {message: "Hello there", sender: "Liam", time:"00:00:00"},
    {message: "Hey, how's it going?", sender: "Max",time:"00:00:10"},
    {message: "pretty good you !", sender: "Liam", time:"00:00:12"},
    {message: "Yeah doing good just trying to get this fkn box to go down and to fix this", sender: "Max",time:"00:01:11"},
    {message: "yeah ? How is that going ?", sender: "Liam",time:"00:01:15"},
    {message: "Hello there", sender: "Liam", time:"00:00:00"},
    {message: "Hey, how's it going?", sender: "Max",time:"00:00:10"},
    {message: "pretty good you !", sender: "Liam", time:"00:00:12"},
    {message: "Yeah doing good just trying to get this fkn box to go down and to fix this", sender: "Max",time:"00:01:11"},
    {message: "yeah ? How is that going ?", sender: "Liam",time:"00:01:15"},
    {message: "Hello there", sender: "Liam", time:"00:00:00"},
    {message: "Hey, how's it going?", sender: "Max",time:"00:00:10"},
    {message: "pretty good you !", sender: "Liam", time:"00:00:12"},
    {message: "Yeah doing good just trying to get this fkn box to go down and to fix this", sender: "Max",time:"00:01:11"},
    {message: "yeah ? How is that going ?", sender: "Liam",time:"00:01:15"},
    {message: "Hello there", sender: "Liam", time:"00:00:00"},
    {message: "Hey, how's it going?", sender: "Max",time:"00:00:10"},
    {message: "pretty good you !", sender: "Liam", time:"00:00:12"},
    {message: "Yeah doing good just trying to get this fkn box to go down and to fix this", sender: "Max",time:"00:01:11"},
    {message: "yeah ? How is that going ?", sender: "Liam",time:"00:01:15"},
    {message: "Hello there", sender: "Liam", time:"00:00:00"},
    {message: "Hey, how's it going?", sender: "Max",time:"00:00:10"},
    {message: "pretty good you !", sender: "Liam", time:"00:00:12"},
    {message: "Yeah doing good just trying to get this fkn box to go down and to fix this", sender: "Max",time:"00:01:11"},
    {message: "yeah ? How is that going ?", sender: "Liam",time:"00:01:15"},
    {message: "Hey ! you did it no ?", sender: "Masoud",time:"00:01:15"},
    {message: "yeah ! I did looks pretty good no !", sender: "Max",time:"00:01:15"},
    {message: "bit janky but it works", sender: "Liam",time:"00:01:15"},
    {message: "おやすみなさい", sender: "Max",time:"00:02:00"},
    {message: "wtf is that ?", sender: "Liam",time:"00:02:01"},
    {message: "bro wtf?", sender: "Masoud",time:"00:02:02"},
    {message: "why you gotta be weird like that ?", sender: "Liam",time:"00:02:02"},
    {message: "alright alright good night ", sender: "Max",time:"00:02:00"},

];

let fname: string = "Max"; /* To be defined for login */
let text: string ="";



</script>


{#each messages as text}
    <Text
            me="{fname}"
            message={text.message}
            sender={text.sender}
            time="{text.time}"
    />
{/each}


<style>
    :global(body) {
        margin: 0;
        padding: 0;
        padding-bottom: 75px;
        background-color: #232323;

    }

    input[type=text]{
        position: fixed;
        width:90%;
        color: black;
        bottom:35px;
        background-color: rgba(35,35,35,60%);
        border-style: solid;
        border-color: dimgray;
        border-width: 1px;
        border-radius: 10px;
        height: 20px;

        margin-right: 6%;
        margin-left: 4%;

        color:white;
    }
    .box {
        position: fixed;
        bottom: -15px;

        width: 100%;
        height: 75px;

        background-color: rgba(35,35,35,85%);

        backdrop-filter: blur(3px);

        border-radius: 15px;


    }
    .input-text{
        padding-left: 10px;
    }


</style>
<div class="box">

    <form>

        <input type="text" bind:value={text} class="input-text" placeholder="Input message : ">
    </form>
</div>





