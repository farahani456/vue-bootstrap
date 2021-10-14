<template>
<!-- Portfolio Grid-->
        <section class="page-section bg-light" id="portfolio">
            <div class="container">
                <div class="text-center">
                    <h2 class="section-heading text-uppercase">Portfolio</h2>
                    <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
                </div>
                <div class="row">
                    <div class="col-lg-4 col-sm-6 mb-4" v-for="(obj,key) in portfolioJSON" :key="key">
                        <!-- Portfolio item 1-->
                        <div class="portfolio-item" >
                            <a class="portfolio-link" data-bs-toggle="modal" href="#portfolioModal1">
                                <div class="portfolio-hover">
                                    <div class="portfolio-hover-content"><i class="fas fa-plus fa-3x"></i></div>
                                </div>
                                <img class="img-fluid" src="/assets/img/portfolio/close-icon.svg" alt="..." />
                            </a>
                            <div class="portfolio-caption">
                                <div class="portfolio-caption-heading">{{ obj.title }}</div>
                                <div class="portfolio-caption-subheading text-muted">{{ obj.caption }}</div>
                            </div>
                        </div>
                    </div>
                    
                </div>
            </div>
        </section>
</template>

<script>
export default{
data : () => ({
    portfolioJSON: [
        {
            img: '../src/assets/img/navbar-logo.svg',
            caption: 'first logo',
            title: 'Graphic design'
        },
        {
            img: '/src/assets/img/navbar-logo.svg',
            caption: 'second logo',
            title: 'Programming'
        },
        {
            img: '/src/assets/img/navbar-logo.svg',
            caption: 'third logo',
            title: 'Development'
        }
    ]
})
}
</script>

<style lang="saas">
</style>