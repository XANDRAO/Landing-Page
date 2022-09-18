# Landing-Page
<!DOCTYPE html>
<html lang ="pt-br">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-witch, initial-scale=1.0">
        <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
        <link rel="stylesheet" href="style.css">
        <title>Landing Page</title>
    </head>
    <body>
        <div class="container">
            <header>
                <div class="logo">
                    <a href="index.html"><img src="https://user-images.githubusercontent.com/100946873/190888198-cc535941-04ad-4745-a940-2adc953a761d.png"></a>
                </div>
                 <nav>
                    <ul class="menu-list">
                        <li><a href="index.html">Pagina inicial</a></li>
                        <li><a href="#">Sobre nós</a></li>
                        <li><a href="#">Contato</a></li>
                        <li><a href="#">Entrar</a></li>
                    </ul>
                 </nav>
                 <buttonS><img src="https://user-imagemenu-icon](https://user-images.githubusercontent.com/100946873/190888204-633b64ef-244d-4982-bd73-01f87b5eaae4.png)s.githubusercontent.com/100946873/190888204-633b64ef-244d-4982-bd73-01f87b5eaae4.png"></button>
            </header>
            <main>
                <section class="main__left">
                  <h1><b>Interface</b> & Experiência</h1>
                  <p>
                    Saiba todas as diferenças Veja as característcias entre UI e UX.
                    Saiba o que são. Acesse. Saiba tudo sobre as diferenças entre UI e UX.Acesse o nosso conteúdo. Veja o Nosso Blog.
                    Sites, Sistemas e Apps. Entre em contato. 31 Anos de Atuação.
                  </p>
                  
                <div class="main__left-btn">
                    <button>Começar</button>
                    <button>Ver mais</button>
                </div>
                </section>
                <section class="main__rigth">
                    <img src="https://user-images.githubusercontent.com/100946873/190888207-1063b434-d3dc-4f9a-8b16-e9ccfe864d18.png" width="100%">


                </section>
            </main>
        </div>
        <script>
            var menu = document.querySelector('nav');
            var menuicon = document.querySelector('.menu-icon');
            var closeicon = document.querySelector('.close-icon');
            menuicon.addEventListener('click' ,()=>{
                menu.classList.add('active');
            });
            closeicon.addEventListener('click',()=>{
                    menu.classList.remove('active');
            });

        </script>
    </body>
</html>

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
    border: 0;
    outline: 0;

}
body{
    background-color: rgb(74, 94, 182);
}
.container{
    max-width: 1400px;
    display: block;
    margin: 0 auto;
    padding: 0 3%;

}
header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px;
}
header .menu-icon{
    background-color: transparent;
    cursor: pointer;
    display: none;
}
nav{
    position: relative;
}
nav .menu-list{
    list-style: none;
}
nav.menu-list.closer-icon{
    cursor: pointer;
    position: absolute;
    top: 30px;
    right: 40px;
    display: none;
}
nav.active .menu-list{
    transform: translateX(0);
}
nav .menu-list li{
    display: inline-block;
    padding: 20px;
    font-size: 20px;
}
nav .menu-list a
{
   color: white;
   text-decoration: none;
   transition: all 0.5s;
}
nav .menu-list a:hover
{
   color:  rgb(231,191,241);

}
main{
    margin-top: 30px;
    display: flex;
    align-items: center;
    justify-content: space-between;

}
main .main__left{
    color: white;
    width: 50%;
    padding: 20px;
}
main .main__left h1{
    font-size: 4rem;
    font-weight: lighter;
    letter-spacing: 1px;
}
main .main__left p{
    font-size: 22px;
    margin: 40px 0;
}
main .main__left-btn button{
    padding: 10px 20px;
    cursor: pointer;
    font-size:  16px;
    margin: 10px;
    border-radius: 20px;
    font-weight: 500;
    box-shadow: 0 20px 35px rgb(0, 0, 0,10%),0 15px 12px rgb(0, 0, 0,8%);
}
main .main__left-btn button:nth :nth-child(1){
    background: rgb(192, 115, 255);
    color: rgb(19, 6, 42);
    transition: all 0.5s;
    
}
main .main__left-btn button:nth :nth-child(1):hover {
    background-color: rgb(161, 59, 255);
}
main .main__left-btn button:nth :nth-child(2){
    background: rgb(192, 115, 255);
    color: white;
    border: 1px solid white;
    transition: all 0.5s;
}
main .main__left-btn button:nth:nth-child(2):hover{
    background-color: white;
    color: rgb(116, 59, 245);
}
main .main__left__right{
    padding-right: 50px;
}
@media (max-width:800px){
    nav .menu-list .close-icon,
    header .menu-icon{
        display: block;
    }
      nav .menu-list{   
      position: fixed;
      top: 0;
      right: 0;
      width: 0;
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      transform: translateX(100%);
      transition: 0.5s;
      background-color: rgba(116, 0, 214)
     }
     nav .menu-list li{
        font-size: 30px;
     }
     main{
        flex-wrap: wrap;
     }
     main .main__left{
        width: 100%;
        text-align: center;
        padding: 50px;
     }
     main .main__left h1{
        font-size: 3rem;
     }
     main .main__right{
        width: 100px;
        margin: 50px 10px;
     }
}
