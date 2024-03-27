<script>
    import '@fortawesome/fontawesome-free/css/all.min.css';

    let showLoginMenu = false;

    const toggleLoginMenu = () => {
        showLoginMenu = !showLoginMenu;
        console.log("ONFOCUSTRIGGERS")
    };

    


    // Keyboard event handler for the button
   
</script>

<header>
    <nav>
        <div class="logocard">
            <img src="../tofi-logo_navbar.png" alt="logo"/>
            <h2>Temples Of India</h2>
        </div>
        <ul class="navlist">
            <li><a href="/">Home</a></li>
            <li><a href="/">Search</a></li>
            <li><a href="/NearByTemples">Nearby Temples</a></li>
            <li><a href="/"><i class="material-icons"></i>Add Temple</a></li>
            <li><a href="/AboutUs">About US</a></li>
            <li><button on:mouseenter={toggleLoginMenu} 
                 aria-haspopup="true" aria-expanded={showLoginMenu}>
                Login <i class="fa fa-chevron-down" aria-hidden="false"></i>
            </button>
            {#if showLoginMenu}
            <div class="login-dropdown" >
                <p>Login</p>
                <p>Signup</p>
                <p>Nearby Temples</p>
                <!-- Add more options as needed -->
            </div>
            {/if}

            </li>
        
       
        </ul>
    </nav>
</header>

<slot/>

<footer>
    <div class="footerContent">

    
     <div>
        <h1>Temples Of India <img src="../tofi-logo_navbar.png" alt="logo"/></h1>
        <p>World's Largest Hindu temples Portal</p>
     </div>
     <div class="quickLinks">
        <p>Quick Links</p>
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/">About</a></li>
            <li><a href="/">Nearby Temples</a></li>
            <li><a href="/">Download App</a></li>
            <li><a href="/">Donate to Us</a></li>
            <li><a href="/">Search Temples</a></li>
            <li><a href="/">Watch Video</a></li>
            <li><a href="/">Disclimer</a></li>
            <li><a href="/">ourBlog</a></li>
            <li><a href="/">Donate for Dharma</a></li>
    
         </ul>
     </div>
     <div>
        <ul class="socialMedia">
            <li><a href="https://www.facebook.com"><i class="fa-brands fa-facebook"></i></a></li>
            <li><a href="https://www.twitter.com"><i class="fa-brands fa-twitter"></i></a></li>
            <li><a href="https://www.instgram.com"><i class="fa-brands fa-instagram"></i></a></li>
            <li><a href="https://www.linkedin.com"><i class="fa-brands fa-linkedin"></i></a></li>
        </ul>
     </div>
    </div>
     <p>©Temples of India 2020-2023 | Email: contact@templesofindia.org</p>
     
</footer>

<style>
nav{
    display: flex;
    justify-content: space-between;
}
.logocard{
    display: flex;
}
.logocard img{
    height: 50px;
    width: 50px;

}
ul{
    list-style: none;
    display: flex;
    justify-content: space-around;
    width:50%;
}
   
a{
    text-decoration: none;
}
button{
    border:none;
    background-color: transparent;
}

footer{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width:100%;
    background-color: rgb(227, 209, 8);
}

.footerContent{
    display: flex;
   width:95%;
    height:300px;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    color: brown;
}


.footerContent ul li{
    font-size: large;
}
.quickLinks ul{


    display: flex;
    flex-wrap: wrap;
    width: 321px;
    height: 150px;
    flex-direction: column;
    gap: 10px;
    color:brown;
}
ul.socialMedia {
    display: flex;
    width: 197px;
    padding-right: 20px;
}
</style>