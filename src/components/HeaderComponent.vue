<template>
    <nav class="navbar navbar-expand-lg px-2 navbar-light bg-light">
        <a class="navbar-brand">
            <BigLogo />
        </a>
        <button class="navbar-toggler " style="width: 100px;" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
                <li class="nav-item active">
                    <a class="nav-link">Home</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link">Features</a>
                </li>
                <li class="nav-item dropdown">
                    <a class="nav-link">Community</a>  
                </li>
                <li class="nav-item">
                    <a class="nav-link">Blog</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link">Pricing</a>
                </li>
                <li class="nav-item">
                    <button>
                        Register Now 
                        <svg width="18" height="21" viewBox="0 0 6 7" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M4.42153 4.5177L5.24609 3.69314C5.34388 3.59535 5.34388 3.4368 5.24609 3.33901L4.42153 2.51445M5.17274 3.51607L1.50012 3.51607" stroke="white" stroke-width="0.367253" stroke-linecap="round"/>
                        </svg>
                    </button>
                </li>
            </ul>
        </div>
    </nav>
</template>
<script setup lang="ts">
    import BigLogo from "../assets/BigLogo.vue";
</script>
<style lang="css" scoped>
@media (min-width: 997px) {
    .nav-item>button{
        margin-left: 2rem;
    }
    .navbar-expand-lg .navbar-collapse {
        justify-content: flex-end;
    }
    .navbar-expand-lg .navbar-nav {
        width:60%;
        justify-content: space-around;
        align-items: center;
        /* width: 100%; */
        justify-content: space-around;
    }
}
    @media (max-width: 325px) {
        .navbar{
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }
    }
    .nav-item{
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .containery{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: .4rem;
    }
    nav{
        font-size: .8rem;
        color: #4D4D4D;
    }

    button{
        height: 36px;
        width: 130.8px;
        border-radius: 3px;
        /* padding: .8rem; */
        background-color:#4CAF4F;
        outline: none;
        font-size: .7rem;
        border: none;
        color: white;
        display: flex;
        align-items: center;
        cursor: pointer;
        justify-content: space-around;
    }
</style>