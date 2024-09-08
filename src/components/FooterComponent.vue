<template>
   
    <div class="containery">
  <footer class="row row-cols-1 row-cols-sm-1 ">
    <div class="col-md-3 mb-3 main">
      <a class="logo d-flex align-items-center mb-3 link-body-emphasis text-decoration-none">
        <BigLogo2 />
      </a>
      <p>Copyright © 2024 Olamilly. <br> Free Template From Figma.</p>
      <p>All rights reserved.</p>
      <div id="social-box">
        <SocialIcons />
      </div>
    </div>
    <div class="col-md-1"></div>

    <div class="col-md-2 mb-3 mycol">
      <h5>Company</h5>
      <ul class="nav aj">
        <li class="nav-item mb-2"><a class="nav-link p-0 ">About Us</a></li>
        <li class="nav-item mb-2"><a class="nav-link p-0 ">Blogs</a></li>
        <li class="nav-item mb-2"><a class="nav-link p-0 ">Contact Us</a></li>
        <li class="nav-item mb-2"><a class="nav-link p-0 ">Pricing</a></li>
        <li class="nav-item mb-2"><a class="nav-link p-0 ">Testimonials</a></li>
      </ul>
    </div>

    <div class="col-md-2 mb-3 mycol">
      <h5 >Support</h5>
      <ul class="nav aj">
        <li class="nav-item mb-2"><a class="nav-link p-0 text-left">Help Center</a></li>
        <li class="nav-item mb-2"><a class="nav-link p-0 ">Terms of service</a></li>
        <li class="nav-item mb-2"><a class="nav-link p-0 ">Legal</a></li>
        <li class="nav-item mb-2"><a class="nav-link p-0 ">Privacy policy</a></li>
        <li class="nav-item mb-2"><a class="nav-link p-0 ">Policy</a></li>
      </ul>
    </div>

    <div class="col-md-4 mb-3 lascol" >
      <h5>Stay up to date</h5>
      <ul class="nav ">
        <li class="nav-item mb-2" style="width: 100%;">
            <div class="my-input-group">
                <input class="email-form" placeholder="Your email address"/>
                <div class="send-icon">
                    <svg width="20" height="20" viewBox="0 0 7 7" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <g clip-path="url(#clip0_315_587)">
                    <path fill-rule="evenodd" clip-rule="evenodd" d="M6.34977 0.37657C6.41778 0.444588 6.44083 0.545558 6.40905 0.636349L4.65625 5.64435C4.62233 5.74125 4.5327 5.80763 4.43011 5.81182C4.32753 5.816 4.23279 5.75715 4.19109 5.66333L3.2286 3.49773L1.06301 2.53525C0.969191 2.49355 0.910331 2.39881 0.914516 2.29622C0.918701 2.19364 0.985083 2.104 1.08199 2.07009L6.08999 0.317288C6.18078 0.28551 6.28175 0.308552 6.34977 0.37657ZM3.71697 3.36348L4.39221 4.88278L5.57388 1.50657L3.71697 3.36348ZM5.21976 1.15245L1.84356 2.33412L3.36285 3.00936L5.21976 1.15245Z" fill="white"/>
                    </g>
                    <defs>
                    <clipPath id="clip0_315_587">
                    <rect width="6.0096" height="6.0096" fill="white" transform="translate(0.663818 0.0527344)"/>
                    </clipPath>
                    </defs>
                    </svg>
                </div>
            </div>
        </li>
      </ul>
    </div>
  </footer>
</div>
</template>
<style lang="css" scoped>
footer{
    width:100%;
}
.email-form{
    background-color: #7d7d7d;
    padding: .8rem;
    border: none;
    outline: none;
    width:80%;
    border-radius: 8px;
    color:white;
    box-shadow: inset 0 0 10px #9b9995;
}

.send-icon{
    margin-left: -30px;
    cursor: pointer;
    z-index: 1;
    margin-top: .2rem;
    padding-right: .5rem;
    /* font-size: 1rem; */
}
.my-input-group{
    display: flex;
    align-items: center;
}
.lascol{
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    text-align: left;
}

::placeholder {
    color:white;
  opacity: 1; /* Firefox */
}

::-ms-input-placeholder { /* Edge 12 -18 */
    color:white;
}
.mycol{
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
}
.aj{
    flex-direction: column;     
    align-items: flex-start;
}
.nav-link{
    text-align: left;
}

@media (min-width: 300px ) and (max-width: 767.98px) {
    .aj{
        display: flex;
        flex-direction: row;
        align-items: center;
        width: 100%;
        justify-content: space-around;
    }
    h5{
        align-self: center;
    }
    .lascol>h5{
        text-align: center;
    }
    .my-input-group{
        justify-content: center;
    }
 }

.nav-link{
    color:white;
}
.logo{
    justify-content: center;
}
.containery{
    padding: 1rem;
    background-color: #263238;
    display: flex;
    align-items: center;
    justify-content: space-around;
    color:white;
    font-size: .55rem;
    padding-top: 2rem;
}

</style>
<script setup lang="ts">
    import BigLogo2 from "../assets/BigLogo2.vue";
    import SocialIcons from "./SocialIcons.vue";
    
</script>