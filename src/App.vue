<template>
	<h1>{{ title }}</h1>
	<p>Welcome...</p>
	<!-- <Modal heading="Sign up for the Givaway!" text="Grab your ninja swag for half price!" /> -->
	<Modal :heading="heading" :text="text" theme="sal" />
</template>

<script>
import Modal from './components/Modal'

export default {
	name: 'App',
	components: { Modal },
	data() {
		return {
			title: 'My First Vue App!',
			heading: 'Sign up for the Givaway!',
			text: 'Grab your ninja swag for half price!',
		}
	},
}
</script>

<style>
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
h1 {
	border-bottom: 1px solid #ddd;
	display: inline-block;
	padding-bottom: 10px;
}
</style>
