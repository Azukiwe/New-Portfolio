<template>
  <div class="about-sec">
    <img
      class="AD"
      src="https://i.postimg.cc/G2sN2Yx9/285884822-1048473679422053-4913379298348541465-n-removebg-preview.png"
    />
    <p>
      I am Uzukhanye Dywili,born 2002 June 14th. lives in 25 Ndemba crescent,site
      B,Khayelitsha,7784.I live with my mother and little sister.My favourite
      colour is lilac. An observer and very thoughtful person.full of life and
      not afraid to learn new things. My favourite person in this whole world
      and my motivation is my nephew who is 5 years old,seeing him/knowing that
      he exist motivates me to workhard and make sure he has a good life/better
      life. Passionate about helping people as a result, I am a Mama'Flo
      ambassador. Mama'flo is a charity organization that provides impoverished
      communities with long and short term solutions of sanitary towels. <br />
      <br />
    </p>
  </div>
</template>
<style scoped>
.about-sec {
  position: relative;
  box-shadow: 5px 10px plum;
  border-radius: 2rem;
  max-width: 60rem;
  max-height: 17rem;
  margin: 0 auto;
  margin-bottom: 5rem;
  display: flex;
 
}

.about-sec p {
  position: relative;;
  z-index: 10;
}
.AD {
  height: 30rem;
  transform: translateY(-10rem);
}
@media screen and (width <500px) {
  .about-sec {
    position: relative;
    max-width: 100%;
    flex-direction: column;
    box-shadow: none;
  }


  
  .AD {
    scale: 0.5;
  }
}
</style>
