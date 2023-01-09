<script>
    let user = {
        username: '',
        password: ''
    };


    function handleForm() {
        console.log(user);
    }

    import { fetch } from 'svelte/fetch';

let email = '';
let password = '';

async function login() {
  const res = await fetch('/login', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ email, password }),
  });
  const data = await res.json();
  if (data.success) {
    // redirect to another page or show a success message
  } else {
    // show an error message
  }
}
</script>


<form on:submit|preventDefault={login}  class="formcenter" action="/login" method="post">
    <h2 class="login jp">ログイン
    </h2>
    <div >
        <input autocomplete="off" class="email jp"  id="username" name="username" placeholder="Username" type="text" bind:value={user.username}>
    </div>
    <div >
        <input autocomplete="off" class="email jp"  id="password" name="password" placeholder="Password" type="password" bind:value={user.password}>
    </div>
    <button class="btn-primary jp"  type="submit" disabled={!user.password|user.username}>ログイン</button>
  </form>