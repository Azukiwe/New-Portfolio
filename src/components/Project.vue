<template >
  <div class="container">
  <div class="card-2"  v-for="project in projects" :key="project">
    <div class="card-whole">
    <img :src="project.image" class="card-img-top" alt="...">
    <div class="card-body">
      <h2 class="card-title">{{project.name}}</h2>
      <p>{{project.info}}</p>
      <div class="btn">
      <a :href="project.github" target="blank"><button>Check code</button ></a>
      <a :href="project.netlify" target="blank"><button>Go Live</button></a>
    </div>
  </div>
  </div>
</div>
</div>

</template>
<script>
export default {
    data(){
      return {
        projects:[
          {
          name: "Black Technology",
          image: "https://i.postimg.cc/DZvh5W2q/2.png" ,
          info: "An e-commerce practise site",
          github: "https://github.com/Azukiwe/black-technology",
          netlify: "https://black-technology.netlify.app",
        },
        {
          name: "Calculator",
          image: "https://i.postimg.cc/NMyVNGwN/homepage.jpg",
          info: "A digital calculator",
          github: "https://github.com/Azukiwe/calculator",
          netlify: "https://calc-ud.netlify.app",
        },
        {
          name: "Free People Boutique",
          image: "https://i.postimg.cc/WpBXMLb7/people.jpg",
          info: "An e-commerce practise site",
          github: "https://github.com/Azukiwe/Free-People-Boutique",
          netlify: "https://free-people.netlify.app",
        },
        {
          name: "Sneaker",
          image: "https://i.postimg.cc/BQHgRHKf/hi2-removebg-preview.png",
          info: "An e-commerce practice site",
          github: "https://github.com/Azukiwe/sneaker_site_2",
          netlify: "https://sneaker2.netlify.app",
        },
        {
          name: "Bootstrap portfolio",
          image: "https://i.postimg.cc/ZqSC6Rkg/49260-20210426-vr-premium-w6603.jpg",
          info: "One of my First portfolio",
          github: "https://github.com/Azukiwe/Uzu-portfolio",
          netlify: "https://uzukhanye-portfolio.netlify.app",
        },
        {
          name: "Connect Eskom",
          image: "https://i.postimg.cc/g0fVxZDW/2023-03-08.png",
          info: "An e-commerce site for Eskom with sells electronics ",
          github: "https://github.com/Azukiwe/connectwithEskom_EOYP.git",
          netlify: "https://connectwitheskom-44de8.web.app/",
        },
      ]
    }
}
}
</script>
<style scoped>
  .container{
    display: grid;
    grid-template-columns: auto auto auto;
    gap: 2rem;
    margin: 6rem;
  }

  .card-2{
    width: 18rem; 
    display:flex; 
    background-color: white;
    height:24rem
  }

  img{
    width: 15rem;
    margin-top: 1rem;
  }

  button{
   margin:1.5rem;
   border: 0.2rem solid plum;
   background-color: plum;
  border-radius: 20%;
 
  }
.btn{
  display: flex;
 padding: 2px;
 align-items: end;
}




 
</style>