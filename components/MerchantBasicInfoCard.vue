<template>
    <div class="three-row-two-sec-card">
        <div class="loader-wrp">
             <vcl-facebook v-if="isFbLoaderNeeded"></vcl-facebook>
        </div>
         <div class="columns is-mobile" v-if="isMainCardNeeded">
            <div class="column is-8">
                <p>
                    {{dataAcceptInput.name}}
                </p>
                <small>
                    {{dataAcceptInput.description}}
                </small>
                <p>
                    {{dataAcceptInput.rating}}
                </p>
            </div>
            <div class="column is-4">
                <figure>
                    <img v-lazy="dataAcceptInput.img" class="right-img" alt="">
                </figure>
            </div>
        </div>
    </div>
</template>

<script>
import { VclFacebook, VclInstagram } from 'vue-content-loading';

export default {
    props : {
        dataAcceptInput : Object
    },
    data() {
        return {
            isFbLoaderNeeded : false,
            isMainCardNeeded  : false
        }
    },
    components : {
        VclFacebook,
        VclInstagram,
    },
    created () {
        this.isFbLoaderNeeded = true;
    },
    mounted () {
        this.isFbLoaderNeeded = false;
        this.isMainCardNeeded = true;
    }
}
</script>

<style scoped>
.three-row-two-sec-card {
    padding: 10px;
    background: #ece4e4;
}
.right-img {
    float: right;
    height: 100px;
    width: 100px;
    background: #ddd;
}
</style>
