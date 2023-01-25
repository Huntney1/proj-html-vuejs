<script>
export default {
    name: "AppFooter",
    data() {
        return {
        
        }
    },
}
</script>

<template>
    
    <footer>
        <section class="footer-main">
            <div class="container">
                <div class="row items">

                    <!-- 1° sezione -->
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

                    <!-- 2° sezione -->
                    <div class="col-12 col-md-6 col-lg-3 item">
                        <div class="card">
                            <h3>Company</h3>
                            
                            <ul class="menu-Company">
                                <li class="menu-item "><a href="#">Institutional</a></li>
                                <li><a href="#">Social & Events</a></li>
                                <li><a href="#">Innovation</a></li>
                                <li><a href="#">Environment</a></li>
                                <li><a href="#">Technology</a></li>
                            </ul>
                    
                        </div>
                    </div> 

                    <!-- 3° sezione -->
                    <div class="col-12 col-md-6 col-lg-3 item">
                        <div class="card">
                            <h3>Services</h3>
                            
                            <ul class="menu-Company">
                                <li class="menu-item "><a href="#">Audit & Assurance</a></li>
                                <li><a href="#">Financial Advisory</a></li>
                                <li><a href="#">Analytics and M&A</a></li>
                                <li><a href="#">Middle Marketing</a></li>
                                <li><a href="#">Legal Consulting</a></li>
                            </ul>
                    
                        </div>
                    </div> 
                    
                    <!-- 4° sezione -->
                    <div class="col-12 col-md-6 col-lg-3 item">
                        <div class="card">
                            <h3>Consultants</h3>
                            
                            <ul class="menu-Company">
                                <li class="menu-item "><a href="#">David Cooper</a></li>
                                <li><a href="#">Oliver jones</a></li>
                                <li><a href="#">Emma Lopez</a></li>
                                <li><a href="#">T. Johnson</a></li>
                                <li><a href="#">jacob Hill jr</a></li>
                            </ul>
                    
                        </div>
                    </div> 

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

        .card{
            position: relative;
            z-index: 1;
            width: 100%;
            padding: 35px;
            border-radius: 10px;
            border: none;
            transition: all 0.4s ease-out 0s;
        }

        .items{
            display: flex;

            .menu-Company{ 
                display: block;
            }
        }
    
    }
</style>