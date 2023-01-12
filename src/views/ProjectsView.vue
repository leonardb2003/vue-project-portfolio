<template>
 <div class="work">
    <h1>Here are a few of my projects</h1>
 </div>
    <div class="container" style="display: inline-block;">
        <div class="row justify-content-center cols-3">
            <div class="col">
                <div class="row">
                    <div class="card" v-for="item in projects">
                        <div class="card">
                            <div class="card-front">
                                <img
                                :src="item.img"
                                alt="Avatar"
                                style="width:400px; height: 350px"/>
                            </div>
                            <div class="card">
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
                {name:'Portfolio draft',
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
<style>
.work h1{
    font-size: 40px;
    color: #0e69f0;
}
.card .name h1{
    color: #0e69f0;

}
</style>