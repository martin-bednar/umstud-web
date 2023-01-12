<ul id="links">
	<li>
		<a href="/press">
			<span>Press</span>
		</a>
	</li>
	<li>
		<a href="/about">
			<span>Abouth</span>
		</a>
	</li>
</ul>

<style>
	ul {
		list-style-type: none;
		display: flex;
		margin: 0;
		padding: 0;
		height: 100%;
		align-items: center;
		justify-content: flex-start;
		margin-right: 10px;
	}
	li {
		display: flex;
		height: 100%;
		width: 10em;
		align-items: center;
		justify-content: center;
		padding-left: 0.5em;
		padding-right: 0.5em;
	}
	li:not(:last-child) {
		border: 1px solid black;
	}
	a {
		display: flex;
		align-items: center;
		justify-content: center;
		text-decoration: none;
		color: inherit;
		text-transform: uppercase;
		border: 1px solid black;
		border-radius: 50%;
		width: 70px;
		height: 70px;
		text-align: center;
		transition: all 500ms ease;
	}
	a:hover {
		background-color: black;
		color: white;
	}
</style>
