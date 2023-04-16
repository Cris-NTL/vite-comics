<script>
export default {
    name: 'AppFooter',
    data() {
        return {
            comic: ["Character", "Comics", "Movies", "TV", "Games", "Videos", "News"],
            shop: ["Shod DC", "Shop DC Collectilbles"],
            dc: ["Terms Of Use", "Privacy Policy", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshop", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
            sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]
        }
    },
}
</script>

<template>
    <div class="container">
        <div class="wrap">
            <div class="left-side">

                <div class="links">

                    <h3>DC COMICS</h3>
                    <ul v-for="(element, index) in comic">
                        <li>{{ element }}</li>
                    </ul>

                    <h3>SHOP</h3>
                    <ul v-for="(element, index) in shop">
                        <li>{{ element }}</li>
                    </ul>

                </div>

                <div class="links">

                    <h3>DC</h3>
                    <ul v-for="(element, index) in dc">
                        <li>{{ element }}</li>
                    </ul>

                </div>

                <div class="links">

                    <h3>SITES</h3>
                    <ul v-for="(element, index) in sites">
                        <li>{{ element }}</li>
                    </ul>

                </div>
            </div>

            <div class="right-side">
                <div class="logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="logo">
                </div>
            </div>
        </div>

        <div class="bottom-container">
            <div class="bottom-left">

            </div>

            <div class="bottom-right">

            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/general.scss" as *;
@use "../style/app-footer.scss" as *;
</style>