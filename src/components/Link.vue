<template>
    <a :href="`#${navLink.link}`">{{ navLink.name }}</a>
  
</template>

<script>
export default {
    name: "Link",

    props: {
        navLink: Object,
    }

}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;300;400&display=swap');


a {
    font-family: "Oswald", sans-serif;
    font-size: 1vw;
    color: rgba(255, 255, 255, 0.85);
    letter-spacing: 1px;
    /* text-transform: uppercase; */
    text-decoration: none;
}


@media (max-width: 1000px) {

    a {
        font-size: 2vw;
        letter-spacing: 0.5px;

    }
    
}


@media (max-width: 600px) {

    a {
        font-size: 3.5vw;
        letter-spacing: 0.5px;

    }
    
}



</style>