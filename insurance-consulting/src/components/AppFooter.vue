<script>
export default {
    name: "AppFooter",
    data() {
        return {
        
        }
    },
}
</script>

<template lang="">
    <footer>
        <section class="footer-main">
            <div class="container">
                <div class="row items">
                    <div class="col-12 col-md-6 col-lg-3 item">
                        <!-- logo -->
                        <div class="content-block logo">
                            <a  href="#" class="navbar-brand">
                                <img id="logo-footer" src="/img/nexgen-logo.svg" alt="Logo_NG" />
                            </a>
                        </div>      
                        <!-- paragrafo -->
                        <div class="content-block paragraph">
                            <p>
                                Built to the smallest detail With
                                <br>
                                a Focus on feature availability.
                            </p>
                        </div>
                        <!-- dati & icons -->
                        <ul class="navbar-nav icons content-block">
                            <li class="nav-item">
                                <a href="#">
                                    <i class="bi bi-telephone-fill"></i>
                                    tel:+1 (305) 1234-5678
                                </a>
                            </li>
                        </ul>
                        <!-- mail -->
                        <ul class="navbar-nav icons content-block">
                            <li class="nav-item">
                                <a href="#">
                                    <i class="bi bi-envelope"></i>
                                    hello@exaple.com
                                </a>
                            </li>
                        </ul>
                        <!-- sede -->
                        <ul class="navbar-nav icons content-block">
                            <li class="nav-item">
                                <a href="#">
                                    <i class="bi bi-geo-alt"></i>
                                    Main Avenue, 987
                                </a>
                            </li>
                        </ul>
                        <!-- button buy -->
                        <ul class="navbar-nav icons content-block">
                            
                            <li class="nav-item">
                                <button type="button" class="buy-button">BUY NEXGEN</button>
                            </li>
                        </ul>



                    </div> 

                    <div class="col-12 col-md-6 col-lg-3 item">

                    </div> 
                    <div class="col-12 col-md-6 col-lg-3 item"></div> 
                    <div class="col-12 col-md-6 col-lg-3 item"></div> 

                </div>
            </div> 
        </section>
    </footer>
</template>
<style lang="scss">
    @use "../style/partials/variables" as *;
    footer{
        background-color: $black-primary;
        color: $azz-secondary;

        .paragraph{
            
            margin-left: 3.2em;
        }

        #logo-footer {
            width: 8.5em;
            margin-top: 3em;
            margin-left: 3.1em;
        }

        .buy-button{
            width: 13em;
            height: 3.5em;
            background-color: $black-primary;
            border: 2px solid $blue-third;
            border-radius: 2.5em;
            color: $grey-secondary;
            
        }
    
    }
</style>