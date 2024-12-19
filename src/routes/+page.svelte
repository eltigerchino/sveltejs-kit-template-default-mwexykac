<script>
	import { enhance } from '$app/forms'
</script>

<form method="post" action="/somewhere" use:enhance>
  This form utilises use:enhance with a generic POST endpoint
	<button>Click me!</button>
</form>

<a href="/out_there"> Also click me!</a>