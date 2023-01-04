<script>
export default {
    props:['AboutData.firstname'],
    methods:{
        about(){
            console.log(this.AboutData)
        }
    },
    data(){
        return{
            AboutData:{
                firstName:null,
                lastName:null,
                pinCode:null
            }
        }
    }
    

}
 </script>

<template>
    <div id='About-info'>
        {{ AboutData.firstName }}
    <h2>About Me</h2>
    <form  @submit.prevent="getFormValues">
        <!-- <v-form v-on:submit="About" action="#" method="post"></v-form> -->
<!--  -->
    First Name:<input type="text" v-model="AboutData.firstName" placeholder="Enter your Name" name="firstName" /><br>
    Last Name:<input type="text" v-model="AboutData.lastName" placeholder="Enter your lastName" name="lastName" /><br>
    Pin Code:<input type="text" v-model="AboutData.pinCode" placeholder="Enter pincode" name="pinCode"/><br>
    <button v-on:click="about">Submit</button>
    <!-- <RouterLink to="/product">></RouterLink> -->
    <!-- <v-on:click="Submit"> -->
    <!-- <v-form v-on:submit="sub" action="#" method="post"></v-form> -->

    </form>
    </div>
</template>