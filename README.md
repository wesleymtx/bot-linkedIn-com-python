<h2>Sobre</h2>
<hr>
Quando você visualiza o perfil do usuário no LinkedIn, ele é notificado de que você consultou o perfil dele. Esse bot permitirá que você visualize os perfis dos usuários, aumentando assim a sua visibilidade na sua rede sugerida no LinkedIn.
<p align="center">
<a target="_blank" rel="noopener noreferrer" href="https://camo.githubusercontent.com/bfb65c087b5f232183b8b57a725d988cae470dc9/68747470733a2f2f707265766965772e6962622e636f2f6d4d4475416b2f6c696e6b65645f496e5f426f745f50726f66696c655f566965775f526573756c74732e706e67"><img src="https://camo.githubusercontent.com/bfb65c087b5f232183b8b57a725d988cae470dc9/68747470733a2f2f707265766965772e6962622e636f2f6d4d4475416b2f6c696e6b65645f496e5f426f745f50726f66696c655f566965775f526573756c74732e706e67" alt="Resultado do LinkedIn" width="325" height="200" data-canonical-src="https://preview.ibb.co/mMDuAk/linked_In_Bot_Profile_View_Results.png" style="max-width:100%;"></a>
</p>
<h2>Exigências</h2>
<hr>
<p>
  Importante: verifique se sua Configuração de visualização de perfil foi alterada de 'Anônimo' para 'Público' para que os membros do LinkedIn possam ver que você os visitou e que podem visitar seu perfil em troca. Você também deve alterar sua configuração de idioma para inglês .

O LinkedInBot foi desenvolvido no Pyhton 2.7 .

Antes de executar o bot, você precisará instalar algumas dependências do Python.

Nota: Python 2.7.9 e posterior (na série python2) e Python 3.4 e posterior incluem pip por padrão, portanto, você já deve ter o pip. Caso contrário, você pode instalar o easy_install sudo apt-get install python-setuptools para instalar o pip sudo easy_install pip .

<ul>
<li><a href="https://pypi.python.org/pypi/beautifulsoup4" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">BeautifulSoup4</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> , para analisar html:</font></font><code>pip install BeautifulSoup4</code></li>
<li><a href="http://www.seleniumhq.org/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Selenium</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> , para automação do navegador:</font></font><code>pip install Selenium</code></li>
</ul>
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
<pre><span class="pl-c"># Configurable Constants</span>
<span class="pl-v">EMAIL</span> <span class="pl-c1">=</span> <span class="pl-s">'youremail@gmail.com'</span>
<span class="pl-v">PASSWORD</span> <span class="pl-c1">=</span> <span class="pl-s">'password'</span>
<span class="pl-v">VIEW_SPECIFIC_USERS</span> <span class="pl-c1">=</span> <span class="pl-c1">False</span>
<span class="pl-v">SPECIFIC_USERS_TO_VIEW</span> <span class="pl-c1">=</span> [<span class="pl-s">'CEO'</span>, <span class="pl-s">'CTO'</span>, <span class="pl-s">'Developer'</span>, <span class="pl-s">'HR'</span>, <span class="pl-s">'Recruiter'</span>]
<span class="pl-v">NUM_LAZY_LOAD_ON_MY_NETWORK_PAGE</span> <span class="pl-c1">=</span> <span class="pl-c1">5</span>
<span class="pl-v">CONNECT_WITH_USERS</span> <span class="pl-c1">=</span> <span class="pl-c1">True</span>
<span class="pl-v">RANDOMIZE_CONNECTING_WITH_USERS</span> <span class="pl-c1">=</span> <span class="pl-c1">True</span>
<span class="pl-v">JOBS_TO_CONNECT_WITH</span> <span class="pl-c1">=</span> [<span class="pl-s">'CEO'</span>, <span class="pl-s">'CTO'</span>, <span class="pl-s">'Developer'</span>, <span class="pl-s">'HR'</span>, <span class="pl-s">'Recruiter'</span>]
<span class="pl-v">ENDORSE_CONNECTIONS</span> <span class="pl-c1">=</span> <span class="pl-c1">False</span>
<span class="pl-v">RANDOMIZE_ENDORSING_CONNECTIONS</span> <span class="pl-c1">=</span> <span class="pl-c1">True</span>
<span class="pl-v">VERBOSE</span> <span class="pl-c1">=</span> <span class="pl-c1">True</span></pre>

<h2>Rodar</h2>
<hr>
<p>
Depois de instalar as dependências necessárias e editar o configarquivo, você pode executar o bot.

Verifique se você está na pasta correta e execute o seguinte comando: python LinkedInBot.py

Depois de escolher o seu navegador favorito, o bot começará a visitar perfis.
</p>

<h2>Resultado</h2>
<hr>
<p>
T: Número de perfis que o bot tentou acessar;

V: Número de perfis que o bot realmente visitou (perfis que você pode acessar: classificação 3 ou menos);

Q: Número de perfis na fila.
</p>

<h2>Aprimoramentos</h2>
<hr>
  <p>Por favor, sinta-se à vontade para me enviar uma mensagem ou abrir um problema se você tiver uma idéia para uma melhoria! Parece que as pessoas estão começando a usar isso e eu gostaria de melhorá-lo.</p>
