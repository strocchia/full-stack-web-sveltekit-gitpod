<div class="todo done">
	<form class="done toggle" action="" method="">
		<input type="hidden" name="done" value="" />
		<button class="toggle" aria-label="Done or not ... that is the question (?)">Done</button>
	</form>

	<form class="text" action="" method="">
		<input type="text" />
		<button class="save" aria-label="Save after edits">Sav</button>
	</form>

	<form action="" method="">
		<button class="delete" aria-label="Delete me">X</button>
	</form>
</div>

<style>
	.todo {
		display: grid;
		grid-template-columns: 2rem 1fr 2rem;
		grid-gap: 0.5rem;
		align-items: center;
		margin: 0 0 0.5rem 0;
		padding: 0.5rem;
		background-color: white;
		border-radius: 8px;
		filter: drop-shadow(2px 4px 6px rgba(0, 0, 0, 0.1));
		transform: translate(-1px, -1px);
		transition: filter 0.2s, transform 0.2s;
	}

	.todo input {
		flex: 1;
		padding: 0.5em;
		border-radius: 3px;
	}

	.todo button {
		width: 2em;
		height: 2em;
		border: none;
		background-color: transparent;
		background-position: 50% 50%;
		background-repeat: no-repeat;
	}

	/* button.toggle {
		border: 1px solid rgba(0, 0, 0, 0.2);
		border-radius: 50%;
		box-sizing: border-box;
		background-size: 1em auto;
	} */

	.text {
		display: flex;
		position: relative;
		flex: 1;
		align-items: center;
	}

	.save {
		position: absolute;
		right: 2%;
		opacity: 0;
		/* background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' viewBox='0 0 24 24'%3E%3Cpath d='M14 3h2.997v5h-2.997v-5zm9 1v20h-22v-24h17.997l4.003 4zm-17 5h12v-7h-12v7zm14 4h-16v9h16v-9z'/%3E%3C/svg%3E"); */
	}

	.todo input:focus + .save,
	.save:focus {
		transition: opacity 0.5s;
		opacity: 1;
	}

	.delete {
		opacity: 0.2;
		/* background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='currentColor' class='bi bi-trash' viewBox='0 0 24 24'%3E%3Cpath d='M5.5 5.5A.5.5 0 0 1 6 6v6a.5.5 0 0 1-1 0V6a.5.5 0 0 1 .5-.5zm2.5 0a.5.5 0 0 1 .5.5v6a.5.5 0 0 1-1 0V6a.5.5 0 0 1 .5-.5zm3 .5a.5.5 0 0 0-1 0v6a.5.5 0 0 0 1 0V6z'/%3E%3Cpath fill-rule='evenodd' d='M14.5 3a1 1 0 0 1-1 1H13v9a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V4h-.5a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1H6a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1h3.5a1 1 0 0 1 1 1v1zM4.118 4 4 4.059V13a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1V4.059L11.882 4H4.118zM2.5 3V2h11v1h-11z'/%3E%3C/svg%3E"); */
	}

	.delete:hover {
		transition: opacity 0.5s;
		opacity: 1;
	}

	/* .done {
		transform: none;
		opacity: 0.4;
	}

	.done .toggle {
		background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' viewBox='0 0 24 24'%3E%3Cpath d='M21.856 10.303c.086.554.144 1.118.144 1.697 0 6.075-4.925 11-11 11s-11-4.925-11-11 4.925-11 11-11c2.347 0 4.518.741 6.304 1.993l-1.422 1.457c-1.408-.913-3.082-1.45-4.882-1.45-4.962 0-9 4.038-9 9s4.038 9 9 9c4.894 0 8.879-3.928 8.99-8.795l1.866-1.902zm-.952-8.136l-9.404 9.639-3.843-3.614-3.095 3.098 6.938 6.71 12.5-12.737-3.096-3.096z'/%3E%3C/svg%3E");
	} */
</style>
