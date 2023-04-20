<template>
  <div class="resume">
    <div class="left">
      <div class="row">
        <div class="subtitle1">
          <h2>Education</h2>
        <!-- </div>
        <div class="life" v-for="school in education">
          <img class="image" :src="school.image" alt="" srcset="" />
          <h3>{{ school.title }}</h3>
          <h5>{{ school.year }}</h5>
          <div class="content">
            <p>{{ school.message }}</p>
          </div>
        </div> -->
       </div>
      <div class="row">
      
        <div class="timeline-items" >
          <div class="timeline-item" v-for="school in education" :key="school">
            <div class="timeline-dot"></div>
            <div class="timeline-date">{{school.year}}</div>
            <div class="timeline-content">
              <h3>{{school.title}}</h3>
              <p>{{ school.message}}</p>
            </div>
          </div>
        </div>
       
          <!-- <div class="timeline-item two">
            <div class="timeline-dot"></div>
            <div class="timeline-date">2010</div>
            <div class="timeline-content">
              <h3>title</h3>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa eius vel magnam necessitatibus numquam voluptatem quasi tempore, quos quaerat facere modi culpa quod ipsum cupiditate dolor fugiat perspiciatis sed iste!</p>
            </div>
          </div>
          <div class="timeline-item three">
            <div class="timeline-dot"></div>
            <div class="timeline-date">2010</div>
            <div class="timeline-content">
              <h3>title</h3>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa eius vel magnam necessitatibus numquam voluptatem quasi tempore, quos quaerat facere modi culpa quod ipsum cupiditate dolor fugiat perspiciatis sed iste!</p>
            </div>
          </div>
          <div class="timeline-item four">
            <div class="timeline-dot"> </div>
            <div class="timeline-date">2010</div>
            <div class="timeline-content">
              <h3>title</h3>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa eius vel magnam necessitatibus numquam voluptatem quasi tempore, quos quaerat facere modi culpa quod ipsum cupiditate dolor fugiat perspiciatis sed iste!</p>
            </div>
          </div>
        </div>  -->
        
          
    
      </div>
        
      </div>
    
    </div>
    <div class="right">
      <div class="subtitle2">
        <H2>Skills</H2>
      </div>
      <div class="group">
      <div class="star"  v-for="skill in skills" :key="skill">
        <img :src="skill.image" alt="" srcset="" />
        <h4>{{ skill.text }}</h4>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star"></span>
      </div>
    </div>
    <div class="soft">
      <ul>
        <li><i class="fa-solid fa-circle-check"> Interpersonal</i></li>
        <li><i class="fa-solid fa-circle-check"> Time Management</i></li>
        <li><i class="fa-solid fa-circle-check"> Teamwork</i></li>
        <li><i class="fa-solid fa-circle-check"> Adaptability</i></li>
        <li><i class="fa-solid fa-circle-check"> Creative</i></li>
        <li><i class="fa-solid fa-circle-check"> Leadership</i></li>
      </ul>
    </div>
      <div class="subtitle2">
        <h2>Interests</h2>
      </div>
      <div class="interest">
      <ul>
        <li>Volunteer work</li>
        <li>Music</li>
        <li>Hiking</li>
        <li>Outdoor Activities</li>
      </ul>
    </div>
      <!-- <div class="icons">
        <a href="https://www.linkedin.com/in/uzukhanye-dywili-a6976b255" target="_blank">
          <i class="fa-brands fa-linkedin fa-bounce"></i
        ></a>
        <a href="https://www.instagram.com/uzukhanyedywili" target="blank">
          <i class="fa-brands fa-instagram fa-bounce"></i
        ></a>
        <a href="https://www.github.com/Azukiwe" target="_blank">
          <i class="fa-brands fa-github fa-bounce"></i
        ></a>
      </div> -->
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      education: [
        {
          image:
            "https://i.postimg.cc/y8XQWmBj/life-choices-removebg-preview.png",
          year: "2022 - 2023",
          title: "Academy",
          message:
            "Accepted @ Life Choices Academy to study a Coding course: Full-Stack Developer.",
        },
        {
          image: "https://i.postimg.cc/QNfyv13Z/mama-flo.jpg",
          year: "2021 - present",
          title: "Volunteerism",
          message: "Became an Ambassador for a charity organisation, Mama'Flo, which provides long and short term solutions to fight period poverty.",
        },
        {
          image: "https://i.postimg.cc/WbC7V1nM/images-removebg-preview.png",
          year: "2021 - 2022",
          title: "College",
          message:
            "Accepted to study Business Management @ False Bay College: N4 - N5.",
        },
        {
          image: "https://i.postimg.cc/MZFv218c/LHS-logo-removebg-preview.png",
          year: "2016 - 2020",
          title: "High School",
          message: "started high school @ Livingstone High School & obtained a National Senior Certificate.",
        },
      ],
      skills: [
        {
          image: "https://i.postimg.cc/02WgvVLp/csslogo-removebg-preview.png",
          text: "CSS",
        },
        {
          image: "https://i.postimg.cc/Bb3g43Rq/Java-Script-logo.png",
          text: "JAVASCRIPT",
        },
        {
          image: "https://i.postimg.cc/63BmsR57/html-logo-removebg-preview.png",
          text: "HTML",
        },
        {
          image:
            "https://i.postimg.cc/prb3dTv8/BOOTSTRAP-LOGO-removebg-preview.png",
          text: "BOOTSTAP",
        },
        {
          image:
            "https://i.postimg.cc/k4hkPc1j/vue-js-logo-removebg-preview.png",
          text: "VUE JS",
        },
        {
          image:
            "https://i.postimg.cc/NLhgCNn2/My-SQL-removebg-preview.png",
          text: "MYSQL",
        },
        {
          image:
            "https://i.postimg.cc/dtQnLqNX/designer-ui-ux-removebg-preview.png",
          text: "UX/UI DESIGN",
        },
        {
          image:
            "https://i.postimg.cc/tgWbMtjL/nodejs-45adbe594d.png",
          text: "NODEJS",
        },
      ],
    };
  },
};
</script>
<style scoped>
.resume {
  display: flex;
 
}
.left,
.right {
  width: 50vw;
  display: flex;
  flex-direction: column;
  gap: 2rem;
  padding: 0;
  margin:0;
}

.image {
  scale: 0.5;
  
}
.life {
  min-height: 18rem;
  font-family: "Courier New", Courier, monospace;
}
.star{
  scale: 0.7;
  min-height: 3rem;
  
 
}
.star img{
 
  height: 6rem;
}

.group{
  display: grid;
  grid-template-columns: auto auto auto auto;
}
.soft ul{
  display: grid;
  grid-template-columns: auto auto ;
  list-style: none;
}
.subtitle1::first-letter,
.subtitle2::first-letter {
  font-size: 4rem;
  color: plum;
}
.subtitle1, .subtitle2{
  font-family: co;
}
.interest ul{
  list-style: none;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
 margin-left: 19rem;

}
.subtitle2{
  font-family: 'Courier New', Courier, monospace;
}
 .interest ul li::before{
  content:"\2022";
  color:orangered;
  font-weight: bold;
}
.fa-bounce{
padding:2rem;
color: black;
font-size: 3rem;
}
.checked {
  color: orangered;
}
.timeline-items{
max-width: 1000px;
margin: auto;
display: flex;
flex-wrap: wrap;
position: relative;
margin-bottom: 2rem;
}
.timeline-items::before{
  content:'';
  position:absolute;
  width:2px;
  height:100%;
  background-color: aliceblue;
  left: calc(50% - 1px);
  
}
.timeline-item{
margin-bottom: 40px;
width: 100%;
}
.timeline-item:last-child{
  margin-bottom: 0;
}
.timeline-item:nth-child(odd){
  padding-right:calc(50% + 30px);
  text-align: right;
}
.timeline-item:nth-child(even){
  padding-left:calc(50% + 30px);
  text-align: left;
}
.timeline-dot{
  height:16px;
  width:16px;
  background-color: palevioletred;
  position: absolute;
  left: calc(50% - 8px);
  border-radius:  50%;
  top: 10px;
}




.timeline-date{
  font-size:18px;
  color:deeppink;
  margin:6px 0 15px;
}
.timeline-content{
  background-color:white;
  padding:30px;
  border-radius: 5px;
}
.timeline-content h3{
  font-size: 20px;
  color:plum;
  margin: 0 0 10px;
  text-transform: capitalize;
  font-weight: 500;
}
.timeline-content p{
  color:black;
  font-size: 16px;
  font-weight: 300;
  line-height: 22px;
}




</style>
