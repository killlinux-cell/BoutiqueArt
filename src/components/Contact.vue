<template>
    <section class="contact" id="contact">
    <div class="contact-info">
        <h2>Contactez-nous</h2>
        <p>Pour toute question ou demande d'assistance, n'hésitez pas à nous contacter :</p>
        <ul>
            <li><i class="fas fa-phone"></i> Téléphone : +1 123 456 789</li>
            <li><i class="fas fa-envelope"></i> Email : contact@votreentreprise.com</li>
            <li><i class="fas fa-map-marker-alt"></i> Adresse : 123 Rue de l'Exemple, Ville</li>
        </ul>
    </div>
    <div class="map">
        <iframe src="https://www.openstreetmap.org/?mlat=48.8588443&mlon=2.2943506&zoom=15" width="600" height="400" frameborder="0" scrolling="no"></iframe>
    </div>
</section>

</template>

<script>


    export default{
        name: 'Contact',
    }
</script>


<style>
@import '../style.css';
</style>