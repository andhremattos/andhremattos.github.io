# **Listas de Exercícios - Integral**

:material-cursor-default-click-outline: Clique no botão abaixo para alternar visualização:

<div class="tx-switch">
  <button data-md-color-scheme="default"><code>Visualização normal</code></button>
  <button data-md-color-scheme="slate"><code>Visualização contraste</code></button>
</div>

<script>
  var buttons = document.querySelectorAll("button[data-md-color-scheme]")
  buttons.forEach(function(button) {
    button.addEventListener("click", function() {
      var attr = this.getAttribute("data-md-color-scheme")
      document.body.setAttribute("data-md-color-scheme", attr)
      var name = document.querySelector("#__code_0 code span:nth-child(7)")
      name.textContent = attr
    })
  })
</script>

<style>
p.combinado:first-letter { 
	color: #F5843A; 
	font-size:xx-large; 
}
.info {
  background-color: #e7f3fe;
  border-left: 6px solid #2196F3;
}
.success {
  background-color: #ddffdd;
  border-left: 6px solid #4CAF50;
}

.danger {
  background-color: #ffdddd;
  border-left: 6px solid #f44336;
}
</style>


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




**Em breve** 

<!-- 
!!! tip "Videoaula 1"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/kJYLWFwfL80"></iframe>
    </p>

!!! abstract "Instalação dos programas MiKTeX e TeXstudio"
    
    **Instalação do TeXstudio**: 

    Acesse texstudio.org ou digite no seu navegador de preferência, ou seja, dá um google em "texstudio", normalmente é o primeiro resultado que aparece na pesquisa. $f(x)$

    Ao clicar, você será levado a página de baixar em função do seu sistema operacional. Basta clicar e aguardar o download. 


## Exercício A 

1. Determine a função derivada de $f(x) = x^4 - \sin(x) + \frac{x^{-2}}{-\pi}$ 

**Solução:** 

Temos que $f(x)$ é uma junção de dois tipos de funções, função polinomial com função trigonométrica. Para derivar $f(x)$ basta utilizar a propriedade básica: 

$$f(x) = x^4 - \sin(x) + \frac{x^{-2}}{-\pi}$$ 

$$ f'(x) = 4x^3 - \cos(x) + \left( \frac{-2x^{-1}}{-\pi} \right)$$ 

$$ f'(x) = 4x^3 - \cos(x) + \displaystyle\frac{2x^{-1}}{\pi} $$ 

Que podemos ainda reescrever, ficando 

$$ f'(x) = 4x^3 - \cos(x) + \frac{2}{\pi x} $$ 

## Fundamento legal - obrigatoriedade

<p style="text-align: justify;">
A determinação legal decorre do artigo 67 da Lei 8.666/93. O Artigo 58, inciso III da citada Lei
assegura à Administração a prerrogativa de fiscalizar os contratos.

</p>
-->




