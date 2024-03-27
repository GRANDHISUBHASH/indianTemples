<script>
   export  let ListofTemples=[
        {
            id:1,
            templeName:"Ekambaranathar Temple",
            imageUrl:"./Ekambaranathar Temple.png",
            placeName:"tamilanadu",
            description:"Lord Shiva in the temple is a swayambumurthi. The Shiva Linga made of sand by Mother Kamakshi adores the sanctum sanctorum. The symbol of Mother embracing the Linga is still visible. Opposite the sanctum of Lord Ekambareswara are the Spatika Linga facing west and the Spatika Nandhi in the prakara. On the Ratha Sapthami day in the month of Thai (January-February) rays of Sun fall on Lord. Of the Panchabhoodha sthalas, the temple belongs to Earth-Prithvi.",
        },
        {
            id:5,
            templeName:"Ekambaranathar Temple",
            imageUrl:"./Ekambaranathar Temple.png",
            placeName:"tamilanadu",
            description:"Lord Shiva in the temple is a swayambumurthi. The Shiva Linga made of sand by Mother Kamakshi adores the sanctum sanctorum. The symbol of Mother embracing the Linga is still visible. Opposite the sanctum of Lord Ekambareswara are the Spatika Linga facing west and the Spatika Nandhi in the prakara. On the Ratha Sapthami day in the month of Thai (January-February) rays of Sun fall on Lord. Of the Panchabhoodha sthalas, the temple belongs to Earth-Prithvi.",
        },
        {
            id:4,
            templeName:"Ekambaranathar Temple",
            imageUrl:"./Ekambaranathar Temple.png",
            placeName:"tamilanadu",
            description:"Lord Shiva in the temple is a swayambumurthi. The Shiva Linga made of sand by Mother Kamakshi adores the sanctum sanctorum. The symbol of Mother embracing the Linga is still visible. Opposite the sanctum of Lord Ekambareswara are the Spatika Linga facing west and the Spatika Nandhi in the prakara. On the Ratha Sapthami day in the month of Thai (January-February) rays of Sun fall on Lord. Of the Panchabhoodha sthalas, the temple belongs to Earth-Prithvi.",
        },
        {
            id:3,
            templeName:"Ekambaranathar Temple",
            imageUrl:"./Ekambaranathar Temple.png",
            placeName:"tamilanadu",
            description:"Lord Shiva in the temple is a swayambumurthi. The Shiva Linga made of sand by Mother Kamakshi adores the sanctum sanctorum. The symbol of Mother embracing the Linga is still visible. Opposite the sanctum of Lord Ekambareswara are the Spatika Linga facing west and the Spatika Nandhi in the prakara. On the Ratha Sapthami day in the month of Thai (January-February) rays of Sun fall on Lord. Of the Panchabhoodha sthalas, the temple belongs to Earth-Prithvi.",
        },
        {
            id:2,
            templeName:"Ekambaranathar Temple",
            imageUrl:"./Ekambaranathar Temple.png",
            placeName:"tamilanadu",
            description:"Lord Shiva in the temple is a swayambumurthi. The Shiva Linga made of sand by Mother Kamakshi adores the sanctum sanctorum. The symbol of Mother embracing the Linga is still visible. Opposite the sanctum of Lord Ekambareswara are the Spatika Linga facing west and the Spatika Nandhi in the prakara. On the Ratha Sapthami day in the month of Thai (January-February) rays of Sun fall on Lord. Of the Panchabhoodha sthalas, the temple belongs to Earth-Prithvi.",
        },
    ]
</script>



<div class="home">
    
        <div class="templetemplate">
            <div class="timepleimg">
                <img src=".\NewHomeTemple.png" alt="HomeTemple"/>
            </div>
            <div class="content">
                <h1>7,50,000 Plus Temples and Counting...</h1>
                <button>Add Your Temple</button>
            </div>
        </div>

    
    <div class="templesfeed">
        <div class="latestAnDFeatures">
            <button>
                <img src="./newFeatured.png" alt="newFeatured"/>
            </button>
            <button>
                <img src="./newRecentlyEdited.png" alt="newRecentlyEdited"/>
            </button>

        </div>
        <div class="feedcontainer">
            
            <ul>
  {#each ListofTemples as temple}
    <li>
      <a href={`/temple-view/${temple.id}`}>
        <div>
          <h1>{temple.templeName}</h1>
          <p>{temple.placeName}</p>
          <img src={temple.imageUrl} alt={temple.templeName} />
          <p>{temple.description}</p>
        </div>
      </a>
    </li>
  {/each}
</ul>
</div>


        <div class="postCard">
            <h2>Posts</h2>
            <p>16 Divine Darshans of Unique Shivlingas</p>
            <hr/>
            <p>Top 10 Tallest Statues of Hindu Gods in the World</p>
            <hr/>
            <p>12 famous and beautiful Hindu Temples outside India</p>
            <hr/>
            <p>10 Ancient Magnificent Sculptures of Hindu Gods</p>
<hr/>
<p>
Arulmigu Subramaniya Swamy Temple, Tiruchendur</p>
<hr/>
<p>
Kopeshwar Temples
</p>
        </div>

    </div>
</div>
<style>
    

    
    .templetemplate{
        display: flex;
    justify-content: space-around;
    align-items: center;
        background: #FFDC60;
        width:100%;
        padding-top: 10%;
    }
    .content{
        flex-direction: column;
    display: flex;
    justify-content: center;
    align-items: center;

    }
    div h1{
        color:#A4213C;
    }
    .content button{
        background-color: #A4213C;
        border:none;
        color:white;
        height: 55px;
        width: 146px;
        border-radius: 10px;
    }
    .latestAnDFeatures{
        display: flex;
        flex-direction: column;
    }
    .templesfeed{
        background-color:rgb(84, 183, 187);
        width: 100%;
        display: flex;
        justify-content: space-between;
        padding: 50px;
    
    }
    .latestAnDFeatures button{
       
        border:none;
       background-color: transparent;
        background-size: contain;
        background-repeat: no-repeat;
        padding: auto;
    }
    a{
        text-decoration: none;
        color: black;
    }
    li{
        list-style: none;
    }
    .feedcontainer {
        border-radius: 20px;
    width: 40%;
    height: 800px;
    overflow-y: auto;
    scroll-behavior: smooth;
    scrollbar-width: none; /* Hide the scrollbar for Firefox */
    -ms-overflow-style: none; /* Hide the scrollbar for Internet Explorer and Edge */
}

.feedcontainer::-webkit-scrollbar {
    display: none; /* Hide the scrollbar for WebKit-based browsers like Chrome and Safari */
}
.feedcontainer div{
    background-color:white;
    border-radius: 12px;
    padding: 10px;
    margin: 20px;
    box-shadow: whitesmoke 1px;

}
    
    .feedcontainer div img{
        width: 100%;
    height: 36%;
    }
    .postCard{
        padding: 51px;
    }
    .latestAnDFeatures {
    padding: 62px;
}
</style>