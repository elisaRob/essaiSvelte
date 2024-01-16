<script>
  let count = 0
  let string;
  let string2;

   $ : {
     string = `You have clicked ${count} times`
   }

   $ : string2 = `You have ${count} times`

  function increment(){
    count+=1
  }
</script>

<button on:click={increment}>Clicks {count}</button>
<h3>{string}</h3>
<h3>{string2}</h3>
<h3>You have clicked {count} times</h3>

<style>
  button{
    padding:15px 20px;
    cursor:pointer
  }
</style>