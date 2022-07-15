
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!-- displays site properly based on user's device -->

    <link
      rel="icon"
      type="image/png"
      sizes="32x32"
      href="./images/favicon-32x32.png"
    />

    <style>
      @import url("https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,700&family=Montserrat:wght@500;700&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: hsl(30, 38%, 92%);
}
html {
  font-size: 10px;
}

.container {
  width: 40%;
  height: 60%;
  display: flex;
  border-radius: 1rem;
  overflow: hidden;
}

img{
  width: 50%;
  object-fit: cover;
}
.heading {
  margin: 0.8rem;
  font-size: 1.45rem;
  padding: 2rem 1.5rem;
  font-weight: 500;
  color: hsl(228, 12%, 48%);
  font-family: "Montserrat", sans-serif;
  letter-spacing: 0.7rem;
  text-transform: uppercase;
}
.details {
  background-color: hsl(0, 0%, 100%);
  width: 50%;
}

.title {
  font-family: "Fraunces", serif;
  font-size: 3.2rem;
  line-height: 3rem;
  padding: 0rem 2.8rem;
  margin: 0.3rem;
}

.discription {
  color: hsl(228, 12%, 48%);
  
  font-family: "Montserrat", sans-serif;
  font-size: 500;
  font-size: 1.4rem;
  padding: 1.8rem 3.4rem;
  line-height: 2.2rem;
}

.price {
  font-family: "Fraunces", serif;
  display: flex;
  /* align-items: center; */
  /* justify-content: space-evenly; */
  padding: 1rem 3.5rem;
}

.discounted-price {
  font-size: 3.5rem;
  color: hsl(158, 36%, 37%);
}

.checked-price{
  margin: 1.5rem;
  text-decoration: line-through;
  color: hsl(228, 12%, 48%);
}

button{
  display: block;
  width: 75%;
  margin: 1rem auto;
  padding: 1.5rem;
  
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
  border-radius: 1rem;
  color: white;
  cursor: pointer;
  background-color: hsl(158, 36%, 37%);
  border: none;
  transition: background-color .3s;  
}

button:hover{
  background-color: hsl(158, 42%, 30%);
}
button i{
  margin: 0 .7rem;
}

 @media screen and (max-width:1365px) {
  .container{
    width: 43%;
  }
}

@media screen and (max-width:1270px) {
  .container{
    width: 46%;
  }
}

@media screen and (max-width:1214px) {
  .container{
    width: 50%;
  }
}

@media screen and (max-width:1150px) {
  .container{
    width: 55%;
  }
}


@media screen and (max-width:1000px) {
  .container{
    width: 61%;
  }
}
@media screen and (max-width:900px) {
  .container{
    width: 67%;
  }
}
@media screen and (max-width:790px) {
  .container{
    width: 74%;
  }
  .discription{
    padding: 1.8rem 3.2rem;
  }
}
@media screen and (max-width:685px) {
  .container{
    width: 82%;
  }
  .title{
    font-size: 3rem;
  }
  .discription{
    font-size: 1.3rem;
    padding: 1.8rem 3rem;
  }
  .discounted-price{
    font-size: 3.2rem;
  }
}

@media screen and (max-width:610px) {
  .container{
    width: 88%;
  }
  .title{
    font-size: 2.8rem;
  }
  .discription{
    font-size: 1.2rem;
    padding: 1.8rem 3rem;
  }
  .discounted-price{
    font-size: 3rem;

  }
}
@media screen and (max-width:525px) {
  .container{
    width: 95%;
  }
  .title{
    font-size: 2.5rem;
    padding: 0rem 2.7rem;

  }
  .discription{
    font-size: 1.2rem;
    padding: 1.8rem 3rem;

  }
  .discounted-price{
    font-size: 2.5rem;
  }
  .price{
    padding: 1rem 3rem;
    }
}
@media screen and (max-width:450px) {
  .container{
    width: 95%;
  }
  .title{
    font-size: 2.3rem;
    padding: 0rem 1.5rem;

  }
  .discription{
    font-size: 1.2rem;
    padding: 1.8rem 1.5rem;

  }
  .discounted-price{
    font-size: 2.3rem;
  }

  .price{
  padding: 1rem 2rem;

  }
}


@media screen and (min-width:375px) {
  .img_mob{
    display: none;
  }
}
@media screen and (max-width:375px) {
  .img_pc{
    display: none;
  }
  .container{
    flex-direction: column;
    width: 80%;
    height: 80%;
  }
  img{
    width: 100%;
    height: 50%;
    object-fit: cover;
  }
  .details{
    width: 100%;
  }
}
    </style>

    <script src="https://kit.fontawesome.com/bbcd22c396.js" crossorigin="anonymous"></script>

    <link rel="stylesheet" href="style.css">

    <title>Frontend Mentor | Product preview card component</title>

    <!-- Feel free to remove these styles or customise in your own stylesheet 👍 -->
    <style>
      
    </style>
  </head>
  <body>
    <div class="container">
      <img class="img_pc" src="./images/image-product-desktop.jpg" alt="" />
      <img class="img_mob" src="./images/image-product-mobile.jpg" alt="">
      <div class="details">
        <h1 class="heading">perfume</h1>

        <h1 class="title">Gabrielle Essence Eau De Parfum</h1>
        <p class="discription">
          A floral, solar and voluptuous interpretation composed by Olivier
          Polge, Perfumer-Creator for the House of CHANEL.
        </p>
        <div class="price">
        <h1 class="discounted-price">
          $149.99 
        </h1>
        <h3 class="checked-price">

          $169.99 
        </h3>
      </div>
      <button>
        <i class="fa-solid fa-cart-shopping"></i>
        Add to Cart
      </button>
      </div>
    </div>
  </body>
</html>
