<template>
	<div>
		<Header :links="menuLinks" />
		<div class="container">
			<slot></slot>
		</div>
		<Footer :links="menuLinks" />
	</div>
</template>
<script setup>
const menuLinks = [
	{ url: '/', name: 'Главная' },
	{ url: '/auto', name: 'Автопарк' },
	{ url: '/prices', name: 'Маршруты/Цены' },
	{ url: '/contacts', name: 'Контакты' },
]
</script>
<style>
/*@import url('/assets/css/mdb.min.css');*/
body {
	background: #efeded;
}
.bg-danger {
	background-color: #ad1a1a !important;
}
.btn-danger {
	background-color: #ad1a1a;
}
.page {
	background: white;
}
</style>
