<script>
import Movie from './movie-child.svelte'
	let moviesList = [
    { id: 1, name: "The Shawshank Redemption" },
    { id: 2, name: "The Godfather" },
    { id: 3, name: "The Dark Knight" },
    { id: 4, name: "12 Angry Men" },
    { id: 5, name: "Schindler List" },
  ];
  let disabled = false
  function deleteEntry() {

if(moviesList.length) {

    moviesList.shift();

    moviesList = moviesList;

}

else {

    disabled = true;

}

}
</script>

<div>
    <h6>Use of Loop: Top 5 Movies.</h6>
    <button disabled = {disabled} on:click = {deleteEntry}>delete</button>
    {#each moviesList as movie}

        <Movie movie = {movie}/>

    {/each}
</div>
