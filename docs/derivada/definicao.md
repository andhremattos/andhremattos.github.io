
# **Definição**

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



**Definição**: Dizemos que $f'(x_0)$ é a derivada da função $y=f(x)$ se o seguinte limite existe: 

$$ f'(x_0) =  \displaystyle\lim_{\Delta x\to 0} \displaystyle\frac{f(x_0 +\Delta x) - f(x_0)}{\Delta x} $$ 

Fazendo uma modificação.


### Exemplo 1 

Determine a derivada da função $f(x)=5x^2+8$ no ponto $x_0=2$.

??? check "Solução"
  
    $\Large \text{Calculamos a derivada no ponto, logo}$ 
	
    $$\Large f'(x_0)=f'(2)= \displaystyle\lim_{\Delta x\to 0} \frac{ f(2+\Delta )-f(2)}{\Delta x}$$ 
	
    $$\Large f'(2)= 28$$ 
	
    $\Large \text{Logo, a derivada de}$ $\Large y=5x^2+8x+1$ $\Large \text{no ponto}$ $\Large x_0=2$ $\Large \text{é}$ $\Large f'(2)=28$.



**Comentário**: 

> A derivada de uma função no ponto $x=x_0$ é a inclinação da reta tangente no ponto $x=x_0$. 



### Exemplo 2 

Encontre uma equação da reta tangente á parábola $y=x^2-8x+9$ no ponto $x_0=3$. 

??? check "Solução"
  
    $\Large \text{Temos}$ 

    $$\Large f'(3)=\displaystyle\lim_{\Delta x\to } \frac{ f(3+\Delta x) -f(3)}{\Delta x} $$ 

    $$\Large f'(3)=-2$$ 

    $\Large \text{Substituir,} $ 


## Taxa de VAriação 


Suponha que $y$ seja uma quantidade que depende de outra quantidade $x$, assim $y=f9x)$. 

Se $x$ variar de $x_1$ para $x_2$, então a variação de $x$ é $\Delta x=x_2-x_1$. 

A variação correspondente de $y$ é $\Delta y= f(x_2)-f(x_1)$. 

Graficamente, temos 

<center>
  <p><small>Representação gráfica. </small></p><br>
    <img src="/assets/images/derivada_reta.png"/>
  </small>
</center>


Uma taxa de variação média é dada por $t_m=\frac{\Delta y}{\Delta x}$


**Definição**: 	Definimos uma taxa instantânea de variação pelo 	

$$\displaystyle\lim_{\Delta x\to 0} \frac{\Delta y}{\Delta x}$$ 
  
$$= \displaystyle\lim_{x_1\to x_2} \frac{f(x_2)-f(x_1)}{x_2-x_1} = f'(x_2)$$ 


### Exemplo 3 

A posição de uma partícula é dada pela equação do movimento $S(t)=\frac{1}{1+t}$, onde $t$ é medido em segundos e $S(t)$ em metros. Determine a velocidade no instante $2$. 


??? check "Solução"
  
    $\Large \text{Temos, 
    
    $$S'(2)=\displaystyle\lim_{\Delta x\to 0 } \frac{ S(2+\Delta x)-S(2)}{\Delta x} $$ 
    
    $$ = \displaystyle\lim_{\Delta x\to 0} \frac{1}{\Delta x} \left(\frac{1}{3+\Delta x}-\frac{1}{3}\right)$$ 
    
    $$ S'(2)= -\frac{1}{9} m $$ 










### Propriedades de derivada 

!!! tip "Derivada"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/fiRCZdvuQAM"></iframe>
    </p>

### Regra do produto 

### Regra do quociente 

!!! tip "Derivada: regra do quociente"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/y5pkvgXgW4k"></iframe>
    </p>

### Derivada da função raiz 

!!! tip "Derivada da função raiz"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/L0RBmcKK64E"></iframe>
    </p>

### Regra da cadeia 

!!! tip "Aula Derivada:Regra da cadeia"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/3luG7gogHeM"></iframe>
    </p>

### Derivada da função exponencial 

!!! tip "Derivada da função exponencial"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/OsJ5CLayD28"></iframe>
    </p>

### Derivada da função logarítmica 

!!! tip "Derivada logaritmo"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/gHivHqbutrk"></iframe>
    </p>

### Derivada da função composta 


!!! tip "Derivada da função composta 2"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/qSXQrypR6cA"></iframe>
    </p>

!!! tip "Derivada da função composta 3"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/ZsKZW2o7u_U"></iframe>
    </p>


!!! tip "Derivada da função composta 5"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/GcHo1Xf-lu0"></iframe>
    </p>

### Derivada implícita 

!!! tip "Derivada da função implícita"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/-xBWwvWbrKA"></iframe>
    </p>

!!! tip "Derivada da função implícita 2"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/QyzVRFO4mGM"></iframe>
    </p>

### Derivação logarítmica 

!!! tip "Derivação logarítmica"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/DTHr9jP97ek"></iframe>
    </p>



### Derivada da função trigonométrica inversa 

!!! tip "Derivada função trigonométrica inversa"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/kQ5J92rlspI"></iframe>
    </p>

### Aplicação da derivada 

!!! tip "Aplicação da derivada: pontos críticos"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/hITyA0Qb720"></iframe>
    </p>

