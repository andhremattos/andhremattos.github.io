
# **Fundamentais**

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

## Limite fundamental trigonométrico

Seja $f(x)=\dfrac{\sen(x)}{x}$, então 

$$\dlim_{x\to 0} \dfrac{\sen(x)}{x}=1$$ 

### Exemplo 1 

Determine o $\dlim_{x\to 0} \dfrac{\sen(7x)}{x}$. 


??? check "Solução"
    $\Large\text{Temos,}$  
    
    $$\Large\dlim_{x\to 0} \dfrac{ 7 \sen(7x)}{7x}$$
    $$\Large = 7\cdot \dlim_{x\to 0} \dfrac{ \sen(7x)}{7x} = 7\cdot 1 = 7$$ 
    
    $\Large\text{Ou fazendo uma mudança de variável}$ $\Large u=7x \Leftrightarrow \dfrac{u}{7}=u$. 
    
    $\Large\text{Quando}$ $\Large x\to 0 \Rightarrow u\to 0$, $\Large\text{pois}$ $\Large u=7\cdot 0 = 0$. 
    
    $\Large\text{Logo,}$ 
	
    $$\Large\dlim_{u\to 0} \dfrac{\sen(u)}{\dfrac{u}{7}}$$ 

    $$\Large = 7 \cdot \dlim_{u\to 0} \dfrac{\sen(u)}{u}$$ 
    
    $$\Large = 7\cdot 1 = 7$$ 


### Exemplo 2 

Determine $\dlim_{x\to 0} \dfrac{1-\cos(x)}{x^2}$. 


??? check "Solução"
    $\Large\text{Vemos que,}$ 
    
    $$\Large \dlim_{x\to 0 } \dfrac{1-\cos(x)}{x^2}$$ 
    
    $$\Large = \dfrac{1-1}{0}=\dfrac{0}{0} \rightarrow \mbox{Indeterminação}$$ 
    
    $$\Large = \dlim_{x\to 0} \dfrac{ (1-\cos(x))(1+\cos(x))}{x^2(1+\cos(x))}$$ 
    
    $$\Large = \dlim_{x\to 0} \dfrac{ 1-\cos^2(x)}{x^2}\cdot \dlim_{x\to 0} \dfrac{1}{1+\cos(x)}$$ 

    $\Large\text{Sabemos que}$ $\Large \cos^2(x)+\sen^2(x)=1 \Leftrightarrow 1-\cos^2(x)=\sen^2(x)$, $\Large\text{logo,}$ 
    
    $$\Large =\dlim_{x\to 0}\left[ \dfrac{\sen(x)}{x}\right]^2\cdot \dfrac{1}{2}$$ 
    
    $$\Large = 1\cdot \dfrac{1}{2} = \dfrac{1}{2}$$ 


### Exercício 3 

Determine $\dlim_{x\to 0} \dfrac{ \tg(x)}{x}$. 

??? check "Solução"
    
    $\Large\text{Quando $x\to 0 $, temos}$ 
    
    $$\Large\dlim_{x\to 0 } \dfrac{\tg(x)}{x}$$ 
    
    $$\Large = \dfrac{0}{0} \rightarrow ~\mbox{Indeterminação}$$ 
    
    $\Large\text{Reescrevendo o limite,}$ 
    
    $$\Large\dlim_{x\to 0} \dfrac{ \dfrac{\sen(x)}{\cos(x)}}{x}$$ 

    $$\Large = \dlim_{x\to 0} \dfrac{ \sen(x)}{x} \cdot \dlim_{x\to 0} \dfrac{1}{\cos(x)}$$

    $$\Large = 1\cdot \dfrac{1}{1} = 1$$ 


### Exercício 4 

Determine $\dlim_{x\to 1} \dfrac{1-x^2}{\sen(\pi x)}$. 

??? check "Solução"
    
    $\Large\text{Fazendo}$ $\Large x\to 1$, $\Large\text{temos}$ 
    
    $$\Large\dlim_{x\to 1} \dfrac{1-x^2}{\sen(\pi x)}$$ 
    
    $$\Large =\dfrac{0}{0} \rightarrow \mbox{Indeterminação}$$ 
    
    $\Large\text{Precisamos retirar a indeterminação, logo façamos}$  
    
    $$\Large\dlim_{x\to 1} \dfrac{(1-x)(1+x)}{\sen(\pi x)}$$ 
    
    $\Large\text{Fazemos uma mudança de variável:}$ $\Large u=1-x \Rightarrow u-1=-x$ 

    $$\Large 1-u=x$$ 
    
    $\Large\text{Quando}$ $\Large x\to 1 \Rightarrow u\to 0$, $\Large\text{pois}$ $\Large u=1-1^2=1-1=0$. 

    $\Large\text{Reescrevendo o limite, temos}$  

    $$\Large =\dlim_{u\to 0} \dfrac{ u(1+1-u)}{\sen(\pi(1-u))}$$ 

    $$\Large =\dlim_{u\to 0} \dfrac{ u(2-u)}{\sen(\pi-u\pi))}$$ 

    $$\Large =\dlim_{u\to 0} \dfrac{u(2-u)}{\sen(\pi)\cos(\pi u)-\sen(\pi u)\cos(\pi)}$$ 

    $\Large\text{Sabendo que}$ $\Large\sen(\pi)=0$ e $\cos(\pi)=-1$, $\Large\text{temos}$ 

    $$\Large =\dlim_{u\to 0} \dfrac{u}{\sen(\pi u)} \dlim_{u\to 0} (2-u)$$ 

    $$\Large =2\dlim_{u\to 0} \left[\dfrac{\sen(\pi u)}{u}\right]^{-1}$$ 

    $\Large\text{Fazendo uma nova mudança de variável:}$ $\Large\varphi = \pi u  \Rightarrow \dfrac{\varphi}{\pi} = u$. 

    $\Large\text{Quando}$ $\Large u\to 0 \Rightarrow \varphi \to 0$, $\Large\text{pois}$ $\varphi = \pi\cdot 0=0$. 

    $\Large\text{Reescrevendo,}$  

    $$\Large =\dlim_{\varphi \to 0} \left[\dfrac{ \sen(\varphi)}{\dfrac{\varphi}{\pi}}\right]^{-1}$$ 

    $$\Large =\dlim_{\varphi \to 0} \left[\dfrac{ \pi \sen(\varphi)}{\varphi}\right]^{-1}$$

    $$\Large = \dfrac{1}{\pi} \left[ \dlim_{\varphi \to 0}\dfrac{ \sen(\varphi)}{\varphi}\right]^{-1}$$ 

    $$\Large = \dfrac{1}{\pi}\cdot 1^{-1}=\dfrac{1}{\pi}$$



### Exemplo 5 

Determine $\dlim_{x\to 0} \dfrac{ 5\mbox{arcsen}(3x)}{2x}$. 

??? check "Solução"
    
    $\Large\text{Fazendo}$ $\Large x\to 0$, $\Large\text{temos}$ 

    $$\Large\dlim_{x\to 0} \dfrac{ 5\mbox{arcsen}(3x)}{2x}=\dfrac{0}{0} \rightarrow \mbox{Indeterminação}$$ 

    $\Large\text{Precisamos retirar essa indeterminação.}$  
    
    $\Large\text{Façamos uma mudança de variável}$ 
    $\Large \xi = \mbox{arcsen}(3x) \Leftrightarrow \sen(\xi)=3x \Rightarrow \dfrac{\sen(\xi)}{3}=x$ 

    $\Large\text{Quando}$ $\Large x\to 0 \Rightarrow \xi \to 0$, $\Large\text{pois}$ $\Large \xi = \mbox{arcsen}(3\cdot 0) = 0$. 

    $\Large\text{Reescrevendo o limite, temos}$ 

    $$\Large =\dlim_{\xi\to 0} \dfrac{ 5 \xi}{2\dfrac{\sen(\xi)}{3}}$$ 

    $$\Large = \dfrac{15}{2}\dlim_{\xi \to 0} \dfrac{\xi}{\sen(\xi)} $$ 

    $$\large =\dfrac{15}{2}\dlim_{\xi \to 0} \left[\dfrac{\sen(\xi)}{\xi}\right]^{-1}$$ 

    $$\Large =\dfrac{15}{2}\left[\dlim_{\xi \to 0} \dfrac{\sen(\xi)}{\xi}\right]^{-1}$$ 

    $$\Large =\dfrac{15}{2}\cdot 1^{-1}= \dfrac{15}{2}$$


### Exemplo 6 

Determine $\dlim_{x\to 0} \dfrac{ \sen(5x)-\sen(2x)}{x}$. 

??? check "Solução"
    
    $\Large\text{Fazendo}$ $\Large x\to 0$, $\Large\text{temos}$ 
    
    $$\Large \dlim_{x\to 0}\dfrac{ \sen(5x)-\sen(2x)}{x}$$

    $$\Large = \dfrac{0}{0}\rightarrow \mbox{Indeterminação} $$ 
    
    $\Large\text{Separando as funções,}$  
	
    $$\Large\dlim_{x\to 0} \dfrac{ \sen(5x)}{x} -\dlim_{x\to 0}\dfrac{\sen(2x)}{x}$$ 

    $\Large\text{Façamos duas mudanças de variáveis:}$ 
	
    $$\Large u=5x \Leftrightarrow \dfrac{u}{5}=x $$ 

    $\Large\text{e$  $\Large \omega = 2x \Leftrightarrow \dfrac{\omega}{2}=x$ 
    
    $\Large\text{Quando}$  $\Large x\to 0 \Rightarrow u \to 0$. $\Large\text{Quando}$  $\Large x\to 0 \Rightarrow \omega \to 0$. 
    
    $\Large\text{Reescrevendo o limite,}$  
    
    $$\Large =\dlim_{u\to 0} \dfrac{ \sen(u)}{\dfrac{u}{5}}-\dlim_{\omega \to 0} \dfrac{ \sen(\omega)}{\dfrac{ \omega}{2}} $$ 
    
    $$\Large =5\dlim_{u\to 0} \dfrac{ \sen(u)}{u}-2\dlim_{\omega \to 0} \dfrac{ \sen(\omega)}{\omega}$$
    
    $$\Large = 5\cdot 1 - 2\cdot 1$$ 
    
    $$= 5-2=3$$ 


### Exemplo 7

Determine $\dlim_{x\to 0} \dfrac{1-\cos(kx)}{k^2x^2}$.

??? check "Solução"

    $\Large\text{Fazendo}$ $\Large x\to 0$, $\Large\text{temos}$ 
    
    $$\Large \dlim_{x\to 0}\dfrac{1-\cos(kx)}{k^2x^2}=\dfrac{0}{0} \rightarrow \mbox{Indeterminação} $$ 

    $\Large\text{Da trigonometria temos que}$ $\Large 1-\cos(u)=2\sen^{2}\left(\dfrac{u}{2}\right)$. $\Large\text{Logo,}$  
    
    $$\Large\dlim_{x\to 0} \dfrac{ 2\sen^2\left(\dfrac{kx}{2}\right)}{k^2x^2}$$ 
    
    $$\Large =2\dlim_{x\to 0} \left[\dfrac{ \sen\left(\dfrac{kx}{2}\right)}{kx}\right]^{2}$$ 
    
    $\Large\text{Façamos uma mudança de variável,}$ $\Large u=\dfrac{kx}{2} \Leftrightarrow \dfrac{2u}{k}=x$. 
    
    $\Large\text{Quando}$ $\Large x\to 0 \Rightarrow u\to 0$, $\Large\text{pois}$ $\Large u= \dfrac{0}{2}=0$. 
    
    $\Large\text{Reescrevendo o limite,}$  
    
    $$\Large =2\dlim_{u\to 0} \left[\dfrac{\sen(u)}{k\dfrac{2u}{k}}\right]^{2}$$ 
    
    $$\Large =\dlim_{u\to 0}\left[ \dfrac{\sen(u)}{u} \right]^{2}=1$$ 
	
## Limite Fundamental Exponencial 


Proposição:

$$\dlim_{x\to \pm \infty} \left(1+\dfrac{1}{x}\right)^x = e \cong 2,7182$$ 

$e:$ Constante de Euler. 

<center>
    <p><small> </small></p><br>
    <img src="../imagens/euler.png" style="width: 50%; height: auto;"/>
    </small>
</center>


$e$: base do logaritmo neperiano. 

Se $y=\ln{(e)}=1$. Graficamente temos


<center>
    <p><small> </small></p><br>
    <img src="../imagens/ln.png" style="width: 50%; height: auto;"/>
    </small>
</center>


$$y=\ln{(x)} \Leftrightarrow y=\log_{e}{(x)}$$ 


### Exemplo 1 

Mostre que $\dlim_{x\to 0} \left(1+x\right)^{\frac{1}{x}} = e$. 


??? check "Solução"

    $\Large\text{Quando}$ $\Large x\to 0$, $\Large\text{temos}$ 
    
    $$\Large \dlim_{x\to 0} \left( 1+x\right){\frac{1}{x}}$$ 
    
    $$\Large = \left(1+0\right)^{+\infty} = 1^{+\infty} \rightarrow \mbox{Indeterminação} $$ 
    
    $\Large\text{Fazendo uma mudança de variável:}$ $\Large u=\dfrac{1}{x} \Rightarrow x=\dfrac{1}{u}$. 
    
    $\Large\text{Quando}$ $\Large x\to 0^{+} \Rightarrow u \to +\infty$. 
    
    $\Large\text{Reescrevendo o limite,}$ 
    
    $$\Large\dlim_{x\to 0^{+}} \left(1+x\right)^{\frac{1}{x}}$$ 
    
    $$\Large = \dlim_{u\to +\infty} \left(1+\dfrac{1}{u}\right)^u=e$$ 
	

### Exemplo 2 

Determine $\dlim_{x\to +\infty} \left(1+\dfrac{1}{x}\right)^{5x}$.  


??? check "Solução"

    $\Large\text{Temos,}$ 

    $$\Large\dlim_{x\to +\infty} \left(1+\dfrac{1}{x}\right)^{5x}$$ 
    
    $$\Large = \dlim_{x\to +\infty}\left[  \left(1+\dfrac{1}{x}\right)^{x} \right]^{5}$$ 
    
    $$\Large = e^{5}$$ 


### Exemplo 3 

Determine $\dlim_{x\to +\infty} \left(1+\dfrac{1}{x}\right)^{2x+3}$.  

??? check "Solução"

    $\Large\text{Fazendo}$ $\Large x\to +\infty$, $\Large\text{temos}$  
    
    $$\Large \dlim_{x\to +\infty} \left(1+\dfrac{1}{x}\right)^{2x+3}=1^{+\infty}$$ 
    
    $\Large\text{Sabendo que para}$ $\Large a^{m+n}=a^{m}\cdot a^{n}$ e $(a^{m})^{n}$, $\Large\text{temos}$
    
    $$\Large =\dlim_{x\to +\infty} \left(1+\dfrac{1}{x}\right)^{2x}\cdot \dlim_{x\to +\infty} \left(1+\dfrac{1}{x}\right)^{3}$$ 
    
    $$\Large =\dlim_{x\to +\infty}\left[\left(1+\dfrac{1}{x}\right)^{x}\right]^{2}\cdot \left(1+0\right)^3$$ 
    
    $$\Large =\left[\dlim_{x\to +\infty}\left(1+\dfrac{1}{x}\right)^{x}\right]^{2}=e^{2}$$ 


### Exemplo 4 

Determine $\dlim_{x\to +\infty} \left(1+\dfrac{3}{x}\right)^{2x}$. 
	

??? check "Solução"

    $\Large\text{Fazendo}$ $\Large x\to +\infty$, $\Large\text{temos}$  
    
    $$\Large\dlim_{x\to +\infty} \left(1+\dfrac{3}{x}\right)^{2x}=1^{+\infty} \rightarrow \mbox{Indeterminação} $$ 
    
    $\Large\text{Façamos uma mudança de variável,}$ 
    
    $$\Large \dfrac{1}{u}=\dfrac{3}{x} \Leftrightarrow x=3u$$ 

    $\Large\text{Quando}$ $\large x\to +\infty \Rightarrow u\to +\infty$. 

    $\Large\text{Reescrevendo o limite, temos}$ 
    
    $$\Large =\dlim_{u\to +\infty} \left(1+\dfrac{1}{u}\right)^{2\cdot (3u)}$$ 

    $$\Large =\dlim_{u\to +\infty} \left(1+\dfrac{1}{u}\right)^{6u}$$

    $$\Large =\dlim_{u\to +\infty} \left[\left(1+\dfrac{1}{u}\right)^{u}\right]^{6}$$

    $$\Large =e^{6}$$ 


## Limite Fundamental Logaritmo

Seja $$ \dlim_{\xi \to 0 } \dfrac{ a^{\xi} - 1}{\xi} = \ln{(a)} $$ 
onde, $a>0 $ e $ a\neq 1$. 


??? check "Demonstração"

    $\Large\text{Fazemos a seguinte mudança de variável:}$  

    $$\Large u=a^{\xi}-1 \Leftrightarrow u+1=a^{\xi} \Leftrightarrow \ln{(u+1)}$$ 

    $$\Large = \ln{(a^{\xi})}$$ 

    $$\Large \Leftrightarrow \ln{(u+1)} = \xi \ln{(a)} \Rightarrow \xi$$ 

    $$\Large = \dfrac{\ln{(u+1)}}{\ln{(a)}}$$ 

    $\Large\text{Note que}$ $\Large x\to 0 \Rightarrow u \to 0$. 

    $\Large\text{Calculando o limite,}$ 

    $$\Large\dlim_{u\to 0} \dfrac{u}{\dfrac{ \ln{(u+1)}}{\ln{(a)}}}$$ 

    $$\Large = \dlim_{u\to 0} \dfrac{ \ln{(a)}}{u\ln{(u+1)}}$$ 

    $$\Large =\dlim_{u\to 0} \dfrac{\ln{(a)}}{\ln{(u+1)^{\frac{1}{u}}}}$$ 

    $$\Large = \dfrac{\ln{a}}{1} = \ln{(a)}$$ 

### Exemplo 1 

Determine o $\dlim_{x\to 1} \dfrac{ e^{x-1}-a^{x-1}}{x-1}$. 


??? check "Solução"

    Fazendo a mudança de variável: $u= $

## Exercícios resolvidos em vídeo

??? check "Aula: Limite fundamental trigonométrico - parte 1"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/3xzZwUJasS0"></iframe>
    </p>

??? check "Aula: Limite fundamental trigonométrico - parte 2"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/xmj8l6etszQ"></iframe>
    </p>

??? check "Limite fundamental trigonométrico"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/Sy1ZfH8Abws"></iframe>
    </p>


??? check "Limite fundamental trigonométrico 2"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/C9L1Eh-mbNI"></iframe>
    </p>

??? check "Limite fundamental trigonométrico 3"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/LalYqBpYTJU"></iframe>
    </p>

??? check "Limite fundamental trigonométrico 4"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/sbC0XAwoAyw"></iframe>
    </p>



