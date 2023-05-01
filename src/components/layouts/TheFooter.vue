<template>
<section>
<h1>Contact me</h1>
<div>
    <ul>
        <li><a :href="linkedinLink" title="Linkedin"><linkedin></linkedin></a></li>
        <li><a :href="mailLink" title="E-Mail"><gmail></gmail></a></li>
        <li><a :href="whatsAppLink" title="Whatsapp"><app></app></a></li>
    </ul>
</div>
<div class="rights">
    <p>~ Copyright Uriel Kasabe ~</p>
</div>
</section>
</template>

<script>
import linkedin from '../../svgs/linkedin.vue';
import gmail from '../../svgs/gmail.vue';
import app from '../../svgs/whatsapp.vue';

export default {
components: {
    linkedin,
    gmail,
    app
},
data() {
    return{
        linkedinLink: 'https://www.linkedin.com/in/uriel-kasabe-276458262/',
        mailLink: 'mailto: urielkasabe5@gmail.com',
        whatsAppLink: 'https://wa.me/972528776372?text=Hi,%20Uriel%20I%20would%20like%20to%20contract%20you%20to%20my%20company!',
    };
}
}
</script>

<style scoped>
section{
background: linear-gradient(345deg ,black,rgb(18, 32, 85), rgb(25, 45, 116), rgb(35, 66, 177),rgb(25, 45, 116), rgb(18, 32, 85), black);
padding: 1rem;
text-align: center;
position: relative;
top: 20rem;
width: 100%;
height: fit-content;
}

h1{
    color: rgb(216, 214, 214);
}

ul{
    list-style: none;
    display: flex;
    justify-content: center;
    margin: 0 auto;
    position: relative;
    right: 1%;
}

.rights{
    text-align: center;
/*     position: relative;
    left: 1%; */
}

@media screen and (max-width: 768px) {
    section{
        width: 100%
    }
}

</style>