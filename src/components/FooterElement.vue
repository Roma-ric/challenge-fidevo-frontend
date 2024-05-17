<template>
    <div>
        <div class="p-lg-4 p-md-3 p-3" style="background-color: #E6F1FC;">
            <p> We’d love to hear what you think! </p>
            <button class="m-0 btn text-dark border-dark rounded rounded-pill bg-light fw-lighter">
                Give feedback
            </button>
        </div>
        <footer class="p-lg-3 p-mb-2 p-2 d-flex flex-column align-items-lg-center align-items-md-start align-items-start" style="background-color: #004F9A;">
            <div class="d-flex flex-column align-items-lg-center align-items-md-start">
                <div class="d-flex flex-lg-row flex-md-column flex-column align-items-start m-1">
                    <routerLink to="/"> All Departments </routerLink>
                    <routerLink to="/"> Store Directory </routerLink>
                    <routerLink to="/"> Careers </routerLink>
                    <routerLink to="/"> Our Company </routerLink>
                    <routerLink to="/"> Sell on Walmart.com </routerLink>
                    <routerLink to="/"> Help </routerLink>
                    <routerLink to="/"> Product Recalls </routerLink>
                    <routerLink to="/"> Accessibility </routerLink>
                    <routerLink to="/"> Tax Exempt Program </routerLink>
                    <routerLink to="/"> Get the Walmart App </routerLink>
                </div>
                <div class="d-flex flex-lg-row flex-md-column flex-column align-items-start m-1">
                    <routerLink to="/"> Sign-up for Email </routerLink>
                    <routerLink to="/"> Safety Data Sheet </routerLink>
                    <routerLink to="/"> Terms of Use </routerLink>
                    <routerLink to="/"> Privacy & Security </routerLink>
                    <routerLink to="/"> California Supply Chain Act </routerLink>
                    <routerLink to="/">
                        <img src="https://i5.walmartimages.com/dfwrs/76316474-d730/k2-_3c5ba298-4f19-46be-9fc3-ac49225d19bd.v1.png"
                            alt="" width="25" height="15">
                        Your Privacy Choices
                    </routerLink>
                    <routerLink to="/"> Notice at Collection </routerLink>
                    <routerLink to="/"> NV Privacy Notice </routerLink>
                </div>
                <div class="d-flex flex-lg-row flex-md-column flex-column align-items-start m-1 mb-4">
                    <routerLink to="/"> WA Privacy Notice </routerLink>
                    <routerLink to="/"> Request My Personal Information </routerLink>
                    <routerLink to="/"> Brand Shop Directory </routerLink>
                    <routerLink to="/"> Pharmacy </routerLink>
                    <routerLink to="/"> Walmart Business </routerLink>
                    <routerLink to="/"> #IYWYK </routerLink>
                </div>
            </div>
            <p class="text-light mx-3" style="font-size: 12px;"> © 2024 Walmart. All Rights Reserved. </p>
        </footer>
    </div>
</template>

<script setup lang="ts">

</script>

<style scoped>
a {
    color: #000000;
    margin-left: 15px;
    font-size: 13px;
    font-weight: lighter;

    &.router-link-exact-active {
        color: #ffffff;
    }
}

a:hover {
    text-decoration: none;
}
</style>