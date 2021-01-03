
# **Função Derivada**

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




A função derivada de uma função $g=f(x)$ é a função $f'(x)$, (lê-se $f$ linha de $x$) tal que seu valor em qualquer $x \in \mbox{D}(f)$ é dado por 

$$ f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ f(x+\Delta x)-f(x)}{\Delta x}$$ 

$$= \displaystyle\lim_{x\to x_0} \frac{ f(x)-f(x_0)}{x-x_0}$$ 


### Exemplo 1 

Determine $f'(x)$, onde $f(x)=\sqrt{2x+1}$. 



??? check "Solução"
  
    $\Large \text{Temos}$ 

    $$\Large f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ \sqrt{2(x+\Delta x)+1}-\sqrt{2x+1}}{\Delta x}$$ 
	
	$$\Large f'(x) = \displaystyle\lim_{\Delta x\to 0} \frac{ (\sqrt{2(x+\Delta x)+1}-\sqrt{2x+1})(\sqrt{2(x+\Delta x)+1}+\sqrt{2x+1})}{\Delta x(\sqrt{2(x+\Delta x)+1}+\sqrt{2x+1})} $$ 
	
	$$\Large f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ 2(x+\Delta x)+1-2x-1}{\Delta x(\sqrt{2(x+\Delta x)+1}+\sqrt{2x+1})} $$ 
	
	$$\Large f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ 2x+2(\Delta x)+1-2x-1}{\Delta x (\sqrt{2(x+\Delta x)+1}+\sqrt{2x+1})} 	$$ 
	
	$\Large\text{Simplificando,}$ 
	
	$$\Large f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ 2(\Delta x)}{\Delta x (\sqrt{2(x+\Delta x)+1}+\sqrt{2x+1})}$$ 
	
	
	$$\Large f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ 2}{ (\sqrt{2(x+\Delta x)+1}+\sqrt{2x+1})}$$
	
	$$\Large f'(x)=\frac{2}{(\sqrt{2x+1}+\sqrt{2x+1})}$$

	$$\Large f'(x)=\frac{2}{2\sqrt{2x+1}} = \frac{1}{\sqrt{2x+1}}$$ 



### Exemplo 2 

Determine $f'(x)$, sabendo que $f(x)=\sqrt[4]{x}$.


??? check "Solução"
  
    $\Large \text{Temos,}$ 
	
	$$\Large f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ \sqrt[4]{x+\Delta x}- \sqrt[4]{x}}{\Delta x} $$ 


## Notação de derivada 

$$f'(x)=\frac{\mbox{df}}{\dx} = \frac{\dy}{\dx} = y'=\dot{y}$$ 


**Definição**: 	Dizemos que a unção $f$ é diferenciável se existe a derivada em todos os pontos pertencentes ao domínio de $f$.  

**Teorema**: Se $f$ é diferenciável, então $f$ é contínua. 

??? check "Solução"
  
    $\Large \text{Demonstração: Queremos provar que}$ 

    $$\Large\displaystyle\lim_{x\to a} f(x)=f(x_0)$$ 

    $\Large \text{se}$  $\Large f$ $\Large \text{é diferenciável.}$  

    $\Large \text{Temos,}$  

    $$\Large \displaystyle\lim_{x\to x_0} f(x)-f(x_0) = \displaystyle\lim_{x\to x_0} \frac{ f(x)-f(x_0)}{x-x_0}\cdot (x-x_0)$$ 

    $$\Large =\displaystyle\lim_{x\to x_0} \frac{ f(x)-f(x_0)}{x-x_0}\cdot \displaystyle\lim_{x\to x_0} (x-x_0)$$ 

    $$\Large =f'(x_0)\cdot 0 = 0$$ 

    $\Large \text{Veja ainda que}$ 

    $$\Large\displaystyle\lim_{x\to x_0} f(x)= \displaystyle\lim_{x\to x_0} f(x)-f(x_0)+f(x_0) $$ 

    $$\Large = \displaystyle\lim_{x\to x_0} f(x)-f(x_0) + \displaystyle\lim_{x\to x_0} f(x_0)$$ 

    $$\Large =0+f(x_0) = f(x_0)$$ 

    $\Large \text{Logo,}$ $\Large\displaystyle\lim_{x\to x_0} f(x)=f(x_0)$, $\Large \text{assim}$ $\Large f$ $\Large \text{é contínua.}$ 


**Comentário**: 

> A reciproca do teorema é falsa!


### Exemplo 4 

Considere $f(x)=|x-3|$. Verifique se $f$ é diferenciável e contínua. 

??? check "Solução"
  
    $\Large \text{Note que a função $f$ é contínua de fato,}$ 
	
	$$f(x)=|x-3|=\left\{ \begin{array}{ccc}
	x-3, & \mbox{se} & x\geqslant 3 \\ 
	-(x-3),& \mbox{se} & x<3 
	\end{array}\right.$$ 
	
    Calculando os limites laterais, temos 

    $$\displaystyle\lim_{x\to 3^{-}} -(x-3)=0 $$ 

    $$\displaystyle\lim_{x\to 3^{+}} (x+3)=0$$ 

    Como 
    
    $\displaystyle\lim_{x\to 3^{-}}f(x) = \displaystyle\lim_{x\to 3^{+}} f(x)$,
    
    então $\displaystyle\lim_{x\to 3}f(x)=0=f(3)$. 
     
    Logo a função $f$ é contínua.

    Aí, vem a dúvida, será que $f(x)=|x-3|$ é diferenciável?

    Verificando, temos 

    $$f_{+}'(x)= \displaystyle\lim_{x\to 3^{+}} \frac{ x-3-0}{x-3} = \displaystyle\lim_{x\to 3^{+}} 1 = 1 $$ 

    $$f_{-}'(x)=\displaystyle\lim_{x\to 3^{-}} \frac{-x+3}{x-3} = \displaystyle\lim_{x\to 3^{-}} - 1 = -1$$ 

    Como $f_{+}'(x)\neq f_{-}'(x)$.

    Logo, $f'(3)=\displaystyle\lim_{x\to 3} \frac{f(x)-f(3)}{x-3}$ não existe. 

    Portanto,  $f$ não é diferenciável. 


### Exemplo 5 

Seja $f(x)=\left\{\begin{array}{ccc} 
1+x^2, & \mbox{se} & x<-2\\ 
9-x^2, & \mbox{se} & x\geqslant -2 
\end{array}\right.$


[(a)] Mostre que $f$ é contínua em $x_0=-2$. 

[(b)] Determine $f_{+}'(-2)$ e $f_{-}'(-2)$

[(c)] $f$ é derivável em $x_0=-2$?


??? check "Solução"
  
    $\Large \text{(a) - 	Temos }$ 


	$$\Large f(-2)=9-(-2)^2=5 $$ 
	
	Calculando os limites laterais: 

	$$\displaystyle\lim_{x\to -2^{+}} f(x)=\displaystyle\lim_{x\to -2^{+}} (9-x^2)=9-4=5$$ 
	
	$$\displaystyle\lim_{x\to -2^{-}} f(x)=\displaystyle\lim_{x\to -2^{-}} (1+x^2)=1+4=5$$ 
	
	Como $\displaystyle\lim_{x\to -2^{-}}f(x) = \displaystyle\lim_{x\to -2^{+}} f(x)=5$, então 

	$$\displaystyle\lim_{x\to -2} f(x)=5=f(-2)$$ 

	Logo, $f$ é contínua em $x_0=-2$. 
	
	
    (b): Temos por definição 

	$$f_{+}'(x)=\displaystyle\lim_{x\to -2^{+}} \frac{ f(x)-f(-2)}{x+2}=\displaystyle\lim_{x\to -2^{+}} \frac{9-x^2-5}{x+2}$$ 
	
	$$= \displaystyle\lim_{x\to -2^{+}} \frac{-x^2+4}{x+2}= \displaystyle\lim_{x\to -2^{+}} \frac{(2-x)(2+x)}{x+2} = 4 $$ 
	
	$$f_{-}'(x)=\displaystyle\lim_{x\to -2^{-}} \frac{ f(x)-f(-2)}{x+2}=\displaystyle\lim_{x\to -2^{+}} \frac{1+x^2-5}{x+2}$$ 
	
	$$= \displaystyle\lim_{x\to -2^{-}} \frac{-x^2+4}{x+2}= \displaystyle\lim_{x\to -2^{+}} \frac{(x-2)(x+2)}{x+2} = -4 $$ 
	
	\textbf{(c)}: Como as derivadas laterais são distintas, então não existe o limite. 
	
	Logo, $\nexists ~f'(-2)$. 