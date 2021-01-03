
# **Inclinação da reta**

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







<center>
  <p><small>Representação gráfica. </small></p><br>
    <img src="/assets/images/derivada_reta.png"/>
  </small>
</center>


A inclinação da reta secante é dada por: 

$$m_s=\dfrac{f(x)-f(x_0)}{x-x_0}$$ 

Sabendo que $y=f(x)$, temos 

$$y-f(x_0)=m_s (x-x_0)$$ 

que é a equação da reta no plano. 

onde $m$ é o coeficiente angular ou inclinação da reta. O nosso objetivo é encontrar a equação da reta tangente. 

Se fizermos $x\to x_0$, veja o que acontece com a curva e a reta $s$:

$$\text{Ainda falta inserir imagem aqui!}$$ 


Assim, quando mais fizermos $x$ tender para $x_0$, a reta secante se transforma numa reta tangente no ponto $(x_0,f(x_0))$. 

Logo, 

$$m_t=\displaystyle\lim_{x\to x_0} \frac{ f(x)-f(x_0)}{x-x_0}$$


## **Definição**
A reta tangente a uma curva $y=f(x)$ em um ponto $P(x_0,f(x_))$ é a reta que passa no ponto $P$ e tem inclinação 
	
$$m_t=\displaystyle\lim_{x\to x_0} \frac{f(x)-f(x_0)}{x-x_0}$$ 
	
Além disso, a equação da reta tangente no ponto $P$ é dada por 
	
$$y-f(x_0)=m_t(x-x_0)$$ 
	
### Exemplo 1 

Determine a equação da reta tangente à curva $y=x^2$ no ponto $x_0=5$. 

??? check "Solução"
  
    Temos 

    $$\Large m_t=\displaystyle\lim_{x\to x_0} \frac{ f(x)-f(x_0)}{x-x_0} $$ 

    $\Large\text{Aplicando as informações dada no exemplo, temos}$

    $$\Large m_t=\displaystyle\lim_{x\to 5} \frac{ x^2-25}{x-5} = \displaystyle\lim_{x\to 5} \frac{ (x-5)(x+5)}{x-5} $$ 

    $$\Large =\displaystyle\lim_{x\to 5} x+5=10$$ 

    $\Large\text{Assim, a equação da reta tangente:}$ 

    $$\Large y-25=10(x-5)$$ 

    $$\Large y=10x-25$$ 

    $\Large \text{A equação da reta tangente.}$ 

    $\Large \text{Veja no gráfico abaixo a função}$ $\Large y=x^2$ $\Large \text{e a sua reta tangente:}$ 

    <center>
    <img src="/assets/images/exemplo_1.png"/>
    </small>
    </center>

### Exemplo 2 

Determine a equação da reta tangente à curva $y=x^3$ no ponto $x_0=1$. 



??? check "Solução"
  
    Temos 

    $$\Large m_t=\displaystyle\lim_{x\to 1} \frac{x^3-1}{x-1}$$ 
    
    $$\Large = \displaystyle\lim_{x\to 1}\frac{(x-1)(x^2+x+1)}{x-1}$$ 
    
    $$\Large = \displaystyle\lim_{x\to 1} x^2+x+1 = 3$$

    $\Large \text{Assim, a equação da reta tangente é dada por:}$ 
	
    $$\Large y-1=3(x-1) \Rightarrow y=3x-2$$ 
	
    $\Large \text{Graficamente, temos}$ 

    <center>
    <img src="/assets/images/exemplo_2.png"/>
    </small>
    </center> 


### Exemplo 3 

Encontrar a tangente do ângulo formado pela tangente à curva $y=x^2$ nos pontos: $M_1\left(\frac{1}{2},\frac{1}{4}\right)$ e $M_2=\left(-1,1\right)$. 

??? check "Solução"
  
    $\Large \text{Temos}$ 

    $\Large \text{Calculamos a derivada,}$ 
	
    $$\Large f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{f(x_0+\Delta x)-f(x_0)}{\Delta x}$$ 
	
    $$\Large f'\left(\frac{1}{2}\right)=\displaystyle\lim_{\Delta x\to 0} \frac{ f\left(\frac{1}{2}+\Delta x\right)-f\left(\frac{1}{2}\right)}{\Delta x} $$ 	

    $$\Large f'\left(\frac{1}{2}\right)=\displaystyle\lim_{\Delta x\to } \frac{ \left(\frac{1}{2}+\Delta x\right)^{2} - \frac{1}{4}}{\Delta x}$$ 

    $$\Large f'\left(\frac{1}{2}\right)=\displaystyle\lim_{\Delta x\to 0} \frac{ \frac{1}{4}+\Delta + 2\frac{1}{2}\Delta x + (\Delta x)^2 - \frac{1}{4}}{\Delta x}$$ 
	
    $\Large \text{Simplificando,}$ 
	
    $$\Large f'\left(\frac{1}{2}\right)= \displaystyle\lim_{\Delta x\to 0} \frac{ \Delta x(1+\Delta x)}{\Delta x}$$ 
	
    $\Large \text{Simplificando,}$ 

    $$\Large f'\left(\frac{1}{2}\right)=\displaystyle\lim_{\Delta x\to 0} 1+\Delta x=1 $$ 
	
    $\Large \text{Logo,}$  
    
    $$\Large f'\left(\frac{1}{2}\right)=1=\tg(\varphi_1)$$
	
    $\Large \text{Assim, o cálculo do ângulo}$ $\Large\varphi_1$, $\Large \text{fica}$ 

    $$\varphi_1=\mbox{arctg}(1)= \frac{\pi}{4}$$ 
	
    $\Large \text{Para o segundo ponto,}$ $\Large M_2$, $\Large \text{temos}$ 

    $$\Large f'(-1)=\displaystyle\lim_{\Delta x\to 0} \frac{f(-1\Delta x)-f(-1)}{\Delta x}$$ 
	
    $$\Large f'(-1)=\displaystyle\lim_{\Delta x\to 0} \frac{ (-1+\Delta x)^2-1}{\Delta x}$$ 
	
    $\Large \text{Desenvolvendo o quadrado da diferença,}$ 
	
    $$\Large f'(-1)=\displaystyle\lim_{\Delta x\to 0} \frac{ 1-2\Delta x+ (\Delta x)^2-1}{\Delta x}$$

    $\Large \text{Simplificando,}$ 
	
    $$\Large f'(-1)=\displaystyle\lim_{\Delta x\to 0} \frac{ \Delta x(-2+\Delta x)}{\Delta x} $$ 
	
    $$\Large f'(-1)=\displaystyle\lim_{\Delta x\to 0} \displaystyle\lim (-2 + \Delta x) = -2 $$ 
	
    $$\Large f'(-1)=-2=\tg(\varphi_2)$$ 

    $$\Large \varphi_2=\mbox{arctg}(-2)$$ 

    $$\Large \varphi_2=-63,43^{\circ}$$ 

    $\Large \text{Logo,}$ $\Large\varphi'=180^{\circ}-63,43^{\circ} = 116,57^{\circ}$. 
	
    $\Large \text{Graficamente, temos}$ 


### Exemplo 4 

Obter a equação da reta tangente ao gráfico $$y=x^2-3x$$ no ponto de abscissa $x_0=4$. 


??? check "Solução"
  
    $\Large \text{Temos que a equação da reta tangente é dada por:}$
	
    $$\Large y-f(x_0)=f'(x_0)(x-x_0)$$ 
	
    $$\Large y-f(4)=f'(4)(x-4)$$ 
	
    $\Large \text{Precisamos determinar}$ $\Large f(4)$ $\Large \text{e}$ $\Large f'(4)$. 
	
    $\Large \text{Calculando a derivada, temos}$
	
    $$\Large f'(x_0)=\displaystyle\lim_{\Delta x\to 0} \frac{f(x_0-\Delta x)-f(x_0)}{\Delta x} $$ 
	
    $$\Large f'(4)=\displaystyle\lim_{\Delta x\to 0} \frac{f(4+\Delta x)-f(4)}{\Delta x}$$ 
	
    $$\Large f'(4)=\displaystyle\lim_{\Delta x\to 0} \frac{ (4-\Delta x)^2-3(4+\Delta x)-4}{\Delta x} $$ 
	
    $$\Large f'(4)=\displaystyle\lim_{\Delta x\to 0} \frac{ 16+8\Delta x+(\Delta x)^2-12-3\Delta x - 4}{\Delta x}$$ 
	
    $\Large \text{Simplificando,}$
	
    $$\Large f'(4)=\displaystyle\lim_{\Delta x\to 0} \frac{ \Delta x(5+\Delta x)}{\Delta x}$$ 
	
    $$\Large f'(4)=\displaystyle\lim_{\Delta x\to 0}  5 + \Delta x=5$$ 

    $\Large \text{Portanto,}$ 
	
    $$\Large y-4=5(x-4) \Rightarrow y=5x-16$$ 

    $\Large \text{Equação reduzida. }$ 
	
    $$\Large 5x-y-16=0$$ 

    $\Large \text{Equação geral.}$ 


## Equação da Reta Normal

Note que duas retas $$s$$ e $$t$$ são ortogonais se $m_s\cdot m_t$ é igual a $-1$. 

Logo, a equação da reta normal a curva $$y$$ no ponto $x_0$ é dada por 

$$y-f(x_0)=-\frac{1}{m_t}(x-x_0)$$ 

onde $m_t=\displaystyle\lim_{x\to x_0} \frac{ f(x)-f(x_0)}{x-x_0}$ 


### Exemplo 5 

Determine a equação da reta normal à curva $y=x^2+3$ no ponto $x_0=2$.


??? check "Solução"
  
    $\Large \text{Temos}$  
	
    $$\Large m_t=\displaystyle\lim_{x\to 2} \frac{x^2+3-7}{x-2}$$ 
    
    $$\Large = \displaystyle\lim_{x\to 2} \frac{(x-2)(x+2)}{x-2} = \displaystyle\lim_{x\to 2} x+2=4$$ 
	
    $\Large\text{Assim,}$ 
	
    $$\Large y-7=-\frac{1}{4}(x-2) \Rightarrow y=-\frac{x}{4}+\frac{1}{2}+7$$ 

    $$\Large y=-\frac{x}{4}+\frac{15}{2}$$ 


## Interpretação Mecânica da Derivada


**Velocidade Média**

$$V_m=\frac{\Delta S}{\Delta t} = \frac{ S(t_0+\Delta t)-S(t_0)}{\Delta t}$$ 

**Velocidade Instantânea**

$$V(t_0)=\displaystyle\lim_{\Delta t\to 0} V_m$$ 

$$= \displaystyle\lim_{\Delta t\to 0} \frac{ S(t_0+\Delta t)-S(t_0)}{\Delta t} = S(t_0)$$ 

**Aceleração Média**

$$V=V(t)$$ 

$$a_m=\frac{\Delta V}{\Delta t} = \frac{V(t_0+\Delta t)-V(t_0)}{\Delta t} $$ 

**Aceleração Instantânea**

$$a(t_0)=\displaystyle\lim_{\Delta t\to 0} a_m=\displaystyle\lim_{\Delta t\to 0} \frac{ V(t_0+\Delta t)-V(t_0)}{\Delta t}=V(t_0)$$ 


### Exemplo 6

Um móvel desloca-se sempre uma reta obedecendo a equação $S=\frac{1}{t}$, sendo $S$ espaços medidos $ft$. Sua velocidade no instante $t=3s$. 

??? check "Solução"
  
    $\Large \text{Temos}$ 
	
    $$\Large V(t_0)=\displaystyle\lim_{\Delta t\to 0} \frac{S(t_0+\Delta t)-S(t_0)}{\Delta t}$$ 
	
    $$\Large V(3)=\displaystyle\lim_{\Delta t\to 0} \frac{ S(3+\Delta t)-S(3)}{\Delta t}$$ 
	
    $$\Large V(3)=\displaystyle\lim_{\Delta t\to 0}  \frac{\frac{1}{3+\Delta t}-\frac{1}{3}}{\Delta t} $$ 
	
    $$\Large V(3)=\displaystyle\lim_{\Delta t\to 0} \frac{\frac{3-3-\Delta t}{3(3+\Delta t)}}{\Delta t} $$ 
	
	
    $$\Large V(3)=\displaystyle\lim_{\Delta t\to 0} \frac{ -\Delta t}{3\Delta t(3+\Delta t)}$$ 
	
    $$\Large V(3)=-\frac{1}{3}\displaystyle\lim_{\Delta t\to 0}\frac{1}{3+\Delta t}$$ 
	
    $$\Large V(3)=\displaystyle\lim_{\Delta t\to 0} -\frac{1}{3}\cdot \frac{1}{3}$$ 
    
    $$=-\frac{1}{9} ft/s$$ 


### Exemplo 7 

Um ponto material desloca-se sobre uma reta obedecendo a equação $V=\sqrt[3]{t}$, sendo $V$ velocidade em $ft/s$ e $t$ tempo em segundos. Obter sua aceleração no instante $t=2s$.  


??? check "Solução"
  
    $\Large \text{Temos}$ 
	
    $$a(t_0)=\displaystyle\lim_{\Delta t\to 0} \frac{ V(t_0+\Delta t)-V(t_0)}{\Delta t} $$ 
	
    $$a(2)=\displaystyle\lim_{\Delta t\to 0} \frac{ V(2+\Delta t)-V(2)}{\Delta t}$$ 
	
    $$a(2)=\displaystyle\lim_{\Delta t\to 0} \frac{ \sqrt[3]{2+\Delta t}-\sqrt[3]{2}}{\Delta t} $$ 
	
    $$a(2)=\displaystyle\lim_{\Delta t\to 0} \frac{ (\sqrt[3]{2+\Delta t})\left[(\sqrt[3]{2+\Delta t})^2+\sqrt[3]{2+\Delta t}\sqrt[3]{2}+(\sqrt[3]{2})^2\right]}{\Delta t\left[(\sqrt[3]{2+\Delta t})^2+\sqrt[3]{2+\Delta t}\sqrt[3]{2}+(\sqrt[3]{2})^2\right]}$$ 
		
    $$a(2)=\displaystyle\lim_{\Delta t\to 0} \frac{2+\Delta t-2}{\Delta t\left[(\sqrt[3]{2+\Delta t})^2+\sqrt[3]{2+\Delta t}\sqrt[3]{2}+(\sqrt[3]{2})^2\right]} $$ 
		
    Simplificando, 
		
    $$a(2)=\displaystyle\lim_{\Delta t\to 0} \frac{\Delta t}{\Delta t\left[(\sqrt[3]{2+\Delta t})^2+\sqrt[3]{2+\Delta t}\sqrt[3]{2}+(\sqrt[3]{2})^2\right]} $$
    
    $$a(2)=\displaystyle\lim_{\Delta t\to 0} \frac{1}{\Delta t\left[(\sqrt[3]{2+\Delta t})^2+\sqrt[3]{2+\Delta t}\sqrt[3]{2}+(\sqrt[3]{2})^2\right]} $$
    
    $$a(2)=\frac{1}{\Delta t\left[(\sqrt[3]{2})^2+\sqrt[3]{2}\sqrt[3]{2}+(\sqrt[3]{2})^2\right]} $$
    
    $$a(2)= \frac{1}{3\sqrt[3]{4}} m/s^2$$ 