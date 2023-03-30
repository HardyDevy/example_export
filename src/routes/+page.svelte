<!-- The problem is with the way I am exporting the value, not sure what. It could be because it is null at start? -->

<script>
  export const search = document.getElementById('searching').value; //Problem Line

  let srch = "";

  const handleInput = (e) => {
   srch = e.target.value;
  };

</script>

<h1>Trying to get thing export working</h1>
<p>Right now the search is: {srch}!</p>

<input type="text" id="searching" on:input={handleInput} placeholder="Search for a Character...">
