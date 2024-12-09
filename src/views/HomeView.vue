<script setup>
  
</script>

<template>
  
  <section class="home-container">
    
    <div class="icon-container">
      <i class="fa-solid fa-desktop"></i>
    </div>

    <div class="name-container">
      <h1>Fernando Arróliga</h1>
    </div>

    <div class="header-container">
      
      <div class="description-text">
        <h2>Software Developer</h2>
        <div style="display: flex;">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque a fringilla magna, 
            eu interdum erat. Nulla elementum vitae neque id pharetra. Vivamus eget mollis est, 
            vitae auctor dui. Proin sed sodales quam. Pellentesque convallis laoreet lectus, in 
            pellentesque ipsum viverra id. Donec sit amet urna in dui laoreet mattis facilisis ut ipsum. 
          </p>
        </div>
        <div style="display: flex;">
          <p>
            Aliquam in mauris ut felis luctus tincidunt. Cras faucibus iaculis lacus et varius. 
            Sed ac ipsum diam. Suspendisse porttitor gravida lacus, eu ornare tortor eleifend vel. 
            Suspendisse et nulla interdum, rhoncus turpis condimentum, laoreet urna. 
            Ut tempus est eu eros fringilla, ac molestie lacus auctor. In mattis eros sit amet 
            aliquam tempus. Fusce eu convallis est. 
          </p>
        </div>
      </div>

      <div class="header-image">
        <img src="../assets/universe01.jpg">
      </div>
    
    </div>

  </section>

  <section class="experience-container">
  
    <div class="experience-one">
      <span>5+</span>
      <p>Years of Experience</p>
    </div>

    <div class="experience-two">
      <span>100+</span>
      <p>Projects Completed</p>
    </div>

    <div class="experience-three">
      <span>30+</span>
      <p>Satisfied Clients</p>
    </div>
  
  </section>

  <section style="height: 100vh;" class="skills-container">
  </section>
   
  <section class="projects-container">
  </section>

  <section class="contact-container">
  </section>

</template>

<style scoped>


  /* Dark Mode Styles*/
  /*body.dark .title-container h1 {
    color: #fff;
  }
  body.dark .home-container {
    background-color: #000;
    color: #fff;
  }
  body.dark .experience-container {
    background-color: #000;
    color: #fff;
  }*/
  
  /* Home Container */
  .home-container {
    display: flex;
    flex-direction: column;
    gap: 10px;
    padding: 100px 100px;
  }
  .icon-container {
    display: flex;
    align-items: center;
  }
  .name-container {
    display: flex;
    align-items: center;
  }
  .name-container h1 {
    font-weight: bold;
    font-size: 40px;
  }
  .header-container {
    display: flex;
    /*grid-template-columns: 1fr 1fr;*/
    justify-content: center;
    align-items: center;
    gap: 10px;
  }
  .description-text {
    display: flex;
    flex-direction: column;
    padding-right: 100px;
    gap: 10px;
  }
  .header-image {
    display: flex;
    align-items: center;
    /*width: 300px;
    height: 300px;*/
  }
  .header-image img {
    width: 250px;
    height: 250px;
  }
  /* Experience Container */
  .experience-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 20px 100px;
    padding-top: 20px;
    padding-bottom: 20px;
    border-top: 1px solid gray;
    border-bottom: 1px solid gray;
  }
  .experience-one {
    display: flex;
    gap: 10px;
    flex-direction: column;
  }
  .experience-one {
    display: flex;
    gap: 10px;
    flex-direction: column;
  }
  .experience-one {
    display: flex;
    gap: 10px;
    flex-direction: column;
  }
  .experience-container span {
    font-weight: bold;
    font-size: 20px;
  }
  
  @media (max-width: 768px) {
    .header-container {
      display: flex;
      flex-direction: column;
    }
    .description-text {
      display: flex;
      padding-right: 0px;
    }
  }
  @media (max-width: 760px) {
    .experience-container {
      display: flex;
      flex-direction: column;
      gap: 10px;
      margin: 10px 10px;
    }
  }

</style>
