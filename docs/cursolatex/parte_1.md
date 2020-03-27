

# **Parte 1 - Instalação dos programas básicos para uso do LaTeX** 

<style>
p.combinado:first-letter { 
	color: #F5843A; 
	font-size:xx-large; 
}

.button {
  border-radius: 20px;
  background-color: #009688;
  border: none;
  color: #FFFFFF;
  text-align: center;
  font-size: 15px;
  padding: 10px;
  width: 150px;
  transition: all 0.5s;
  cursor: pointer;
  margin: 5px;
}


.button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.button span:after {
  content: '\00bb';
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.button:hover span {
  padding-right: 25px;
}

.button:hover span:after {
  opacity: 1;
  right: 0;
}	

/** AVISOS **/
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  border-radius: 50px;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

.alert {
  padding: 12px;
  background-color: #f44336;
  color: white;
  border-radius: 50px;
}

.success {
  padding: 12px;
  background-color: #6BBD6E;
  color: white;
  border-radius: 50px;
}

.info {
  padding: 12px;
  background-color: #47A8F5;
  color: white;
  border-radius: 50px;
}

.warning {
  padding: 12px;
  background-color: #FFAA2C;
  color: white;
  border-radius: 50px;
}

.closebtn {
  margin-left: 25px;
  color: white;
  font-weight: bold;
  float: right;
  font-size: 22px;
  line-height: 25px;
  cursor: pointer;
  transition: 0.3s;
}

.closebtn:hover {
  color: black;
}

/** ANOTAÇÕES **/

.atencao {
  background-color: #ffdddd;
  border-left: 6px solid #f44336;
  margin-bottom: 15px;
  padding: 4px 12px;
}

.sucesso {
  background-color: #ddffdd;
  border-left: 6px solid #4CAF50;
  margin-bottom: 15px;
  padding: 4px 12px;
}

.informacao {
  background-color: #e7f3fe;
  border-left: 6px solid #2196F3;
  margin-bottom: 15px;
  padding: 4px 12px;
}


.atento {
  background-color: #ffffcc;
  border-left: 6px solid #ffeb3b;
  margin-bottom: 15px;
  padding: 4px 12px;
}
</style>

<div class="card">
<div class="info">
  <span class="closebtn" onclick="this.parentElement.style.display='none';">&times;</span> 
  <strong>Informe:</strong> Videoaula liberada!</a>
</div>
</div>


!!! tip "Videoaula 1"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/kJYLWFwfL80"></iframe>
    </p>

!!! abstract "Instalação dos programas MiKTeX e TeXstudio"
    
    **Instalação do TeXstudio**: 

    Acesse texstudio.org ou digite no seu navegador de preferência, ou seja, dá um google em "texstudio", normalmente é o primeiro resultado que aparece na pesquisa. 

    Ao clicar, você será levado a página de baixar em função do seu sistema operacional. Basta clicar e aguardar o download. 


    **Instalação do MiKTeX**: 

    Acesse miktex.org ou digite no seu navegador de preferência, ou seja, dá um google em "miktex", normalmente é o primeiro resultado que aparece na pesquisa.

    Ao entrar na página, você terá logo a opção de baixar um tipo de instalador. Não instale usando o instalador sugerido, vá até  "all downloads" e escolha a opção em função do seu sistema operacional. 

    Agora é a hora de escolher a instalação _basic_ ou _net_ e se é 32bit ou 64bit. Neste tutorial, minha recomendação é utilizar a opção _net_. Clique em baixar e aguarde. 

    Após baixar, dê um clique e autorize a instalação no computador, a segunda tela que aparecerá é para concordar com os termos de instalação, clique na caixa indicada, depois em _net_ (próximo). 

    **Atenção**: O MiKTeX tem duas etapas para sua completa instalação. Primeiro você irá baixar os pacotes em seu computador. Depois fará a instalação usando os pacotes baixados inicialmente. 

    Vamos lá, escolha _download_ e depois o local onde será o _download_, em seguida você vai escolher o distribuidor em função do país, as primeiras opções são do Brasil, da USP, clique na opção que tem **HTTP** e depois em _net_. Aguarde o _download_. Demora de 40min a 1h 30min. 

    Agora é hora de fazer a instalação. Clique novamente no arquivo **setup.exe** do MiKTeX e siga com _net_ escolhendo a versão completa e se será somente para seu usuário do computador ou para os demais. Busce a pasta onde você baixou os pacotes e siga com _net_. Aguarde, vai demorar bastante! 

    Após as etapas você já tem o "sitema" LaTeX instalado no seu computador. Tendo dúvidas, fique a vontade para me indagar pelo WhatsApp ou Telegram. 


<!--
## **Licença**

<center> <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img src="../../images/CC.jpg" style="width:200px;height:70px"/></a></center>
<center> <p>Esta obra está sob licença <em>Creative Commons</em> CC BY-NC-SA 4.0: esta licença
permite que outros remixem, adaptem e criem a partir do seu trabalho para fins não
comerciais, desde que atribuam o devido crédito e que licenciem as novas criações
sob termos idênticos.</p>
-->