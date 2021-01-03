
# **Definição**

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


input[type='checkbox'] { display: none; } .wrap-collabsible { margin: 1.2rem 0; } .lbl-toggle { display: block; font-weight: bold; font-family: monospace; font-size: 1.2rem; text-transform: uppercase; text-align: center; padding: 1rem; color: #DDD; background: #0069ff; cursor: pointer; border-radius: 7px; transition: all 0.25s ease-out; } .lbl-toggle:hover { color: #FFF; } .lbl-toggle::before { content: ' '; display: inline-block; border-top: 5px solid transparent; border-bottom: 5px solid transparent; border-left: 5px solid currentColor; vertical-align: middle; margin-right: .7rem; transform: translateY(-2px); transition: transform .2s ease-out; } .toggle:checked+.lbl-toggle::before { transform: rotate(90deg) translateX(-3px); } .collapsible-content { max-height: 0px; overflow: hidden; transition: max-height .25s ease-in-out; } .toggle:checked + .lbl-toggle + .collapsible-content { max-height: 350px; } .toggle:checked+.lbl-toggle { border-bottom-right-radius: 0; border-bottom-left-radius: 0; } .collapsible-content .content-inner { background: rgba(0, 105, 255, .2); border-bottom: 1px solid rgba(0, 105, 255, .45); border-bottom-left-radius: 7px; border-bottom-right-radius: 7px; padding: .5rem 1rem; } .collapsible-content p { margin-bottom: 0; }
</style>

<!-- 
![Legenda](../imagens/capitulo.png)
--> 






<!-- 
<div class="card">
<div class="info">
  <span class="closebtn" onclick="this.parentElement.style.display='none';">&times;</span> 
  <strong>Informe:</strong> Modelo de informe</a>
</div>
</div>
-->

## Limite de uma Função 

**Definição**: Seja $y = f(x)$ uma função definida na vizinhaça do ponto $a$ ou também em certos pontos desta
vizinhança. Dizemos que tal função $f$ possui um limite finito $L$ quando $x$ tende para um valor de $a$, se para cada número positivo $\epsilon$, por menor que seja, existe em correspondência um número positivo $\delta$, tal que para $|x-a| < \delta$, tenhamos $|f(x)-L| < \epsilon$, para todo $x$. Assim, como você já deve ter percebido a letra $L$ aqui representa o limite de uma função $f(x)$ quando $x$ tende para $a$, e escrevemos 

$$ \displaystyle\lim_{x\to a} f(x) = L $$ 

### Exemplo 1 

**Mostre pela definição de limite que $\displaystyle\lim_{x\to 2} 3x+1=7.$**


!!! abstract "Solução"
    
    Aplicando a definição, temos que para todo $\epsilon > 0$ existe um $\delta > 0$ tal que 

    $$ | x-2| <\delta \Rightarrow |(3x+1)-7| < \epsilon $$ 

    Desenvolvendo, 

    Multiplicando em ambos os membros por 3 unidades, resulta em: 
  
    $$ | x - 2 | < \delta \Rightarrow 3\cdot |x-2| < 3\delta $$ 

    Como 3 unidades é positivo, podemos escrever |3|, resulta em: 

    $$ \Leftrightarrow |3|\cdot |x-2| < 3\delta $$ 

    Usando propriedades, o produto de módulos e módulo do produto, resulta em: 

    $$ \Leftrightarrow |3\cdot (x-2)| < 3\delta $$ 

    Desenvolvendo o produto, resulta em: 

    $$ \Leftrightarrow |3x-6| < 3\delta $$ 

    Veja que podemos reescrever o número -6 como sendo -7+1, este é um artifício para podermos chegarmos na expressão, resulta em: 

    $$ \Leftrightarrow |3x+(1-7)| < 3\delta $$ 

    Comparando com o enunciado da prova, resulta em: 

    $$ \Leftrightarrow |3x+1-7| < 3\delta $$

    Reeorganizando, resulta em: 

    $$ \Leftrightarrow |(3x+1)-7| < 3\delta $$ 

    Como, $|(3x+1)-7| < \epsilon$ e encontramos que $|(3x+1)-7| < 3\delta$, temos que os lados esquerdos das duas expressões são iguais, como temos uma desiguldade, implica que o lado direito das duas expressões também são iguais, logo 

    $$ 3\delta = \epsilon$$ 

    $$ \Leftrightarrow \delta = \displaystyle\frac{\epsilon}{3}$$

    Portanto, para $\displaystyle\lim_{x\to 2} 3x+1=7$ bsta tomarmos um $\delta = \displaystyle\frac{\epsilon}{3}$.

### Exemplo 2 


**Mostre que $\displaystyle\lim_{x\to 3} x^2=9$.**


!!! abstract "Solução"

    Temos que 
	
	  $$ \\displaystyle\lim_{x\to 3} x^2=9 \Leftrightarrow $$ 
    
    $$ \forall \varepsilon >0, \exists ~ \delta >0 ~| $$
    
    $$ ~ 0<|x-3|<\delta \Rightarrow |x^2-9|< \varepsilon$$ 
	
	  Desenvolvendo, 
	
	  $$|x^2-9|<\varepsilon $$ 
    
    $$\Leftrightarrow |(x-3)(x+3)|< \varepsilon $$ 
	
	  $$\Leftrightarrow |x-3||x+3| < \varepsilon $$ 

    Supondo que $\delta \leqslant 1$
	
	  $$ |x-3|\leqslant 1 $$ 
    
    $$\Leftrightarrow -1\leqslant x-3\leqslant 1$$ 

	  Somando $6$ unidades em ambos os membros, 
	
	  $$ -1+6 \leqslant x-3+6 \leqslant 1+6 $$ 
	
	  $$ 5 \leqslant x+3\leqslant 7 $$ 
	
	  Logo, 
	
	  $$ |x+3|< 7 $$ 
	
	  Assim, $|x^2-9|=|x-3||x+3| < \delta \cdot 7 = \varepsilon$
	
	  Resultando em 
	
	  $$ \delta =\frac{\epsilon}{7} $$ 
	
	  Portanto, tome $\delta = \mbox{min}\left(1,\dfrac{\varepsilon}{7}\right)$.


### Exercício em vídeo

**Mostre pela definição de limite que $\displaystyle\lim_{x\to 1} \displaystyle\frac{1}{(1-x)^2} = + \infty$**.
<div class="wrap-collabsible"> <input id="collapsible" class="toggle" type="checkbox"> <label for="collapsible" class="lbl-toggle">Solução</label>
<div class="collapsible-content">
<div class="content-inner">
<p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/wk7SOi2bgXQ"></iframe>
    </p>
</div>
</div>
</div>


<!-- 
!!! tip "Videoaula 1"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/kJYLWFwfL80"></iframe>
    </p>

!!! abstract "Instalação dos programas MiKTeX e TeXstudio"
    
    **Instalação do TeXstudio**: 

    Acesse texstudio.org ou digite no seu navegador de preferência, ou seja, dá um google em "texstudio", normalmente é o primeiro resultado que aparece na pesquisa. 

    Ao clicar, você será levado a página de baixar em função do seu sistema operacional. Basta clicar e aguardar o download. 


## Fundamento legal - obrigatoriedade

<p style="text-align: justify;">
A determinação legal decorre do artigo 67 da Lei 8.666/93. O Artigo 58, inciso III da citada Lei
assegura à Administração a prerrogativa de fiscalizar os contratos.

</p>
-->




