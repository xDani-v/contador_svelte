<script>
	let cursos = ['html','css','html'];
	let numeros = [2,3];
	const agg_numero  = () =>{
		let num = Math.floor(Math.random() * (20 - 1)) + 1;
		numeros = [...numeros,num];
	}
</script>

<main class="container">
	<h1>Cursos</h1>
	<ul>
		{#each cursos as curso, index}
			<li>{index + 1}. {curso}</li>
		{/each}
	</ul>
	<button on:click={agg_numero} class="btn btn-primary">Agregar numero</button>
	<ul>
		{#each numeros as numero}
			 <li>{numero}</li>
		{/each}
	</ul>
</main>

