<template>
  	<header>
   		<nav class="nav-container">
            <div class="logo">Life-Art</div>
            <ul class="nav-links">
                <li><a href="#">Accueil</a></li>
                <li><a href="#service">Services</a></li>
                <li><a href="#produit">Produits</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>

             <!-- hambuger menu -->
			<div class="hamburger-menu-container" @click="openMenu">
				<div
					class="hamburger-menu"
					:class="{ close: isActive }"
					id="toggle-menu"
				>111</div>
			</div>
			<!-- hambuger menu -->

			<!-- responsive mobile -->
			<div class="nav-mobile">
				<span class="close-mobile-menu" @click="openMenu">X</span>
				<a href="#" class="mobile-element" @click="openMenu">Accueil</a>
				<a href="#service" class="mobile-element" @click="openMenu">Service</a>
				<a href="#produit" class="mobile-element" @click="openMenu">Produits</a> 
				<a href="#Contact" class="mobile-element" @click="openMenu">Contact</a>
			</div>
			<!-- responsive mobile -->
        </nav>
    </header> 

    
</template>

<script>

export default{
  name: 'Navbar',
   data() {
    return {
     isActive: false,
    };
},
methods: {
		openMenu(event) {
			const toggleButton = document.getElementsByClassName("hamburger-menu")[0];
			const navLinks = document.getElementsByClassName("nav-mobile")[0];

			if (this.isActive == false) {
				navLinks.style.transform = "translate(-100%, 0)";
				this.isActive = true;
			} else if (this.isActive == true) {
				navLinks.style.transform = "translate(100%, 0)";
				this.isActive = false;
			}
		},
	},
}
</script>

<style>
@import '../style.css';
</style>