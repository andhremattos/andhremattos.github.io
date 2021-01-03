
# **Assíntotas**

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


## Assíntota Vertical 

Dizemos que a reta $x=a$ é uma assíntota vertical de $f(x)$, se 

(i) $\dlim_{x\to a}f(x)=\pm \infty$;

(ii) $\dlim_{x\to a^{-}} f(x)=\pm \infty$;

(iii) $\dlim_{x\to a^{+}} f(x)=\pm \infty$

### Exemplo 1 

Verifique se a reta $x=2$ é uma assíntota vertical do gráfico de $y=\dfrac{1}{(x-2)^2}$.
 
??? check "Solução"

    $\Large\text{Devemos analisar o seguinte limite:}$ 
	
    $$\Large\dlim_{x\to 2} f(x) = \dlim_{x\to 2} \dfrac{1}{(x-2)^2}$$ 
	
    $\Large\text{Note que}$ $\Large\dlim_{x\to 2} g(x) = \dlim_{x\to 2} 1 = 1 $. 

    $\Large\dlim_{x\to 2} f(x) = \dlim_{x\to 2} (x-2)^2>0$. 

    $\Large\text{Então como}$ $\Large g(x)>0$ e $\Large f(x)\to 0$ $\Large\text{por valores positivos, logo}$

    $$\Large\dlim_{x\to 2} \dfrac{g(x)}{f(x)} = +\infty$$

    $\Large\text{Portanto, a reta}$ $\Large x=2$ $\Large\text{é uma assíntota vertical.}$ 


## Assíntota Horizontal 

Dizemos que a reta $y=L$ é uma assíntota horizontal do gráfico da função $f$, se 

$$\dlim_{x\to +\infty} f(x)=L ~\mbox{ou}~\dlim_{x\to -\infty} f(x)=L$$

### Exemplo 2 

Determine as assíntotas verticais e horizontais da função $f(x)=\dfrac{2x+1}{x+1}$.


??? check "Solução"

    $\Large\text{Devemos calcular os limites,}$  
	
    $$\Large\dlim_{x\to +\infty} f(x)=\dlim_{x\to +\infty} \dfrac{ 2x+1}{x+1} = \dlim_{x\to +\infty} \dfrac{2x}{x}=2$$ 

    $\Large\text{Ainda temos que}$ $\Large\dlim_{x\to -\infty} f(x) = 2$. 

    $\Large\text{Portanto, a reta}$ $\Large y=2$ $\Large\text{é uma assíntota horizontal.}$  

    $\Large\text{Note que}$ $\Large\mbox{D}(f)=\{x\in \R ~| ~x+1 \neq 0 \} = \left\{x\in \R ~| ~ x\neq -1 \right\}$. 

    $\Large\text{Para determinar a assíntota vertical, calculamos o seguinte limite}$ 

    $$\Large\dlim_{x\to -1^{-}} \dfrac{2x+1}{x+1} = +\infty $$ 

    $\Large\text{pois o numerador tende para}$ $\Large -1<0$ $\Large\text{e denominador tende para}$ $\Large 0^{-}$, $\Large\text{portanto o limite tende para}$ $\Large +\infty$. 

    $\Large\text{Assim, a reta}$ $\Large x=-1$ $\Large\text{é uma assíntota vertical para todo}$ $\Large f(x)=\dfrac{2x+1}{x+1}$. 



