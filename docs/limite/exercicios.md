
# **Exercícios**

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

## Exercício - limite indeterminado

Calcule $\dlim_{x\to -1} \dfrac{\sqrt[3]{x+2}-1}{x+1}$. 

??? check "Solução passo a passo"
    $\Large\text{Para resolver este exercício vamos empregar um artifício de mudança de variável}.$

    $\Large\text{Seja}$ $\Large u=\sqrt[3]{x+2} \Leftrightarrow u^3=x+2 \Leftrightarrow u^3-2=x$. 
	
    $\Large\text{Quando}$ $\Large x\to -1 \Rightarrow u \to 1$, $\Large\text{pois}$ $\Large u=\sqrt[3]{x+2}=\sqrt[3]{-1+2}=1$. 
	
    $\Large\text{Reescrevendo o limite, temos}$
	
    $$\Large\dlim_{u\to 1} \dfrac{u-1}{u^3-1}$$ 
    
    $$\Large = \dlim_{u\to 1} \dfrac{(u-1)}{(u-1)(u^2+u+1)}$$ 

    $$\Large =\dlim_{u\to 1} \dfrac{1}{u^2+u+1} = \dfrac{1}{3}$$ 
	
    $\Large\text{Portanto,}$ $\Large \dlim_{x\to -1} \dfrac{\sqrt[3]{x+2}-1}{x+1}=\dfrac{1}{3}.$ 


## Exercício - limite indeterminado 2 

Calcule $\dlim_{x\to 1} \dfrac{\sqrt{x^2+3}-2}{x^2-1}$.

??? check "Solução passo a passo"
    
    $\Large\text{Seja}$ $\Large \xi= \sqrt{x^2+3} \Leftrightarrow \xi^2=x^2+3 \Leftrightarrow \xi^2-3=x^2$.
    
    $\Large\text{Note que quando}$ $\Large x\to 1 \Rightarrow \xi \to 2$, $\Large\text{pois}$ $\Large \xi = \sqrt{1^2+3}=\sqrt{4}=2$. 
	
	$\Large\text{Reescrevendo o limite,}$ 
	
	$$\Large \dlim_{\xi \to 2} \dfrac{\xi -2}{\xi^2-3-1}$$
    
    $$\Large =\dlim_{\xi \to 2} \dfrac{ \xi-2}{(\xi -2)(\xi+2)}$$ 

    $$\Large = \lim_{\xi \to 2 } \dfrac{1}{\xi +2}=\dfrac{1}{4}$$ 


## Exercício - limite indeterminado 3 

Determine $\dlim_{x\to 1} \dfrac{ (3-x^3)^4-16}{x^3-1}$ 

??? check "Solução passo a passo"
    
    $\Large\text{Seja}$  $\Large u=(3-x^3) \Leftrightarrow u-3=-x^3 \Leftrightarrow -u+3=x^3$. 

    $\Large\text{Quando}$ $\Large x\to 1 \Rightarrow u\to 2$, $\Large\text{pois}$ $\Large u=(3-1^3)=2$. 
    
    $\Large\text{Reescrevendo o limite,}$

    $$\Large\dlim_{u\to 2} \dfrac{u^4-16}{-u+3-1}$$
    
    $$\Large =\dlim_{u\to 2} \dfrac{(u^2)^2-(2^2)^2}{-u+2}$$ 

    $$\Large= \dlim_{u\to 2} \dfrac{(u-2)(u+2)(u^2+2^2)}{-(u-2)}$$ 

    $$\Large = \dlim_{x\to 2} -(u+2)(u^2+4)=-32$$ 

## Exercício - Continuidade 

Verifique a continuidade para 

$$f(x)=\left\{ \begin{array}{lcl}
\dfrac{(x-2)(x-3)}{(x-3)} & \mbox{se} & x \neq 3 \\
2 & \mbox{se} & x=3
\end{array}\right.$$ 

??? check "Solução passo a passo"
    
    Em breve. 


## Exercício - Continuidade 2 

Verifique a continuidade da função 

$$f(x)=\left\{ \begin{array}{lcl}
\dfrac{x^2+3+2}{x+1} & \mbox{se} & x <-1 \\
1 & \mbox{se} & x=-1\\ 
3x & \mbox{se} & x>-1
\end{array}\right.$$ 


??? check "Solução" 

    $\Large\text{Primeiro vamos verificar se o limite existe,}$ $\Large\dlim_{x\to x_0} f(x)$, $\Large\text{logo precisamos calcular os limites laterias,}$ 
	
    $$\Large\dlim_{x\to -1^{-}} f(x) = \dlim_{x\to -1^{-}} \dfrac{x^2+3+2}{x+1}$$ 
    
    $$\Large = \dfrac{0}{0} ~\mbox{(Indeterminação)}$$ 
	
    $\Large\text{Precisamos fatorar o polinômio no numerador para talvez retirar a indeterminação,}$ 
	
    $$\Large\dlim_{x\to -1^{-}} \dfrac{x^2+3+2}{x+1}$$
    
    $$\Large =\dlim_{x\to -1^{-}} \dfrac{(x+1)(x+2)}{x+1}$$ 
	
    $$\Large = \dlim_{x\to -1^{-}} x+2 = 1$$ 

    $\Large\text{Pela direita,}$ 
	
    $$\Large\dlim_{x\to -1^{+}} 3x=-3$$ 
	
    $\Large\text{Como os limites laterais são diferentes, ou seja}$ $\Large\dlim_{x\to -1^{-}} f(x) \neq \dlim_{x\to -1^{+}} f(x)$. $\Large\text{Assim,}$  $\Large \nexists \dlim_{x\to -1} f(x)$. $\Large\text{Portanto,}$ 
	
    $\Large f$ $\Large\text{é descontínua no ponto}$ $\Large x_0=-1$. 


## Exercício - Continuidade 3 

Verificar se a função $f(x)$ é contínua no ponto $x_0=2$ 

$$ f(x)= \left\{ \begin{array}{lcl}
7x-6 & \mbox{se} & x <2 \\
2x^2 & \mbox{se} & x \geqslant 2
\end{array}\right. $$  


??? check "Solução"
    $\Large\text{Primeiro vamos verificar se o limite existe, para isso precisamos calcular os limites laterais, visto que a função é dada por sentenças,}$  
    
    $$\Large \dlim_{x\to 2^{-}} f(x)=\dlim_{x\to 2^{-}} 7x-6 = 8$$
    
    $$\Large\dlim_{x\to 2^{+}} f(x) = \dlim_{x\to 2^{+}} 2x^2=8$$
    
    $\Large\text{Como os limites laterais existem e são iguais, ou seja}$ $\Large\dlim_{x\to 2^{-}} f(x)= \dlim_{x\to 2^{+}} f(x) = 8$, $\Large\text{temos que}$ $\Large\dlim_{x\to 2} f(x) =8$
    
    $\Large\text{Veja ainda que}$ $\dlim_{x\to 2} f(x) = f(2) = 2\cdot 2^2 = 8$. $\Large\text{Portanto,}$ $\Large f$ $\Large\text{é contínua no ponto}$ $\Large x_0=2$.


## Exercício - Continuidade 4

Seja $f:\R - \{1 \} \rightarrow \R$ 

$$ f(x)=\dfrac{|x-1|}{x-1}$$ 

Calcular $\dlim_{x\to 1^{-}}f(x)$, $\dlim_{x\to 1^{+}} f(x)$ e $\dlim_{x\to 1} f(x)$.

??? check "Solução"
    $\Large\text{Como a função dada envolve uma outra função modular, temos que reescrever a função}$ $\Large f$, $\Large\text{usando a definição de módulo,}$  

    $\Large\text{Recorde-se que:}$
    
    $\Large |x|=\left\{ \begin{array}{lcl}
    x & \mbox{se} & x\geqslant 0 \\
    -x & \mbox{se} & x < 0
    \end{array}\right.$

    $\Large\text{Assim,}$  

    $$\large f(x) = \dfrac{|x-1|}{x-1}=\left\{ \begin{array}{lcl}
    \dfrac{x-1}{x-1} & \mbox{se} & x>1 \\
    -\dfrac{x-1}{x-1} & \mbox{se} & x < 1
    \end{array}\right.$$ 

    $\Large\text{Calculando os limites laterais,}$  

    $\Large\dlim_{x\to 1^{-}} f(x) = \dlim_{x\to 1^{-}} -\dfrac{x-1}{x-1}$$ 
    
    $$\Large = \dlim_{x\to 1^{-}} -1 = -1$$


    $\Large\dlim_{x\to 1^{+}} f(x) = \dlim_{x\to 1^{+}} \dfrac{x-1}{x-1}$$ 
    
    $$\Large = \dlim_{x\to 1^{+}} 1 = 1$ 

    $\Large\text{Como os limites laterais são diferentes,}$ $\Large \nexists \dlim_{x\to 1} f(x)$, $\Large\text{ou seja não existe o limite para}$ $\Large x$ $\Large\text{tendendo para}$ $\Large 1$. 

    $\Large\text{Por fim, podemos reescrever}$ $\large f$ $\Large\text{da seguinte forma:}$  

    $$\Large f(x) = \left\{ \begin{array}{lcl}
    1 & \mbox{se} & x>1 \\
    -1 & \mbox{se} & x < 1
    \end{array}\right.$$ 

    $\Large\text{Graficamente, temos}$  

    <center>
    <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/exercicio_cont.png" style="width: 50%; height: auto;"/>
    </small>
    </center>

    