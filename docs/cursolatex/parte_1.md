

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
<div class="warning">
  <span class="closebtn" onclick="this.parentElement.style.display='none';">&times;</span> 
  <strong>Informe:</strong> começa sexta-feira, 27 de março, às 21h, com as primerias videoaulas liberadas!</a>
</div>
</div>

## Instalação do MiKTeX no Windows

Após baixar o programa, basta seguir as orientações que aparecem na tela. Teremos uma videoaula mostrando o processo de instalação. 

## Instalação do TeXstudio no Windows 
Após baixar o programa, basta também seguir as orientações que aparecem na tela. 


<!--
## **Licença**

<center> <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img src="../../images/CC.jpg" style="width:200px;height:70px"/></a></center>
<center> <p>Esta obra está sob licença <em>Creative Commons</em> CC BY-NC-SA 4.0: esta licença
permite que outros remixem, adaptem e criem a partir do seu trabalho para fins não
comerciais, desde que atribuam o devido crédito e que licenciem as novas criações
sob termos idênticos.</p>
-->