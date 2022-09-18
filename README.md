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
                 <buttonS><img src="https://user-images.githubusercontent.com/100946873/190888207-1063b434-d3dc-4f9a-8b16-e9ccfe864d18.png"></button>
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

