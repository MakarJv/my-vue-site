<template>
	<nav>
		<div class="openMenu">
			<ion-icon name="menu" class="openBtn"></ion-icon>
			<ion-icon name="close" class="closeBtn"></ion-icon>
		</div>
	</nav>
	<div class="group">
		<ul>
			<li><a href="#" class="homePage">Home</a></li>
			<li><a href="#" class="aboutMe">About Me</a></li>
			<li><a href="#">Setting</a></li>
		</ul>
	</div>
</template>

<script>
export default {
	mounted() {
		let openMenu = document.querySelector('.openMenu')
		let closeBtn = document.querySelector('.closeBtn')
		let openBtn = document.querySelector('.openBtn')
		let group = document.querySelector('.group')
		
		openBtn.onclick = function () {
			openMenu.classList.add('open')
			group.classList.add('open')
		}
		closeBtn.onclick = function () {
			openMenu.classList.remove('open')
			group.classList.remove('open')
		}
	}
}
</script>