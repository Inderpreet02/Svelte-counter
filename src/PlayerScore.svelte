<script>
    export let playerName;
    let playerScore = 0;
  
    function increasePlayer1Score(){
        playerScore++;
    }

    export function resetTheScore(){
        playerScore = 0;
    };
  
  </script>

<div class="yes">
    
    <h1>{playerName}</h1>
    <h2>{playerScore}</h2>
    <button on:click={increasePlayer1Score}>
        Up
    </button>
    <button on:click={() => playerScore--}>
        down
    </button>

</div>

<style>
    .yes{
        flex: 1;
    }
</style>