<template>
    <h1>Testimonials</h1>
     <div class="container" style="display: inline-block;">
        <div class="row justify-content-center cols-3">
            <div class="col">
                <div class="row">
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
                    title: 'Colleague',
                    img:"https://i.postimg.cc/c4sr7gB5/pic2.jpg",
                    test:'Beyonce is a unique person with great determination and not afraid to ask questions, which is a great quality to becoming a great professional. She is a diligent person as well with good time management skills.'
                },
                {name: 'Jake Jansen',
                    title: 'Colleague',
                    img:"https://i.postimg.cc/PtggkFdj/IMG-20221103-162448.jpg",
                    test:'Beyoncé is very calm and observant, at the same time though, communicative especially in group work. Open and understanding and works well in groups. She is also the type to dedicate herself to effectively complete any task at hand. Beyoncé is very trustworthy and is someone you can rely on.'
                },
                {name: 'Ryan Thomas',
                    title: 'Colleague',
                    img:"https://i.postimg.cc/NMg4vfwJ/testimonial-img-5.jpg",
                    test:'Beyonce is a strong and hard-working individual who always tries to ensure that she has trialed and tested multiple solutions before asking for any help, which strongly contributes to her growing as a strong and quick learner. Beyonce also has a good sense of humor and a bubbly personality.'
                },
                {name: '',
                    title: 'Colleague',
                    img:"https://i.postimg.cc/PtggkFdj/IMG-20221103-162448.jpg",
                    test:''
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
  /* This container is needed to position the front and back side */
  .flip-card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.8s;
    transform-style: preserve-3d;
  }
  /* Do an horizontal flip when you move the mouse over the flip box container */
  .flip-card:hover .flip-card-inner {
    transform: rotateY(180deg);
  }
  /* Position the front and back side */
  .flip-card-front, .flip-card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    -webkit-backface-visibility: hidden; /* Safari */
    backface-visibility: hidden;
  }
  /* Style the front side (fallback if image is missing) */
  .flip-card-front {
    background-color: white;
    color: black;
  }
  /* Style the back side */
  .flip-card-back {
    background-color: rgb(237, 246, 255);
    color: rgb(62, 83, 240);
    transform: rotateY(180deg);
  }
</style>