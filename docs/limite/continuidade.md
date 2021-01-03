
# **Continuidade**

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


## Definição 

Dizemos que uma **função** $f$ é **contínua** em um ponto $x_0$, quando:

+ $f(x_0)$ está definida; 

+ Existe $\displaystyle\lim_{x\to x_0} f(x)$ e; 

+ $\displaystyle\lim_{x\to x_0} f(x) = f(x_0)$. 

Para a definição de **função contínua à esquerda** ou à **direita**, usamos os conceitos de limites laterais. Quando a **função** $f$ não é contínua em um ponto $x_0$, temos que $f$ é **descontínua** neste ponto. 

### Exemplo 1

1. Considere a seguinte função 

$$f(x)= \left\{\begin{array}{cccc}
\displaystyle\frac{x-2}{(x+1)(x-2)}, & & x\neq 2  &\\
-4, & & x = 2&
\end{array}\right.$$

Na figura abaixo, temos um esboço do gráfico de $f$. 

<center>
  <p><small>Figura 1: Esboço gráfico. </small></p><br>
    <img src="../imagens/figura_1.png" style="width: 70%; height: auto;"/>
  </small>
</center>

Vamos verificar a continuidade desta função nos seguintes pontos: 

**a)** $x=2$. Neste ponto, temos que $f(-2) = -1$ e 

$$\displaystyle\lim_{x\to -2} \displaystyle\frac{x-2}{(x+1)(x-2)} = \displaystyle\frac{-4}{-1\cdot (-4)}$$ 

$$ = -1 = f(-2).$$ 

Com isso, concluímos que $f$ é contínua no ponto $x=-2$. 

**b)** $x=-1$. Neste ponto, 

$$f(-1) = \displaystyle\frac{x-2}{(x+1)(x-2)} = \displaystyle\frac{1}{(x+1)} = \displaystyle\frac{1}{(-1+1)} = \displaystyle\frac{1}{0}$$ 

logo, $f(-1)$ não está definido e, portanto, $f$ é descontínua neste ponto. Observemos que $f$ tem uma assíntota vertical em $x=-1$. 

**c)** $x=2$. Neste ponto, temos $f(2)=-4$ e 

$$ \displaystyle\lim_{x\to 2} \displaystyle\frac{x-2}{(x+1)(x-2)} = \displaystyle\lim_{x\to 2} \displaystyle\frac{x-2}{(x+1)}$$ 

$$ = \displaystyle\lim_{x\to 2} \displaystyle\frac{1}{x+1} = \displaystyle\frac{1}{3} \neq f(2).$$

Portanto, concluímos que $f$ é descontínua em $x=2$. 

É importante salientarmos que uma função $f$ é dita ser **contínua em um intervalo** $(a,b)$, quando $f$ é contínua em todos os pontos $x_0 \in (a,b)$. Para intervalos, $[a,b), ~(a,b]$ ou $[a,b]$, empregamos a noção de continuidade lateral nos pontos de extremos fechados dos intervalos. Quando a função é contínua em $(-\infty, +\infty)$, dizemos que ela é **contínua em toda parte.** 

### Exemplo 2 

Verifique se a função $f(x)=\left\{\begin{array}{ccc} 
x-2 & \mbox{se} & x\leqslant 3 \\ 
2 & \mbox{se} & x>3 
\end{array} 
\right.$ 


??? check "Limite - continuidade"
    Verificando os limites laterais: 
	
    $$ \dlim_{x\to 3^{-}} f(x)=\dlim_{x\to 3^{-}} (x-2)=1 $$ 
	
    $$\dlim_{x\to 3^{+}} f(x)=\dlim_{x\to 3^{+}} 2 = 2$$ 
	
    Logo, os limites laterais existem, porém são diferentes, assim $\dlim_{x\to 3} f(x)$ não existe, portanto a função $f$ não é contínua em $x=3$. 
	
    Graficamente, temos

    <center>
    <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/exemplo_2_cont.png" style="width: 50%; height: auto;"/>
    </small>
    </center> 

### Exemplo 3 

Verifique se as seguintes funções são contínuas: 

(a) $f(x)=\dfrac{x^2-x-2}{x-2}, ~a=2$

(b) $g(x)=\left\{\begin{array}{ccc}
\dfrac{1}{x^2}, & \mbox{se}& x\neq 0\\ 
1, & \mbox{se} & x=0 
\end{array}\right.$ 

\(c)  $h(x)=\left\{\begin{array}{ccc}
\dfrac{x^2-x-2}{x-2}, & \mbox{se}& x\neq 2\\ 
1, & \mbox{se} & x=0 
\end{array}\right.$

??? check "Solução"
  
    $\Large\text{Para o item (a):}$
    
    $\Large\mbox{D}(f)=\{x\in \R ~| ~ x-2\neq 0\} = \{x\in \R ~|~ x\neq 2\}$. Significa que $\Large 2$ não pertence ao domínio de $\Large f$, logo a função é descontínua em $\Large a=2$. 
	
    $\Large\text{Para o item (b):}$
    
    $\Large\mbox{D}(g)=\R$. 

    $$\Large\dlim_{x\to 0} g(x)=\dlim_{x\to 0}\dfrac{1}{x^2}=+\infty$$

    $\Large\text{como}$  $\Large\dlim_{x\to 0}g(x)$ $\Large\text{não existe, segue que}$ $\Large g(x)$ $\Large\text{é descontínua no ponto}$ $\Large a=0$. 
	
    $\Large\text{Para o item (c):}$ 
    
    $\Large\mbox{D}(h)=\R$. 
	
    $$\Large\dlim_{x\to 2} h(x)= \dlim_{x\to 2} \dfrac{x^2-x-2}{x-2}$$
    
    $$\Large =\dlim_{x\to 2} \dfrac{(x-2)(x+1)}{x-2}$$ 
    
    $$\Large =\dlim_{x\to 2} x+1=3 \neq h(3)=1$$ 

	  $\Large\text{Assim,}$ $\Large h$ $\Large\text{é descontínua em}$ $\Large a=2$. 


## Definição 

Dizemos que a função é contínua a esquerda, se o $\dlim_{x\to a^{-}} f(x)=f(a)$ e se $\dlim_{x\to a^{+}}f(x)=f(a)$, dezemos que $f$ é contínua pela direita. 


## Definição 

Dizemos que a função $f$ é contínua no intervalo $I$ se $f$ é contínua em todos os pontos de $I$. 


### Exemplo 4 

Seja $f(x)=1-\sqrt{x^2-1}$. Mostre que $f$ é contínua em $I=[-1,1]$. 

??? check "Solução"
  
    $\Large\text{Para o intervalo}$ $\Large -1<a<1$. $\Large\text{Queremos mostrar que}$

    $$\Large\dlim_{x\to a}f(x)=f(a)$$ 

    $$\Large\dlim_{x\to a} 1-\sqrt{x^2-1}=1-\sqrt{a^2-1}$$ 

    $\Large\text{Logo, se}$ $\Large -1<a<1$, $\Large\text{temos que}$ $\Large f$ $\Large\text{é contínua.}$

    $\Large\text{Analisando os laterais:}$

    $\Large\dlim_{x\to -1^{+}} f(x)=f(-1)$$ 

    $$\Large\dlim_{x\to -1^{+}} 1-\sqrt{x^2-1}=1$$ 

    $$\Large f(-1)=1-\sqrt{(-1)^2-1}=1$$ 

    $\Large\text{Assim,}$ $\Large f$ $\Large\text{é contínua em}$ $\Large -1$ $\Large\text{pela direita.}$  

    $\Large\text{Agora provaremos que}$ $\Large\dlim_{x\to 1^{-}}f(x)=f(1)$. 

    $$\Large\dlim_{x\to 1^{-}} f(x)=\dlim_{x\to 1^{-}} 1-\sqrt{1^2-1}=1$$ 

    $$\Large f(1)=1$$ 

    $\Large\text{Portanto,}$ $\Large f$ $\Large\text{é contínua no intervalo}$ $\Large I=[-1,1]$.

### Exemplo 5 

Seja $f(x)=\dfrac{x^2-x-2}{x-2}$. Verifique se $f$ é contínua em $2$.  

??? check "Solução"
  
    $\Large\text{Sabemos que}$ $\Large f$ $\Large\text{não é contínua em}$ $\Large 2$. $\Large\text{Mas,}$
	
    $$\Large\dlim_{x\to 2}\dfrac{x^2-x-2}{x-2}$$ 

    $$\Large =\dlim_{x\to 2} \dfrac{(x-2)(x+1)}{x-2}$$

    $$\Large =\dlim_{x\to 2} x+1=3$$

### Exemplo 6 

Mostre que $g(x)=\left\{\begin{array}{ccc}
\dfrac{x^2-x-2}{x-2}, & \mbox{se}& x\neq 2 \\ 
3, & \mbox{se} & x=2
\end{array}\right.$ 
é contínua em $2$?


??? check "Solução"
  
    $\Large\text{Note que}$ $\Large\mbox{D}(g)=\R$ e $\Large\dlim_{x\to 2} \dfrac{x^2-x-2}{x-2}3=f(2)$. 

    $\Large\text{De forma geral, se}$ $\Large f$ $\Large\text{é descontinua em}$ $\Large a$, 
    $\Large\text{mas}$  $\Large\dlim_{x\to a} f(x)=L$, $\Large\text{então a função}$ $\Large g$ $\Large\text{definida por}$
	
    $$\Large g(x)=\left\{\begin{array}{ccc}
    f(x), & \mbox{se}& x\neq a \\ 
    L, & \mbox{se} & x=a 
    \end{array}\right. 
    $$ 
	
    $\Large\text{é uma função contínua em}$ $\Large a$, $\Large\text{além disso, dizemos que}$ $\Large f$ $\Large\bf \text{sofre uma descontinuidade removível}$.


### Exemplo 7 

Determine o valor da constante $k$ para que $f(x)$ seja contínua em toda parte em $x_0=0$. 

$$f(x)=\left\{\begin{array}{ccc} 
\dfrac{\sqrt{1+x}-1}{x}, & \mbox{se} & x>0\\ 
3x^2-4x+k, & \mbox{se} & x\leqslant 0 
\end{array}\right.$$ 


??? check "Solução"
  
    $\Large\text{Queremos verificar}$
	
    $$\Large\dlim_{x\to x_0} f(x)=f(x_0)$$ 

    $$\Large\dlim_{x\to 0} f(x)=f(0)$$ 

    $\Large\text{Calculando os limites laterais,}$

    $$\Large\dlim_{x\to 0^{+}} \dfrac{\sqrt{1+x}-1}{x}$$

    $$\Large = \dfrac{0}{0} \rightarrow \mbox{Indeterminação} $$ 

    $\Large\text{Precisamos retirar a indeterminação, racionalizamos}$

    $$\Large =\dlim_{x\to 0^{+}} \dfrac{(\sqrt{1+x}-1)(\sqrt{1+x}+1)}{x(\sqrt{1+x}+1)}$$ 

    $$\Large =\dlim_{x\to 0^{+}} \dfrac{[(\sqrt{1+x})^2-(1)^2]}{x(\sqrt{1+x}+1)}$$ 

    $$\Large =\dlim_{x\to 0^{+}} \dfrac{1+x-1}{x(\sqrt{1+x}+1)}$$

    $$\Large =\dlim_{x\to 0^{+}} \dfrac{x}{x(\sqrt{1+x}+1)}$$

    $\Large\text{Simplificando,}$ 

    $$\Large =\dlim_{x\to 0^{+}} \dfrac{1}{\sqrt{1+x}+1}$$

    $\Large\text{Fazendo novamente,}$ $\Large x\to 0^{+}$, $\Large\text{temos}$

    $$\Large =\dfrac{1}{\sqrt{1+0}+1}=\dfrac{1}{2}$$

    $\Large\text{Calculando o limite lateral pela esquerda,}$

    $$\Large \dlim_{x\to 0^{-}} 3x^2-4x+k=k$$ 

    $\Large\text{Para o limite}$ $\Large\dlim_{x\to 0} f(x)$ $\Large\text{existir, temos}$

    $$\Large\dlim_{x\to 0^{-}}f(x)=\dlim_{x\to 0^{+}} f(x) \Rightarrow $$ 

    $$\Large k=\dfrac{1}{2}$$ 

    $\Large\text{Assim, temos também que}$ $\Large\dlim_{x\to 0}f(x)=f(0)=\dfrac{1}{2}$.



## Teorema 

Seja $f$ e $g$ duas funções contínuas então as seguintes funções são contínuas:  

(i) $f+g$; 

(ii) $f\cdot g$;

(iii) $\lambda \cdot f, ~\lambda \in \R$; 

(iv) $\dfrac{f}{g}, \mbox{desde que}~ \dlim_{x\to a}g(x)\neq 0$ 

## Teorema 2 

As seguintes funções são contínuas em seus domínios: 

(i) Funções polinomiais; 

(ii) Funções racionais; 

(iii) Funções trigonométricas e suas inversas;

(iv) Funções exponenciais e suas inversas 


Veja que uma função é dita racional se, 
	
$$f(x)=\dfrac{P(x)}{Q(x)}$$ 
	
onde $P$ e $Q$ são polinômio com $\mbox{D}(f)=\left\{x\in \R ~|~ Q(x)\neq 0 \right\}$.


### Exercícios 

1. Encontre os pontos de continuidade da função $f(x)=\displaystyle\frac{x^3-27}{x^2-3x+2}$. 


??? check "Solução do exercício 1"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/y8124fk78i4"></iframe>
    </p>


