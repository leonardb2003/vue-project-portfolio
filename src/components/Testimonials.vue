<template>
    <div class="name">
        <h1>Testimonials</h1>
    </div>
     <div class="container" >
        <div style="display: inline-block;">
            <div class="col">
                <div class="row pleaseWork">
                    <div class="flip-card" v-for="item in testimonials">
                        <div class="flip-card-inner">
                            <div class="flip-card-front">
                                <img
                                :src="item.img"
                                alt="Avatar"
                                style="width:300px; height: 300px"/>
                            </div>
                            <div class="flip-card-back">
                                <h1>{{ item.name }}</h1>
                                <h4>{{ item.title }}</h4>
                                <p>{{ item.test }}</p>
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
    testimonials: "test-cards",
    data(){
        return{
            testimonials:[
                {name: 'Zoe Daniels',
                    title: 'Colleague',
                    img:"https://i.postimg.cc/PtggkFdj/IMG-20221103-162448.jpg",
                    test:'Beyonce is a hard working lady with a big heart.She is organised,efficient and extremely competent with excellent rapport with people of all ages.Her communication skills are excellent no matter if you are talking about verbal or written. Her most important quality is that she always keeps herself updated with new information.Its just amazing to work with such a kind personality.'
                },
                {name: 'Keenan Olivier',
                    title: 'Colleague',
                    img:"https://i.postimg.cc/8NF3DKdc/IMG-4210.jpg",
                    test:'Beyonce is a resilient character and always looking out for others.'
                },
                {name: 'Oslin Johnson',
                    title: 'Lecturer',
                    img:"https://i.postimg.cc/c4sr7gB5/pic2.jpg",
                    test:'Beyonce is a unique person with great determination and not afraid to ask questions, which is a great quality to becoming a great professional. She is a diligent person as well with good time management skills.'
                },
                {name: 'Jake Jansen',
                    title: 'Colleague',
                    img:"https://i.postimg.cc/CLb12QLM/1-Jake.jpg",
                    test:'Beyoncé is very calm and observant, at the same time though, communicative especially in group work. Open and understanding and works well in groups. She is also the type to dedicate herself to effectively complete any task at hand. Beyoncé is very trustworthy and is someone you can rely on.'
                },
                {name: 'Ryan Thomas',
                    title: 'Lecturer',
                    img:"https://i.postimg.cc/NMg4vfwJ/testimonial-img-5.jpg",
                    test:'Beyonce is a strong and hard-working individual who always tries to ensure that she has trialed and tested multiple solutions before asking for any help, which strongly contributes to her growing as a strong and quick learner. Beyonce also has a good sense of humor and a bubbly personality.'
                },
                {name: 'Nikita Ramawoothar',
                    title: 'Colleague',
                    img:"https://i.postimg.cc/W4Pd37Db/nikita-instg.jpg",
                    test:'Beyonce is a wonderful person to work with and is always helpful when a colleague is in need. She displays amazing teamwork skills and always brings a positive energy to the workplace.'
                },
            ]
        }
    }
}

</script>
<style scoped>
.flip-card {
    background-color: transparent;
    width: 300px;
    height: 300px;
    perspective: 1000px;
    margin-top: 20px;
  }
  .flip-card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.8s;
    transform-style: preserve-3d;
  }
  .flip-card:hover .flip-card-inner {
    transform: rotateY(180deg);
  }
  .flip-card-front, .flip-card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    -webkit-backface-visibility: hidden; 
    backface-visibility: hidden;
  }
  .flip-card-front {
    background-color: white;
    color: black;
  }
  .flip-card-back {
    background-color: rgb(237, 246, 255);
    color: rgb(62, 83, 240);
    transform: rotateY(180deg);
  }
  .name h1{
    color:  #3773f7;
    font-size: 55px;
    text-transform: uppercase;
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