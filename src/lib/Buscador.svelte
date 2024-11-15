<script>

let search = ""; 
const items = ['manzana', 'potato', 'martin', 'naranja'];

function filterItems(){
    return items.filter(item=>
        item.toLowerCase().includes(search.toLowerCase())
    );
}
</script>

<p>BUSCADOR</p>
<div class="container">
<input type="text" bind:value={search}>



<ul>
    {#each filterItems() as item}
    <li>{item}</li>
    {/each}
</ul>

</div>