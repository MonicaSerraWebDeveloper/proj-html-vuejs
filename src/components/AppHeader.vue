<script>

    export default {
        name: 'AppHeader'
    }


</script>

<template>

    <header>
        <div class="container">
            <div class="row">
                <div>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quae, eligendi.</div>
            </div>
            <button class="button-primary">Get in touch</button>
            <button class="button-secondary">Get in touch</button>
        <h1>get in touch</h1>
        <h2><span class="span-title">The</span> Company</h2>
        <div class="dark">
            <h2><span class="span-title-negative">The</span> Company</h2>
        </div>
        
        
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eos reiciendis consequuntur maiores repellendus repudiandae pariatur, voluptatibus ipsam ullam quae sequi optio beatae voluptatum sed omnis delectus quos culpa odio? Fuga?</p>
        </div>
        <div class="container-large">
            <h3>get in touch</h3>
            <h4>get in touch</h4>
        </div>
        
    </header>

</template>

<style scoped lang="scss">

    @use '../style/partials/buttons' as *;

    .dark {
        background-color: #000;
        padding: 50px;
    }

</style>