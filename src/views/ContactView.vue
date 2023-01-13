<template>
  <div class="name">
    <h1>Contact Us</h1>
  </div> 
  <section id="contact" class="contact">
    <div class="container">
                    <div class="info">
                      <div class="address">
                        <i class="fa fa-map-marker" aria-hidden="true" ></i>
                        <h4>Location:</h4>
                        <p>6 Skepe Square,Factreton Avenue</p>
                      </div>
                      <div class="email">
                        <i class="fa fa-envelope" aria-hidden="true"></i>
                        <h4>Email:</h4>
                        <p>beyonceleonard65@gmail.com</p>
                      </div>
                      <div class="phone">
                        <i class="fa fa-phone" aria-hidden="true"></i>
                        <h4>Call:</h4>
                        <p>+27 6179 275 89</p>
                      </div>
                    </div>
        
                <div class="header">
                  <form action="https://formspree.io/f/xlevpezg" method="post" role="form" class="formspree-form">
                    <input type="text" name="name" class="form-control" placeholder="Your Name" required>
                    <input type="email" name="email" class="form-control" placeholder="Your Email" required>
                    <input type="text" name="subject" class="form-control" placeholder="Subject" required>
                    <textarea name="message" rows="8" placeholder="Your Message" required></textarea>
                    <div class="text-center"><button type="submit">Send Message</button></div>
                  </form>
                </div> 
    </div>  
  </section>       
</template>

<script>

</script>

<style scoped>
.contact .address,.email,.phone h4,p{
  color: black;
}
.contact{
    padding-bottom: 0px;
    margin-top: 100px;
}
.contact .header{
   width: 100%;
   display: flex;
   justify-content: center;
   align-items: center;
}
.header{
  max-width: 700px;
  margin-right: 50px;
  float: right;
  margin-top: -400px;
}
 .name h1{
  color:  #3773f7;
  font-size: 50px;
}  
.contact .info{
    padding: 30px;
    width: 300px;
    height: 400px;
    border-radius: 5px;
    box-shadow: 0 0 24px 0 rgba(0,0,0,0.12);
} 
.contact .info i{
    font-size: 20px;
    color: #149ddd;
    float: left;
    width: 44px;
    height: 44px;
    background: #dff3fc;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    transform: all 0.3s ease-in-out;
}
.contact .formspree-form .form-group{
    padding-bottom: 8px;
}
.contact .formspree-form input{
    height: 17px;
    border-radius: 6px;
}
.contact .formspree-form input,
.contact .formspree-form textarea{
    padding: 10px 12px;
}
.contact .formspree-form button[type="submit"]{
    background: #149ddd;
    border: 0;
    padding: 10px 12px;
    color: #fff;
    transition: 0.4s;
    border-radius: 4px;
}
.contact .formspree-form button[type="submit"]:hover{
    background: #004e72;
}
</style>