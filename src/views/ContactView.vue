<template>
  <div class="header">
  <h1>Contact Us</h1>
</div>
  <section id="contact" class="contact">
   <section class="form-group">
                <div class="row" data-aos="fad-in">
                  <div class="col-lg-5 d-flex align-items-stretch">
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
                  </div>
                </div>

                    
          <!-- Form Section -->
          <div class="col-lg-7 mt-5 mt-lg-0 d-flex align-items-stretch">
            <form action="https://formspree.io/f/xlevpezg" method="post" role="form" class="formspree-form">
            <div class="form-row">
              <div class="form-group col-md-6">
                <label for="name">Your Name</label>
                <input type="text" name="name" class="form-control" id="name" data-rule="minlen:4" data-msg="Please enter at least 4 chars"/>
                <div class="validate"></div>   
              </div>
              <div class="form-group col-md-6">
                <label for="name">Your Email</label>
                <input type="email" class="form-control" name="email" id="email" data-rule="email" data-msg="Please enter a valid email "/>
                <div class="validate"></div>
              </div>
            </div>
            <div class="form-group">
              <label for="name">Subject</label>
              <input type="text" class="form-control" name="subject" id="subject" data-rule="minlen:4" data-msg="Please enter at least 8 chars of subject"/>
              <div class="validate"></div>
            </div>
            <div class="form-group">
              <label for="name">Message</label>
              <textarea class="form-control" name="message" rows="10" data-rule="required" data-msg="Please write something for us"></textarea>
              <div class="validate"></div>
            </div>
            <!-- Button -->
            <div class="text-center"><button type="submit">Send Message</button></div>
          </form>
          </div>
    </section><!-- End Section-->
  </section>

        
          
         
</template>

<script>

</script>

<style>
.contact{
    padding-bottom: 130px;
}
 .header h1{
  color: #149ddd;
  font-size: 90px;
}  
/* .contact .info{
    padding: 30px;
    background: #fff;
    width: 100%;
    box-shadow: 0 0 24px 0 rgba(0,0,0,0.12);
} */
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
 .contact .info h1{
    padding: 0 0 0 60px;
    font-size: 22px;
    font-weight: 600;
    margin-bottom: 5px;
    color: #050d18;
}  
/* .contact .formspree-form{
    width: 100%;
    padding: 0px;
    background: #dff3fc;
    box-shadow: 0 0 24px 0 rgba(0,0,0,0.12);
} */
.contact .formspree-form .validate{
    display: none;
    color: red;
    margin: 0 0 15px 0;
    font-weight: 400;
    font-size: 13px;
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