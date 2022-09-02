<script>
  import PlayerScore from "./PlayerScore.svelte";

  let player1Component;
  let player2Component;

  function reset(){
    player1Component.resetTheScore();
    player2Component.resetTheScore();
  }

</script>

<main>

  <PlayerScore bind:this={player1Component} playerName="Player 1"/>
  <PlayerScore bind:this={player2Component} playerName="Player 2"/>
  <button on:click={reset} class="contrast outline">RESET</button>
  
</main>

<style>
  main{
    width: 100%;
  }
</style>
