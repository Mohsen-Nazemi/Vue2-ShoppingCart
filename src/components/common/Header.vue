<template>
  <header>
    <div class="header">

       <!-- ==================Left Header Section=========================  -->
      <div v-on:click="goTo('home')" class="logo">
        <h4 class="rest-title">Restaurant</h4>
        <img src="../../assets/images/logo.png" width="45px" height="45px"  />
      </div>


<!-- ==============Right Header Section============================ -->
      <div class=" header-right" >
        <i class="fa fa-shopping-cart cart-icon mb-1"></i>
        <span class="cart-count">0</span>

        <h5 class="login">ورود</h5>
        <h5 class="register">ثبت نام</h5>
      </div>

    </div>
  </header>
</template>

<script>
export default {

}
</script>

<style scoped>
.header{
    display: flex;
    justify-content: space-between;
}
.logo{
    display: flex;  
    align-items: center;
    margin: 15px;
}
.logo img{
    width: 35px;
    height: 35px;
    margin-left: 20px;
}
.header-right{
    width:200px;
    display: flex;
    justify-content: space-between;
    padding-right: 25px;
    align-items: center;
    font-family: Vazir;
    font-weight: 100!important;
}
header{
    /* background: rgba(140, 208, 240, 0.568); */
        box-shadow: 5px 5px 20px rgba(211, 46, 5, 0.376);
        

}
.rest-title{
    font-size: 20px;
}
.login, .register{
    border: 1px solid rgba(143, 14, 3, 0.486);
    padding: 3px 6px;
    border-radius: 5px;
        font-weight: 300!important;
        font-size:18px;    
}
.login:hover, .register:hover{
    color:#fff;
    border:none;
    background-color:rgba(143, 14, 3, 0.486) ;
    transition: all ease .5s;
       
}
.cart-icon{
    font-size:18px;
}
.cart-count{
    border: 1px solid black;
    border-radius: 100%;
    position: relative;
    bottom: 15px;
    right: 10px;
    padding:0px 6px;
    font-size:15px;
    background-color: rgba(255, 127, 80, 0.424);
    font-weight: bold;
    /* color: */

}
</style>