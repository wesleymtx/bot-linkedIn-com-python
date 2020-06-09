<h2>Sobre</h2>
<hr>
Quando você visualiza o perfil do usuário no LinkedIn, ele é notificado de que você consultou o perfil dele. Esse bot permitirá que você visualize os perfis dos usuários, aumentando assim a sua visibilidade na sua rede sugerida no LinkedIn.
<p align="center">
<a target="_blank" rel="noopener noreferrer" href="https://camo.githubusercontent.com/bfb65c087b5f232183b8b57a725d988cae470dc9/68747470733a2f2f707265766965772e6962622e636f2f6d4d4475416b2f6c696e6b65645f496e5f426f745f50726f66696c655f566965775f526573756c74732e706e67"><img src="https://camo.githubusercontent.com/bfb65c087b5f232183b8b57a725d988cae470dc9/68747470733a2f2f707265766965772e6962622e636f2f6d4d4475416b2f6c696e6b65645f496e5f426f745f50726f66696c655f566965775f526573756c74732e706e67" alt="Resultado do LinkedIn" width="325" height="200" data-canonical-src="https://preview.ibb.co/mMDuAk/linked_In_Bot_Profile_View_Results.png" style="max-width:100%;"></a>
</p>
<h2>Exigências</h2>
<hr>
<h2>Exigências</h2>
<p>
  Importante: verifique se sua Configuração de visualização de perfil foi alterada de 'Anônimo' para 'Público' para que os membros do LinkedIn possam ver que você os visitou e que podem visitar seu perfil em troca. Você também deve alterar sua configuração de idioma para inglês .

O LinkedInBot foi desenvolvido no Pyhton 2.7 .

Antes de executar o bot, você precisará instalar algumas dependências do Python.

Nota: Python 2.7.9 e posterior (na série python2) e Python 3.4 e posterior incluem pip por padrão, portanto, você já deve ter o pip. Caso contrário, você pode instalar o easy_install sudo apt-get install python-setuptools para instalar o pip sudo easy_install pip .

BeautifulSoup4 , para analisar html:pip install BeautifulSoup4
Selenium , para automação do navegador:pip install Selenium
Se você planeja usar o Firefox (ou Iceweasel), não precisa de mais nada.

Para o Chrome, primeiro obtenha o driver da web e coloque-o na mesma pasta que o bot, se você estiver no Windows, ou na /usr/binpasta se estiver no OS X.

PhantomJS:

No Windows, baixe o binário no site oficial e coloque-o na mesma pasta que o bot.
No OS X Yosemite, o binário fornecido pela equipe do PhantomJS não funciona ( selenium.common.exceptions.WebDriverException: Mensagem: 'Não é possível conectar ao GhostDriver' ). Você pode compilá-lo sozinho ou baixar o binário fornecido pelo incrível eugene1g . Em seguida, coloque-o na /usr/binpasta
É o mesmo para o Raspbian: compile-o e coloque-o na /usr/binpasta ou baixe o binário fornecido pelo incrível fg2it .
Se você deseja criar seus próprios binários, aqui estão as instruções de construção para o PhantomJS.

Configuração
Antes de executar o bot, edite a parte de configuração do script. Isso incluirá as informações de login da sua conta (email, senha etc.) e outros valores lógicos para tornar o bot mais seu. É simples assim!

# Configuração
EMAIL = 'youremail@gmail.com'
PASSWORD = 'password'
VIEW_SPECIFIC_USERS = False
SPECIFIC_USERS_TO_VIEW = ['CEO', 'CTO', 'Developer', 'HR', 'Recruiter']
NUM_LAZY_LOAD_ON_MY_NETWORK_PAGE = 5
CONNECT_WITH_USERS = True
RANDOMIZE_CONNECTING_WITH_USERS = True
JOBS_TO_CONNECT_WITH = ['CEO', 'CTO', 'Developer', 'HR', 'Recruiter']
ENDORSE_CONNECTIONS = False
RANDOMIZE_ENDORSING_CONNECTIONS = True
VERBOSE = True
</p>
