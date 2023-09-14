<script>
    export let data
</script>

<!-- <h1>{data.title}</h1> -->

<!-- <pre>
    {JSON.stringify(data,null, 2)}
</pre> -->

<main>
	<div class="card-container">
		<span class="pro">{data.label}</span>
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<img class="round" src="{ data.zenit.url }" width="100px" height="100px" alt="photo"/>
		<h3>{data.title}</h3>
		<p>{ data.bio[0].text }<br/></p>
        <h4>{data.locatie}</h4>
		<div class="buttons">
			<button class="primary">{data.message}</button>
			<button class="primary ghost"> {data.follow}</button>
		</div>
		<div class="skills">
			<h4>{data.skill}</h4>
			<ul>
				<li>{ data.skills[0].text}</li>
			</ul>
		</div>
	</div>
</main>