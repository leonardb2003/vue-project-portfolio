<template>
    <div class="work">
       <h1>Here are my projects</h1>
    </div>
       <div class="container" style="display: inline-block;">
           <div class="row justify-content-center cols-3">
               <div class="col">
                   <div class="row pleaseWork">
                       <div v-for="item in projects">
                           <div class="card" data-aos="fade-down" data-aos-duration="3000">
                               <div class="card-front ">
                                   <img
                                   :src="item.img"
                                   alt="Avatar"
                                   style="width:350px; height: 300px"/>
                               </div>
                               <div>
                                   <h1>{{ item.name }}</h1>
                                   <h4><a :href="item.github">Github</a></h4>
                                   <h4><a :href="item.netlify">netlify</a></h4>
                               </div>
                           </div>
                       </div>
                   </div>
               </div>
           </div>
       </div>     
   </template>
   <script>
   export default {
       projects: "cards",
       data(){
           return{
                projects:[
                   {name:'Calculator',
                    img:'https://i.postimg.cc/76XvySfh/Screenshot-20230112-143615.png',
                    github:'https://github.com/leonardb2003/my-calculator.git',
                    netlify:'https://beyonce-calculator.netlify.app/',
                   },
                   {name:'Javascript project',
                    img:'https://i.postimg.cc/wjF8Z7j0/Screenshot-20230112-143733.png',
                    github:'https://github.com/leonardb2003/javascript-project.git',
                    netlify:'https://beyonce-javascript-project.netlify.app/',
                   },
                   {name:' First Portfolio',
                    img:'https://i.postimg.cc/xdS5vR2Z/Screenshot-20230112-143855.png',
                    github:'https://github.com/leonardb2003/My-Portfolio.git',
                    netlify:'https://beyonce-leonard-portfolio.netlify.app/',
                   },
                   {name:'Calculator',
                    img:'https://i.postimg.cc/76XvySfh/Screenshot-20230112-143615.png',
                    github:'https://github.com/leonardb2003/my-calculator.git',
                    netlify:'https://beyonce-calculator.netlify.app/',
                   },
                   {name:'Calculator',
                    img:'https://i.postimg.cc/76XvySfh/Screenshot-20230112-143615.png',
                    github:'https://github.com/leonardb2003/my-calculator.git',
                    netlify:'https://beyonce-calculator.netlify.app/',
                   },
                   {name:'Calculator',
                    img:'https://i.postimg.cc/76XvySfh/Screenshot-20230112-143615.png',
                    github:'https://github.com/leonardb2003/my-calculator.git',
                    netlify:'https://beyonce-calculator.netlify.app/',
                   },
   
                ]
           }
       }
   }
   </script>
   <style scoped>
   .card{
    border: 2px solid black;
    border-radius: 1rem;
   }
   .work h1{
       font-size: 40px;
       color: #3773f7;
   }
   .card .name h1{
       color: #0e69f0;
   }
   .pleaseWork {
    display: grid;
    grid-template-rows: 1fr 1fr;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 20px;
    padding: 20px;
  }

  @media screen and (max-width: 992px) {
    .pleaseWork{
        display: grid;
        grid-template-rows: repeat(3, fr);
        grid-template-columns: 1fr 1fr;
    }
  }
  @media screen and (max-width: 674px) {
    .pleaseWork{
        grid-template-columns: 1fr;
        grid-template-rows: repeat(6, 1fr);
    }
  }
   </style>