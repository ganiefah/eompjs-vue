<template>
    <div>
        <nav class="navbar navbar-expand-lg bg-body-tertiary">
            <div class="container-fluid">
              <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                  <li class="nav-item">
                    <router-link to="/" class="nav-link">Home</router-link>
                  </li>
                  <li class="nav-item">
                    <router-link to="/products" class="nav-link">Catalog</router-link>
                  </li>
                  <li class="nav-item">
                    <router-link to="/checkout" class="nav-link">Checkout</router-link>
                  </li>
                  <li class="nav-item">
                    <router-link to="/admin" class="nav-link">Admin</router-link>
                  </li>
                  <li class="nav-item">
                    <router-link to="/contact" class="nav-link">Contact Us</router-link>
                  </li>
                </ul>
              </div>
            </div>
          </nav>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>

.navbar{
    background-color: rgb(130, 234, 118) !important;
    
}
.nav-link{
    text-decoration: none;
    color: black;

}

.nav-link:hover{
color:rgb(120, 248, 133);
text-shadow: 1px 1px white;
}


</style>