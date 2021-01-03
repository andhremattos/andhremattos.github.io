
# **Indeterminados**

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

## Limites Indeterminados 

Temos que  

1. $\displaystyle\lim_{x\to a} \displaystyle\frac{f(x)}{g(x)}$

Aplicando a propriedade, resulta em: 

$$ \displaystyle\frac{\displaystyle\lim_{x\to a}f(x)}{\displaystyle\lim_{x\to a}g(x)}$$

Quando fizermos $x \to a$ resultar em $f(x) \to 0$, $g(x) \to 0$; $f(x) \to \infty$ e $g(x) \to \infty$, 
resultaria em um quociente dos tipos: 

$$ \displaystyle\frac{``0"}{0}$$ 

e 

$$ \displaystyle\frac{``\infty"}{\infty}$$

Que são expressões onde não é possível determinarmos um valor para elas, logo são ditas expressões indeterminadas. Muitos limites após fazermos $x\to a$ podem resultar em uma dessas expressões, para estes limites, respeitando especificidades, teremos que utilizar de procedimentos algébricos e manipulações matemáticas adequadas para "**Retirar**" a indeterminação, para assim, calcularmos o limite. 

O mesmo acontece, com expressões do tipo 

$$`` \infty - \infty "$$ 


## Exemplo 1 

**Calcule $\displaystyle\lim_{x\to 1} \left[\displaystyle\frac{1}{1-x}-\dfrac{3}{1-x^3}\right]$.**

??? check "Solução"

    Fazendo $x\to 1$, temos 

    $$\Large\displaystyle\lim_{x\to 1} \left[\displaystyle\frac{1}{1-x}-\displaystyle\frac{3}{1-x^3}\right]$$
    
    $$ \Large=\left[\displaystyle\frac{1}{1-1}-\displaystyle\frac{3}{1-(1)^3}\right]$$
    
    $$ \Large= \left[\displaystyle\frac{1}{0}-\displaystyle\frac{3}{0}\right] $$ 
    
    $$ \Large= \infty-\infty \rightarrow \mbox{Indeterminação} $$ 

    Resolvendo essa diferença de frações, obtemos 

    $$\Large=\displaystyle\lim_{x\to 1} \left[\displaystyle\frac{1-x^3-3(1-x)}{(1-x)(1-x^3)}\right]$$

    $$\Large=\displaystyle\lim_{x\to 1} \left[\displaystyle\frac{-x^3+3x-2}{(1-x)(1-x^3)}\right]$$  

    Precisamos retirar a indeterminação, para isso vamos fatorar os polinômios do numerador e denominador. 

    Para o numerador, temos $x^3+3x-2$, como temos uma das raízes, fatoramos usando o dispositivo de Briot Ruffini, 

    $$\Large\begin{array}{c|cccc}
    1 & -1 & 0 & 3 & -2 \\ \hline 
    & -1 & -1 & 2 & 0 
    \end{array}$$ 

    Assim, temos 

    $$ \Large=\displaystyle\lim_{x\to 1} \displaystyle\frac{(x-1)(-x^2-x+2)}{-(x-1)(1-x^3)}$$ 

    $$ \Large=\displaystyle\lim_{x\to 1} \displaystyle\frac{-x^2-x+2}{-(1-x^3)}$$ 

    Fazendo novamente $x\to 1$, temos 

    $$ \Large=\displaystyle\lim_{x\to 1} \displaystyle\frac{-x^2-x+2}{-(1-x^3)}$$ 
    
    $$ \Large=\displaystyle\frac{0}{0} \rightarrow \mbox{Indeterminação}$$ 

    Fatorando novamente usando Ruffini, 

    $$ \Large\begin{array}{c|ccc}
    1 & -1 & -1 & 2\\ \hline 
    & -1 & -2 & 0 
    \end{array}$$ 


    Assim, 

    $$\Large=\displaystyle\lim_{x\to 1} \displaystyle\frac{ (x-1)(-x-2)}{(x-1)(x^2+x+1)}$$ 

    $$\Large=\displaystyle\lim_{x\to 1} \displaystyle\frac{-x-2}{x^2+x+1}= \displaystyle\frac{-3}{3}=-1$$

## Exercício resolvido 1 

**Determine o seguinte limite**: 
$$ \dlim_{x\to 0} \dfrac{1 - \sqrt[3]{1-x}}{x}$$ 

??? check "Limite Indeterminado"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/mWnO5a8S9v4"></iframe>
    </p>

## Exercício resolvido 2 

**Determine o seguinte limite**: 
$$ \dlim_{x\to 2} \dfrac{x^2-4}{x-2}$$ 

??? check "Limite Indeterminado 2"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/h26QwqUgmLc"></iframe>
    </p>

## Exercício resolvido 3 

**Determine o seguinte limite**: 
$$ \dlim_{x\to 0} \dfrac{\sqrt{\cos(x)} - \sqrt[3]{\cos(x)}}{\text{sen}^2(x)}$$ 

??? check "Limite Indeterminado 4"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/au8dFcsEBmE"></iframe>
    </p>

## Exercício resolvido 4

**Determine o seguinte limite**: 
$$ \dlim_{x\to \dfrac{\pi}{6}} \dfrac{2\text{sen}^2(x) + \text{sen}(x) - 1}{2\text{sen}^2(x) - 3\text{sen}(x) + 1}$$ 

??? check "Limite Indeterminado 5"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/n5axuGG8sQc"></iframe>
    </p>








