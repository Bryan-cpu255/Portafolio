# Portafolio
<!DOCTYPE html!>

<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MY PERSONAL WEBSITE</title>
    <link rel="stylesheet" href="HomePage.css">
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
</head>
<body>
    <nav class="navbar">
    <div class="max-width">
    <div class="logo"><a href="#">Portafo<span>lio.</span></a></div>    
        <ul class="menu">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Skills</a></li>
        <li><a href="#">Teams</a></li>
        <li><a href="#">Contact</a></li>
        </ul>
        <div class="menu-btn">
        <i class="fas fa-bars"></i>
        </div>
    </div>
    </nav>
    <!-- Home section start-->
    <section class="home" id="home">
    <div class="max-width">
    <div class="home-content">
    <div class="text-1">Hello, My name is:</div> 
    <div class="text-2">Bryan Eduardo Cos Palma</div>    
    <div class="text-3">And I'm <span>Student</span></div>    
    </div>    
    </div>
    </section>
    <p>Con que me quieres conocer bueno me presento: me llamo Bryan tengo 17 años de 1.70, me considero un poco introvertido, en parte inteligente y algo curioso pues me gusta indagar mucho en aquello que me interese y esa es una de las razones por las que estoy aqui, en esta carrera porque logro llamar mi atencion y aunque hay veces en que no me salen las cosas me agrada la carrera pues no voy a mejorar si no aprendo de mis errores es mas ustedes podrian comparar mi primer diseño a este al que ven en pantalla y me enorgullezco de mi mismo.Abajo encontraran mas informacion sobre mi, mis gustos, mis trabajos y demas.</p>
    <script src="Script.js"></script>
</body>

</html>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Ubuntu:wght@400;500;700&display=swap');
</style>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
}
.max-width{
    max-width: 1300px;
    padding: 0 80px;
    margin: auto;
}
/* navbar styling*/

.navbar{
    position: fixed;
    width: 100%;
    padding: 30px 0;
    font-family: "Ubuntu",sans-serif;
    transition: all 0.3s ease;
}
.navbar.sticky{
    padding: 15px 0;
    background: crimson; 
}
.navbar .max-width{
    display: flex;
    align-items: center;
    justify-content:space-between;
}
.navbar .logo a{
    color: #fff;
    font-size: 35px;
    font-weight: 600;
}
.navbar .logo a span{
    color: crimson;
    transition: all 0.3s ease;
}
.navbar.sticky .logo a span{
    color: #fff;
}
.navbar .menu li{
    list-style: none;
    display: inline-block;
}
.navbar .menu li a{
    color: #fff;
    font-size: 18px;
    font-weight: 500;
    margin-left: 25px;
    transition: color 0.3s ease;
}
.navbar .menu li a:hover{
    color: crimson;
}
.navbar.sticky .menu li a:hover{
    color: #fff;
}
/*menu btn styling*/
.menu-btn{
    color: #fff;
    font-size: 23px;
    cursor: pointer;
    display: none;
}
/* home section styling*/
.home{
    display: flex;
    background: url(Banner.png)no-repeat center;
    height: 100vh;
    color: #fff;
    min-height: 500px;
    font-family: "Ubuntu", sans-serif;
}
.home .max-width{
    margin: auto 0 auto 40px;
}
.home .home-content .text-1{
    font-size: 27px;
}
.home .home-content .text-2{
    font-size: 75px;
    font-weight: 600px;
    margin-left: -3px;
}
.home .home-content .text-3{
    font-size: 40px;
    margin: 5px 0;
}
.home .home-content .text-3 span{
    color: crimson;
    font-weight: 500;
}

/*responsive media query start*/

@media (max-width: 947px){
    .menu-btn{
    display: block;
    z-index: 999;
}
    .max-width{
    padding: 0 50px;
    }
    .navbar .menu{
        position: fixed;
        height: 100vh;
        width: 100%;
        left: -100%;
        top: 0;
        background: #111;
        text-align: center;
        padding-top: 80px;
    }
    .navbar .menu.active{
        left: 0;
    }
    .navbar .menu li{
        display:block;
    }
    .navbar .menu li a{
        display: inline-block;
        margin: 20px 0;
        font-size: 25px;
    }
}
