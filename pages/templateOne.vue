<template>
    <div class="full">
        <div class="header d-flex flex-row justify-space-around align-center">
            <div class="d-flex flex-row">
                <v-avatar 
                class="rounded-lg bg-darkBlue"
                size="30"
                tile                
              >
                <span class="white--text text-h5">K.</span>
              </v-avatar>
              <h3 class="darkBlue pl-2">Kreed</h3>
            </div>
            <div class="buttons">
                <v-btn text>Home</v-btn>
                <v-btn text>About Us</v-btn>
                <v-btn text>How it Works</v-btn>
                <v-btn text>Services</v-btn>
                <v-btn text>Contact</v-btn>
                <v-btn rounded color="primary" class="white--text">Get Started</v-btn>
            </div>
        </div>
        <div class="main d-flex flex-row align-center justify-space-around">
            <div>
                <h1 class="darkBlue heading text-h2 font-weight-bold">
                    Connecting All your Banking Needs
                </h1>
                <p>A smart mobile application you can control your bussiness needs</p>
                <v-btn large rounded class="primary-btns mr-3"> 
                    <v-icon  left>mdi-apple</v-icon>
                    Download App
                </v-btn>
                <v-btn large rounded class="primary-btns">
                    <v-icon left>mdi-google-play</v-icon>
                    Download App
                </v-btn>
            </div>
            <v-img 
            class="image"
            :src="require('~/assets/mobile.png')"
            />
        </div>
    </div>
</template>
<script>
export default {
    layout: "template",
}
</script>
<style scoped>
.full{
    height:100vh;
    width: 100%;
    background: #f7f7f9;
}
.darkBlue{
    color:#1e255d;
}
.bg-darkBlue{
    background: #1e255d;
}
.header{
    height:100px;
}
.buttons .v-btn{
    color: #1e255d;
}
.image{
    max-width: 200px;
    height:auto;
    transform: rotate(45deg);
}
.heading{
    width:14ch;
    line-height: 1.3;
}
.main p{
    width:40ch
}
.primary-btns.v-btn{
    color:#1976d2 ;
    background:#e4e6f8 ;
}
</style>