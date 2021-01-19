<script>
export let todos = [];
</script>

<style>
/*  Todo list */

/* .container .toto-list {
} */

.container .toto-list ul.list-unstyled {
  list-style-type: none;
  margin-left: -10%;
}

.container .toto-list ul.list-unstyled li {
  margin: 15px;
  padding: 10px;
  border: 1px solid;
}

.container .toto-list ul.list-unstyled li .list-item {
  display: flex;
  justify-content: space-between;
}

</style>

  <div class="toto-list">
    <ul class="list-unstyled">
      {#each todos as todo, index}
      <li>
        <div class="list-item">
          <span class="text">{todo.name}</span>
          <span class="remove">X</span>
        </div>
      </li>  
      {/each}
      <!-- <li>
        <div class="list-item">
          <span class="text">ABC</span>
          <span class="remove">X</span>
        </div>
      </li>
      <li>
        <div class="list-item">
          <span class="text">DEF</span>
          <span class="remove">X</span>
        </div>
      </li>
      <li>
        <div class="list-item">
          <span class="text">GHI</span>
          <span class="remove">X</span>
        </div>
      </li> -->
    </ul>
  </div>