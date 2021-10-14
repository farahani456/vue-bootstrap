<template>
        <!-- Services-->
        <section class="page-section" id="services">
            <div class="container">
                <div class="text-center">
                    <h2 class="section-heading text-uppercase">Services</h2>
                    <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
                </div>
                <div class="row text-center" >
                    <div class="col-md-4" v-for="(obj,key) in servicesJSON" :key="key">
                        <span class="fa-stack fa-4x">
                        <i class="fas fa-circle fa-stack-2x text-primary"></i><i class="fas fa-shopping-cart fa-stack-1x fa-inverse"></i>
                        </span>
                        <h4 class="my-3">{{ obj.title }}</h4>
                        <p class="text-muted">{{ obj.caption }}</p>
                    </div>
                </div>
            </div>
        </section>
</template>

<script>
export default{
data : () => ({
    servicesJSON: [
        {
            img: '<i class="fas fa-circle fa-stack-2x text-primary"></i><i class="fas fa-shopping-cart fa-stack-1x fa-inverse"></i>',
            caption: 'e-commerce embedded with payment system',
            title: 'E-Commerce'
        },
        {
            img: '<i class="fas fa-circle fa-stack-2x text-primary"></i><i class="fas fa-laptop fa-stack-1x fa-inverse"></i>',
            caption: 'best responsive design',
            title: 'Responsive Design'
        },
        {
            img: '<i class="fas fa-circle fa-stack-2x text-primary"></i><i class="fas fa-lock fa-stack-1x fa-inverse"></i>',
            caption: 'included responsive design',
            title: 'Web Security'
        }
    ]
})
}
</script>

<style lang="saas">
</style>