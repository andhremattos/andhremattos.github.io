
# **Laterais**

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



## Definição 1 

Expressamos o limite a esquerda por $\dlim_{x\to a^{-}} f(x)=L$ se $\forall \varepsilon > 0, \exists \delta >0$ tal que 

$$a-\delta < x< a \Rightarrow |f(x)-L|<\varepsilon $$


## Definição 2 

Expressamos  o limite a direita por $\dlim_{x\to a^{+}} f(x)=L$ se $\forall \varepsilon > 0, \exists \delta > 0$ tal que 

$$ a< x < a+\delta \Rightarrow |f(x)-L|<\varepsilon $$ 

## Teorema 1

Se $\dlim_{x\to a^{-}} f(x)=L = \dlim_{x\to a^{+}} f(x)= L$ implica que  

$$\dlim_{x\to a} f(x)=L$$ 
	
ou seja, se os limites laterais existirem e forem iguais, o limite quando $x\to a$ existe, e é igual a $L.$ 

## Exemplo 1 

**Determine os limites laterais de**

$$f(x)=\dfrac{x}{|x|}$$ 

??? check "Solução"

    Reescrevendo a função $f$, temos 
	
    $$\Large f(x)=\dfrac{x}{|x|}=\left\{\begin{array}{ccc} 
    \dfrac{x}{x}, & \mbox{se} & x> 0 \\ 
    \dfrac{x}{-x}, & \mbox{se} & x<0 
    \end{array}	\right. $$ 
    
    $$\Large = \left\{\begin{array}{ccc}
    1, & \mbox{se} & x>0 \\ 
    -1, & \mbox{se} & x<0 
    \end{array}\right. $$

    $\Large\text{Graficamente, temos}$ 

    <center>
    <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/lateral_1.png" style="width: 50%; height: auto;"/>
    </small>
    </center>

    $\Large\text{Logo,}$ 
    
    $$\Large\dlim_{x\to 0^{-}} f(x) = \dlim_{x\to 0^{-}} -1 = -1 $$ 

    $$\Large\dlim_{x\to 0^{+}} f(x)= \dlim_{x\to 0^{+}} 1 = 1 $$ 

    $\Large\text{Assim,}$ 
    
    $$\Large\dlim_{x\to 0^{-}} f(x) \neq \dlim_{x\to 0^{+}} f(x)$$ 

    $\Large\text{Portanto,}$  $\Large\dlim_{x\to 0} f(x)$ $\Large\text{não existe.}$


## Exemplo 2 

Se 
$$f(x)=\left\{\begin{array}{ccc}
x^2, & \mbox{se} & x<0\\ 
x+5, & \mbox{se} & 0\leqslant x < 3 \\ 
x-1, & \mbox{se} & x\geqslant 3 
\end{array}\right. $$ 

Esboce o gráfico de $f(x)$ e calcule os seguintes limites:

(i) $\dlim_{x\to 0^{-}}f(x)$

(ii)$\dlim_{x\to 0^{+}}f(x)$
	
(iii) $\dlim_{x\to 0} f(x)$

(iv)$\dlim_{x\to 3^{-}} f(x)$

(v) $\dlim_{x\to 3^{+}} f(x)$

(vi) $\dlim_{x\to 3} f(x)$ 


??? check "Solução"

    $\Large\text{Primeiro vamos plotar o gráfico de}$ $\Large f(x):$

    <center>
    <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/laterais_2.png" style="width: 50%; height: auto;"/>
    </small>
    </center>

    $\Large\text{Calculando os limites, temos}$

    (i)$\Large \dlim_{x\to 0^{-}} f(x)=\dlim_{x\to 0^{-}}x^2=0$

    (ii)$\Large\dlim_{x\to 0^{+}} f(x)=\dlim_{x\to 0^{+}} x+5=5$ 

    (iii)$\Large\dlim_{x\to 0} f(x) ~\mbox{não existe, pois}~$

    $$\Large\dlim_{x\to 0^{-}}f(x)\neq \dlim_{x\to 0^{+}}f(x).$$ 

    (iv)$\Large\dlim_{x\to 3^{-}}f(x)=\dlim_{x\to 3^{-}} x+5=8$ 
    
    (v)$\Large\dlim_{x\to 3^{+}}f(x)=\dlim_{x\to 3^{+}} x-1=2$

    (vi)$\Large\dlim_{x\to 3} f(x)~ \mbox{não existe, pois}~$

    $\Large\dlim_{x\to 3^{-}}f(x)\neq \dlim_{x\to 3^{+}}f(x)$
 


## Exercícios resolvidos  

??? check "Limites laterais"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/pCW4l2uKna4"></iframe>
    </p>

??? check "Aula 2: Limites laterais"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/iz4EUNBGb1s"></iframe>
    </p>

??? check "Exercício: Limites laterais"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/ypahehpYqAs"></iframe>
    </p>

??? check "Exercício: Limites laterais"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/VAJZjBWAvj8"></iframe>
    </p>






