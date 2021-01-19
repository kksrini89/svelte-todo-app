<script>
	import TodoInput from './components/todo-input.svelte';
	import TodoList from './components/todo-list.svelte';
	let todos = [{
		name: 'ABC'
	}, {
		name: 'DEF'
	}]
</script>

<!-- <main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main> -->

<style>
* {
  box-sizing: border-box;
}

body {
  background-color: #242333;
  color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  padding: 25%;
}

.container .title {
  text-align: center;
  margin-bottom: 25px;
}
</style>

<body><div class="container">
	<div class="title">TODO APP</div>
	<TodoInput	/>
	<TodoList todos={todos}/>
</div>
</body>