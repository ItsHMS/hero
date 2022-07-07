<template>
    <div class="full">
        <div class="header d-flex flex-row justify-space-between container align-center">
            <div class="d-flex flex-row ml-2">
                <v-avatar 
                class="rounded-lg bg-darkBlue"
                size="30"
                tile                
              >
                <span class="white--text text-h5">K.</span>
              </v-avatar>
              <h3 class="darkBlue pl-2">Kreed</h3>
            </div>
            <div class="buttons mr-3">
                <v-btn small>
                    <v-icon color="white">mdi-menu</v-icon>
                </v-btn>
               
            </div>
        </div>
        <div class="main d-flex flex-row align-center justify-space-around">
            <div class="first-half d-flex flex-column align-center justify-center">
                <div>
                <h1 class="darkBlue heading text-h2 font-weight-bold">
                    The easiest way to manage team projects & tasks
                </h1>
                <p>Take a tour of work management platform to see how you can do more of your best works.</p>
                    <v-btn large rounded class="primary-btns mr-3"> 
                        Know More
                        <v-icon  right>mdi-more</v-icon>
                    </v-btn>
                </div>
            </div>
            <div class="second-half d-flex flex-column align-center justify-center">
                <div>

                    <v-img 
                    class="image"
                    :src="require('~/assets/web.png')"
                    contain
                    />
                </div>
            </div>
            
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
    background: transparent;
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
    background: #1e255d;
}
.main{
    height: 100vh;
    margin-top:-100px
}

.heading{
    width:14ch;
    line-height: 1.3;
}
.main p{
    width:40ch
}
.primary-btns.v-btn{
    color:white ;
    background: #0061fe;
}
.first-half{

    width: 50%;
    height: 100%;

}
.second-half{
    width:50%;
    background:#0061fe;
    height:100%
}
</style>