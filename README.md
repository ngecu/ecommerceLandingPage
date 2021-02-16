# E-COMMERCE LANDING PAGE ![](https://www.vectorlogo.zone/logos/w3_html5/w3_html5-icon.svg)  ![](https://www.vectorlogo.zone/logos/sass-lang/sass-lang-icon.svg) ![](https://www.vectorlogo.zone/logos/getbootstrap/getbootstrap-icon.svg) 

***

screenshot 001
![](Src/1.png)

screenshot 002
![](Src/2.png)

screenshot 003
![](Src/3.png)

screenshot 004
![](Src/4.png)

***

I will be using visual studio code and recommend you install the following extensions:

1.SASS Live Compiler by Ritwick Dey

2.Live Server by Ritwock Dey

3.HTML Snipetts by Mohammed Abusaid

4.HTML CSS Support by ecmel

5.Auto Rename Tag by Jun Han

6.Auto Close Tag by Jun Han

7.BeautifybyHookyQR
***
To start off,download the boilerplate from [my github account](https://github.com/ngecu?tab=repositories).You can access the repo by [clicking here](https://github.com/ngecu/ecommerceLandingPage)

***
So what does it entail exactly:

1.Html wit j basic structure having imported bootstrap script,main custom styling sheet and fontawesome javascript

    <!DOCTYPE html>
    <html>
    <head>
    <title>Online Store(Dev Ngecu)</title>

    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, minimum-scale=1" />

    <link rel="stylesheet" type="text/css" href="Css/bootstrap.min.css">

    <link rel="stylesheet" type="text/css" href="Css/main.css">
    <script src="js/fontawesome.js" crossorigin="anonymous"></script>



    </head>


    </html>

2.Bootstrap styling sheet

3.Main script styling sheet
***
We will begin with the top part of including the contact ad like the following:

![](Start/images/4.gif)

    <div class="bg-dark text-center">
    <img src="images/4.gif">
    </div>

This centers the image add and sets a dark background across the whole width of view
***
![](Src/first_nav.png)
Next is the navbar.Since we need it to center it having eqaul magins on right and left,we will enclose it in a class container

    <div class="container">
        <nav class="navbar  navbar-expand-lg navbar-light bg-light text-dark" id="myHeader">
        <a class="navbar-brand" href="#">
            <img src="images/logo.png" alt="" style="width: 100px;">
        </a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
    
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <a class="nav-link" href="#">Wholesale & Retail <span class="sr-only">(current)</span></a>
          </li>
     
        </ul>
    
    
        <div class="dropdown">
        
          <button class="btn dropdown-toggle text-dark" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Hi,Dev Ngecu
          </button>
          <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
            <a class="dropdown-item" href="#"> Account</a>
    
            <hr>
            <a class="dropdown-item btn btn-primary" href="#">Logout</a>
          </div>       
          
    
          
        </div>
    
        <div class="form-inline my-2 my-lg-0">
          
             <a href="#">
                <img  id="cart-icon" src="images/cart.png">
            </a>
            <p id="cart-total">0</p>
    
        </div>
      </div>
    </nav>
    </div>

We will also have another navbar that will display the main categories of products at the top:
![](Src/second_nav.png)

    <nav class="navbar navbar-expand-sm second-navbar navbar-light bg-danger text-light" id="navbar" data-toggle="affix">
        <div class="mx-auto d-sm-flex d-block flex-sm-nowrap">
            
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarsExample11" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse text-center" id="navbarSupportedContent">
    
              
                <ul class="navbar-nav mr-auto">
                  <li class="nav-item image-nav" id="image-nav">
                    <a href="#">
                      <img src="images/logo.png" width="50px" alt="">
                    </a>
                   
                  </li>
                 
                    <li class="nav-item dropdown">
                        <a class="nav-link  text-light" href="#">
                       Supermarket
                        </a>
                      
                      </li>

                      <li class="nav-item dropdown">
                        <a class="nav-link  text-light" href="#">
                       Electronics
                        </a>
                      
                      </li>

                      <li class="nav-item dropdown">
                        <a class="nav-link  text-light" href="#">
                       Computing
                        </a>
                      
                      </li>

                      <li class="nav-item dropdown">
                        <a class="nav-link  text-light" href="#">
                       Fashion
                        </a>
                      
                      </li>

                      <li class="nav-item dropdown">
                        <a class="nav-link  text-light" href="#">
                       Gaming
                        </a>
                      
                      </li>
            </div>
        </div>
    </nav>

On our main section of the body.We will introduce a div of class main and the contents inside it in a container div for equal margins as we did with the navbar above:

    <div class="main">
        <div class="w-100">
            <div class="container">
                //content
            </div>
        </div>

    </div>

![](Src/1st_row.png)

To begin the main content,it will have a first row having 3 columns where the first is 1/6 view,the third 2/3 and final 1/6 view.The first smaller column is our navbar having links to product categories.
                        
    <div class="col-lg-2 col-md-4 col-sm-6 col-xs-12 p-lg-0 ol bg-white rounded p-2">
          <ul style="padding-left: 0;padding:1%">
              <div id="accordion">
              
                  <div class="card m-2" >
                    <div  id="headingOne">
                      <div class="mb-0">
                          <li >
                              <a href="#">
                                  <i class="fas fa-shopping-basket" aria-hidden="true"></i>
                                  SuperMarket
                                  
                              </a>    
                              
                                  <i class=" fas fa-plus " data-toggle="collapse" data-target="#collapse_{{ forloop.counter }}" aria-expanded="false" aria-controls="collapse{{category}}" class="fas fa-plus"></i>
                          </li>
                      
                      </div>
                    </div>

                  </div>		  
              
                 </div>
          </ul>


      </div>

THe bigger column is an automated slider of coursel design

                    <div class="col-lg-8 col-md-4 col-sm-6 col-xs-12 rounded">
        
                        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
                            <ol class="carousel-indicators">
                                <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
                                <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
                                <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
                            </ol>
                            <div class="carousel-inner">
                                <div class="carousel-item active">
                                    <a href="#">
                                    <img class="d-block w-100 scr"	src="images/carousel/KE_Cross_BTS_1220_S.jpg" alt="First slide">
                                </a>
                                </div>
                                <div class="carousel-item">
                                    <a href="#">
                                    <img class="d-block w-100 scr"	src="images/carousel/Estee-Lauder_Jumia-1424x768.jpg" alt="Second slide">
                                </a>
                                </div>
                                <div class="carousel-item">
                                    <a href="">
                                    <img class="d-block w-100 scr"	src="images/carousel/KE_Grocery_1220_S-(1)-(1).jpg" alt="Third slide">
                                </a>
                                </div>
                                <div class="carousel-item">
                                    <a href="">
                                    <img class="d-block w-100 scr" 	src="images/carousel/1424x768-Homepage-Slider.png"		alt="Third slide">
                                </a>
                                </div>
                            </div>
                            <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
                                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                                <span class="sr-only">Previous</span>
                            </a>
                            <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
                                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                                <span class="sr-only">Next</span>
                            </a>
                        </div>
        
                    
                    </div>

The other smaller column is for ads

                    <div class="col-lg-2 col-md-4 col-sm-6 col-0 p-lg-0 advert ">
                        <div class="row h-100">
                          <div class="col-lg-12 h-50" >
                              <a href="#">
                            <img src="images/ee1.jpg" class="w-100 h-100" >
                        </a>
                        </div>
                            <div class="col-lg-12 h-150" >
                                <a href="">
                            <img  src="images/ee2.jpg"  class="w-100 h-100" alt="">
                        </a>
                          </div>
                        </div>
                            
                              
                      </div>

![](Src/2nd_row.png)

The next row will also classify more categories in a more classic way,whereby on hover the background image zooms in with a nice transition effect.For now will deal with the containments.

       <div class="row">   
       //three of these                
        <div class="col-lg-4 col-md-4 col-sm-12 col-xs-12">
            <div class="hovereffect">
                <img class="img-responsive" src="images/lr1.jpg" alt="">
                <div class="overlay p-4 text-light justify-content-lg-start font-weight-bold text-left">
                    <h2>Supermarket</h2>
                    <a class="btn btn-danger text-light info" href="#">Shop Now</a>
                </div>
            </div>
        </div>
      </div>

![](Src/3_rd.png)

The third row will have the same structure as the 2nd but will have a relative margin top to separate the two.

    <div class="row" style="margin-top: 1%;">
        <div class="col-lg-4 col-md-4 col-sm-12 col-xs-12">
            <div class="hovereffect">
                <img class="img-responsive" src="images/lr1.jpg" alt="">
                <div class="overlay p-4 text-light justify-content-lg-start font-weight-bold text-left">
                    <h2>Fashion</h2>
                    <a class="btn btn-danger text-light info" href="#">Shop Now</a>
                </div>
            </div>
        </div>
    </div>
  
![](Src/4_th.png)

The 4th row is of sponsoring brands

    <div class="row">
        <div class="card w-100">
            <h5 class="card-header bg-danger">Official Brands
              <p style="float: right;"> <a style="color: white;" href=""> More &#62; </a></p>
            </h5>

            <div class="card-body">
                <div class="row bg-white m-2 rounded ">
            
                    <div class="col-2">
                        <a href="#">
                        <img class="w-100" src="images/Brands/Xiaomi-400x200.jpg" alt="">
                    </a>
                    </div>
                    
                    <div class="col-2">
                        <a href="#">
                            <img class="w-100" src="images/Brands/On-Site-Logos66.jpg" alt="">
                        </a>
                    </div>
                    
                    <div class="col-2">
                        <a href="#">
                            <img class="w-100" src="images/Brands/Maybelline-400x200.jpg" alt="">
                        </a>
                        
                    </div>
                    
                    <div class="col-2">
                        <a href="#">
                        <img class="w-100" src="images/Brands/Samsung-400x200.jpg" alt="">
                        </a>
                    </div>
                    
                    <div class="col-2">
                        <a href="#">
                        <img class="w-100" src="images/Brands/Huawei-400x200.jpg" alt="">
                    </a>
                    </div>
                    
                    <div class="col-2">
                        <a href="#">
                        <img class="w-100" src="images/Brands/Carrefour-400x200.jpg" alt="">
                    </a>
                    </div>
    
    
                    <div class="col-2">
                        <a href="#">
                        <img class="w-100" src="images/Brands/Garnier-400x200.jpg" alt="">
                    </a>
                    </div>
                    
                    <div class="col-2">
                        <a href="#">
                        <img class="w-100" src="images/Brands/Bruhm.png" alt="">
                    </a>
                    </div>
                    
                    <div class="col-2">
                        <img class="w-100" src="images/Brands/Guiness-400x200.jpg" alt="">
                    </div>
                    
                    <div class="col-2">
                        <a href="#">
                        <img class="w-100" src="images/Brands/Hot-point.jpg" alt="">
                    </a>
                    </div>
                    
                    <div class="col-2">
                        <a href="#">
                        <img class="w-100" src="images/Brands/Nokia-400x200.jpg" alt="">
                    </a>
                    </div>
                    
                    <div class="col-2">
                        <a href="">
                        <img class="w-100" src="images/Brands/Jameson-400x200.jpg" alt="">
                    </a>
                    </div>
    
                    
                </div>
    
            </div>
          </div>
    </div>

![](End/static/images/bf20.gif)

    <div class="row">
        <img src="images/bf20.gif" alt="">
    </div>

The site will have 2 footers:

First being the lighter one and the other dark:

![](Src/1st_footer.png)

    <footer class="text-center text-lg-start">
      <!-- Grid container -->
      <div class="container p-4">
        <!--Grid row-->
        <div class="row">
          <!--Grid column-->
          <div class="col-lg-12 col-md-12 mb-4 mb-md-0">
            <h2 class="text-warning">
              Brands we stock
              
              </h2>
    
            <p>
              We pick the very best so you can be assured of the quality. There can be no compromises <br/> when it comes to materials, ease of wear, and durability.
            </p>
          </div>
    
          <div class="col-lg-12 col-md-12 mb-4 mb-md-0">
            <div class="row">
              <div class="col-lg-3 col-sm-12 col-3 ">
                <a href="">
                <img src="images/Brands/LG.jpg" alt="">
               </a>
              </div>
              <div class="col-lg-3 col-sm-12 col-3">
                <a href="">
                <img src="images/Brands/hotpoint.jpg" alt="">
               </a>
              </div>
    
              <div class="col-lg-3 col-sm-12 col-3">
                <a href="">
                <img src="images/Brands/redberry.jpg" alt="">
               </a>
              </div>
    
              <div class="col-lg-3 col-sm-12 col-3">
                <a href="">
                <img src="images/Brands/nunix.jpg" alt="">
               </a>
              </div>
    
            </div>
          
          
          </div>
         
        </div>
        <hr/>
        <div class="row">
          <div class="col-lg-3">
            <div class="row">
            <div class="col-lg-2 col-2">
              <i class="far fa-compass"></i>
            </div>
            <div class="col-lg-10 col-10 foo">
              
              <b>Countrywide Delivery</b>
              <br/>
              <p>
              We deliver in all parts of the country 
              </p>
            </div>
          </div>
          </div>
    
          <div class="col-lg-3">
            <div class="row">
            <div class="col-lg-2 col-2">
              <i class="fas fa-directions"></i>
                      </div>
            <div class="col-lg-10 col-10 foo">
              <b>Best Price</b>
              <br/>
              <p>
              We offer the affodable prices in all our products 
            </p>
            </div>
          </div>
          </div>
    
          <div class="col-lg-3">
            <div class="row">
            <div class="col-lg-2 col-2">
              <i class="fas fa-globe-africa"></i>
            </div>
            <div class="col-lg-10 col-10 foo">
    
              <b>Top Quality</b>
              <br/>
              <p>
              We have hand picked the best quality products, just for you. 
              </p>
            </div>
          </div>
          </div>
    
          <div class="col-lg-3">
            <div class="row">
            <div class="col-lg-2 col-2">
              <i class="far fa-compass"></i>
            </div>
            <div class="col-lg-10 col-10 foo">
              <b>100% Secure Checkout</b>
              <br/>
              <p>
              Mpesa/ PayPal / MasterCard / Visa 
            </p>
            </div>
          </div>
          </div>
          
    
        </div>
        <!--Grid row-->
      </div>
      <!-- Grid container -->
    
      <!-- Copyright -->
    
      <!-- Copyright -->
    </footer>

![](Src/2nd_footer.png)
