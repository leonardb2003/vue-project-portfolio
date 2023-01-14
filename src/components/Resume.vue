<template>
    <section id="education" class="education">
      <div class="container">
        <h2>Education</h2>
        <p>My education are here to help and guide you. I am here to provide my education to help other developers to uderstand my work and to see what I'm cable of doing in my work areas.</p>
      </div>

        <div class="col-lg-4 icon-box" data-aos="fade-up" data-aos-delay="100">
          <div class="icon"><i class="fa fa-book" aria-hidden="true"></i></div>
          <h4 class="title"><a href="#">Subjects</a></h4>
          <p class="description">English Home Language</p>
           <p class="description">Afrikaans First Additional Language</p>
            <p class="description">Accounting</p>
             <p class="description">Business Studies</p>
              <p class="description">Life Science</p>
                <p class="description">Life Orientation</p>

        </div>
        <div class="col-lg-4 icon-box" data-aos="fade-up" data-aos-delay="200">
          <div class="icon"><i class="fa fa-certificate" aria-hidden="true"></i></div>
          <h4 class="title"><a href="#">Certificates</a></h4>
          <p class="description">National Senior Certificate</p>
          <p class="description">2019 National High School Olympiad</p>
            <p class="description">A Learning-and Life Skills Course</p>
            <p class="description">Banking On Our future Programme</p>

        </div>
        <div class="col-lg-4 icon-box" data-aos="fade-up" data-aos-delay="300">
          <div class="icon"><i class="far fa-id-card" aria-hidden="true"></i></div>
          <h4 class="title"><a href="#">Leadership</a></h4>
          <p class="description">L.E.A.D Scripture Union Prefect Camp</p>
          <p class="description">Bulls Award For Biggest Risk Taker</p>
          <p class="description">Prefect(Primary and High School)</p>


        </div>
        <div class="col-lg-4 icon-box" data-aos="fade-up" data-aos-delay="400">
          <div class="icon"><i class="fas fa-running" aria-hidden="true"></i></div>
          <h4 class="title"><a href="#">Extra Murals</a></h4>
          <p class="description">Atletics</p>
          <p class="description">Soccer</p>
          <p class="description">Netball</p>
          <p class="description">Adventure Club</p>

        </div>
        <div class="col-lg-4 icon-box" data-aos="fade-up" data-aos-delay="500">
          <div class="icon"><i class="fa fa-desktop" aria-hidden="true"></i></div>
          <h4 class="title"><a href="#">Computer Literacy</a></h4>
          <p class="description">Internet</p>
          <p class="description">Email</p>
          <p class="description">Microsoft Word</p>
          <p class="description">Microsoft Powerpoint</p>

        </div>

      <div class="card" v-for="item in resume">
                           <div class="card1" data-aos="fade-left" data-aos-duration="3000">
                               <div class="card-front brad">
                                   <img
                                   :src="item.img"
                                   alt="Avatar"
                                   style="width:400px; height: 350px"/>
                                   <div class="card">
                                       <h2>{{ item.name }}</h2>
                                       <h4>{{ item.title }}</h4>
                                       <h4>{{ item.year }}</h4>
                                       <h3>{{ item.description }}</h3>
                                   </div>
                               </div>
                           </div>
                          </div> 
     </section>
<div class="skills">
     <div class="div">
      <img src="https://i.postimg.cc/65hBMmCx/Bootstrap-logo-svg.png">
      <h1>BOOTSTRAP</h1>
      <p>60%</p>
     </div>
     <div class="div">
      <img src="https://i.postimg.cc/Df9xvR2V/download-1.png">
      <h1>HTML</h1>
      <p>80%</p>
     </div>
     <div class="div">
      <img src="https://i.postimg.cc/KzyYvZsk/198-1985002-css3-logo-hd-png-download.jpg">
      <h1>CSS</h1>
      <p>78%</p>
     </div>
     <div class="div">
      <img src="https://i.postimg.cc/6qkZ0V1T/Java-Script-Logo.png">
      <h1>JAVASCRIPT</h1>
      <p>50%</p>
     </div>
    </div>
  </template>
  <script>
  export default {
    resume: "card",
    data(){
      return{
        resume:[
          {name:'Academics',
           img:'https://i.postimg.cc/6qYn63J9/download-1.jpg',
           title:'Kensington High School',
           year:'2017-2021',
           description:'Highest grade passed is Grade 12',
        },
          {name:'Academics',
           img:'https://i.postimg.cc/qBP92XYV/download.png',
           title:'Life Choices',
           year:'2022-2023',
           description:'I am currently at Life Choices training coding, my goal is to improve my skills and become a full stack front-developer. ',
        },
        ]
      }
    }
  }
</script>
  <style scoped>

  .card1{
    display: flex;
    justify-content: center;
  }
  .card-front {
  border-radius: 50px;
  }
  .card-front img{
    margin-top: 20px;
  }
  .brad{
    border:4px solid black ;
    width: 500px;
    min-height: 200px;
    margin-top: 20px;
    /* margin-left: 500px; */
  }
  .card h4,h2,h3{
    font-size: 20px;
    color: black;
  }
  .container{
    color: black;
    font-size: 23px;
    font-weight: 500;
  }
  .container h2{
    font-size: 30px;
      color: #3773f7;
  }

  .div{
    background-color: #fbf4f4;
    width: 400px;
    height: 350px;
    margin-bottom: 20px;
  }
  .div img{
    width: 200px;
    height: 150px;
    margin-top: 20px;
  }
  .skills{
    display: grid;
    grid-template-columns: 1fr 1fr ;
    gap: 20px;
    padding: 20px;
    
  }
  .education .icon-box{
    margin-bottom: 20px;
}
.education .icon-box .icon i::before{
    line-height: 2 !important;
    margin-left: 2px;
}
.fa-certificate{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 54px;
    height: 54px;
    background: #0e8ac4;
    border-radius: 50%;
    transition: 0.5s;
    border: 1px solid #0e8ac4;
}
.fa-graduation-cap{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 54px;
    height: 54px;
    background: #0e8ac4;
    border-radius: 50%;
    transition: 0.5s;
    border: 1px solid #0e8ac4;
}
.fa-book{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 54px;
    height: 54px;
    background: #0e8ac4;
    border-radius: 50%;
    transition: 0.5s;
    border: 1px solid #0e8ac4;
}
.fa-running{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 54px;
    height: 54px;
    background: #0e8ac4;
    border-radius: 50%;
    transition: 0.5s;
    border: 1px solid #0e8ac4;
}
.fa-desktop{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 54px;
    height: 54px;
    background: #0e8ac4;
    border-radius: 50%;
    transition: 0.5s;
    border: 1px solid #0e8ac4;
}
.fa-id-card{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 54px;
    height: 54px;
    background: #0e8ac4;
    border-radius: 50%;
    transition: 0.5s;
    border: 1px solid #0e8ac4;
}
.education .icon i{
    color: black;
    font-size: 24px;
    margin-left: 12px;
}
.education .icon-box:hover .icon{
    /* background: #fff; */
}
.education .icon-box:hover .icon i{
    color:#fff;
}
.education title{
    margin-left: 80px;
    font-weight: 700;
    margin-bottom: 15px;
    font-size: 18px;
}
.education .title a{
    color: #ebebf0;
    margin-left: 80px;
    line-height: 24px;
}
.education .title a:hover{
    color: #0e8ac4;
}
.education .description{
    margin-left: 80px;
    line-height: 24px;
    font-size: 14px;
    color: black;
}

@media only screen and (max-width: 950px){
  .div{
    width: 270px;
  }
}
  </style>