<script>

</script>

<template>
<div>
<h2>Login</h2>
<form v-on:submit="login">
<input type="text" placeholder="Enter your email" name="email" /><br>
<input type="password" placeholder="Emter your password" name="password" /><br>
<input type="submit" value="Login"/>
</form>
</div>
</template>