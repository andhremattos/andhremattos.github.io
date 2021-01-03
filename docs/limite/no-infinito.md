
# **No infinito**

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


## Definição 

O $\dlim_{x\to -\infty} f(x)=L$, se $\forall M > 0, \exists N < 0$ tal que 
$x< N \Rightarrow |f(x)-L|< M$. 


Graficamente temos:

<center>
    <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/no_infinito_1.png" style="width: 50%; height: auto;"/>
    </small>
</center>

## Teorema 

Seja $P(x)=a_0+a_1x+\cdots+a_nx^n$ e $Q(x)=b_0+b_1x+\cdots+b_mx^m$, então 
	
$$\dlim_{x\to +\infty} \dfrac{P(x)}{Q(x)}=\dlim_{x\to +\infty} \dfrac{a_nx^n}{b_mx^m}$$ 

e 

$$\dlim_{x\to -\infty} \dfrac{P(x)}{Q(x)}=\dlim_{x\to -\infty} \dfrac{a_nx^n}{b_mx^m}$$ 


### Demonstração 

Seja $P(x)=a_0+a_1x_1+a_2x_2+\cdots + a_nx^n$ 

$$=a_nx^n\left(\dfrac{a_0}{a_nx^n}+\dfrac{a_1x}{a_nx^n}+\cdots+\dfrac{a_nx^n}{a_nx^n}\right)$$ 

$$=a_nx^n\left(\dfrac{a_0}{a_nx^n}+\dfrac{a_1}{a_nx^{n-1}}+\cdots+1\right)$$ 

E $Q(x)=b_mx^m\left(\dfrac{b_0}{b_mx^m}+\dfrac{b_1}{b_mx^{m-1}}+\cdots+1\right)$ 

Calculando o limite, 

$$\dlim_{x\to +\infty} \dfrac{P(x)}{Q(x)} = \dlim_{x\to +\infty} \dfrac{ a_nx^n\left(\overbrace{\dfrac{a_0}{a_nx^n}}^{=0}+\overbrace{\dfrac{a_1}{a_nx^{n-1}}}^{=0}+\cdots+1\right)}{b_mx^m\left(\underbrace{\dfrac{b_0}{b_mx^m}}_{=0}+\underbrace{\dfrac{b_1}{b_mx^{m-1}}}_{=0}+\cdot+1\right)} $$ 

$$\dlim_{x\to +\infty} \dfrac{a_n x^n}{b_mx^m}$$ 

**Casos Possíveis:**


+  Se $n=m$ 

$$ \dlim_{x\to +\infty} \dfrac{P(x)}{Q(x)} = \dlim_{x\to +\infty} \dfrac{a_n x^n}{b_mx^m} = \dfrac{a_n}{b_m}$$ 

+  Se $n>m \Rightarrow n=m+r$ 

	$$\dlim_{x\to +\infty} \dfrac{P(x)}{Q(x)} = \dlim_{x\to +\infty} \dfrac{a_n x^n}{b_mx^m}$$
  
  $$=\dlim_{x\to +\infty} \dfrac{a_n x^{m+r}}{b_mx^{m}} $$
  
  $$=\dlim_{x\to +\infty} \dfrac{a_n x^{r}}{b_m}=+\infty $$ 


+ Se $n< m \Rightarrow m=n+s$ 

$$\dlim_{x\to +\infty} \dfrac{P(x)}{Q(x)} $$ 

$$= \dlim_{x\to +\infty} \dfrac{a_n x^{n}}{b_m x^{m}}$$ 

$$= \dlim_{x\to +\infty} \dfrac{a_n x^{n}}{b_m x^{n+s}}$$ 

$$=\dlim_{x\to +\infty} \dfrac{ a_n}{b_m x^{s}} = 0 $$

## Teorema 2 

Se $r>0$ é um número racional, então 

$$\dlim_{x\to +\infty} \dfrac{1}{x^r}=0$$ 

$$ ~\mbox{ou}~ \dlim_{x\to -\infty} \dfrac{1}{x^r}=0$$ 


## Exemplo 1 

Determine o limite $\dlim_{x\to +\infty} \dfrac{1}{x^4}$. 

??? check "Solução"

    $\Large\text{Temos,}$
 	
    $$\Large\dlim_{x\to +\infty} \dfrac{2}{x^4}$$
   
    $$\Large =2\cdot \dlim_{x\to +\infty} \dfrac{1}{x^4}=0$$


## Exemplo 2 

Determine o limite $\dlim_{x\to +\infty} \dfrac{2x}{x^2+1}.$

??? check "Solução"
    $\Large\text{Temos,}$
	
	  $$\Large\dlim_{x\to +\infty} \dfrac{2x}{x^2+1} $$ 

	  $\Large\text{Pegamos o termo de}$ $\Large x$ $\Large\text{de maior grau, ou seja,}$ $\Large x^2$, $\Large\text{e dividimos toda a expressão, ou seja, o numerador e denominador,}$ 
	
	  $$\Large\dlim_{x\to +\infty} \dfrac{ \dfrac{2x}{x^2}}{\dfrac{x^2+1}{x^2}} $$ 
   
    $$\Large =\dlim_{x\to +\infty} \dfrac{\dfrac{2}{x}}{1+\dfrac{1}{x^2}} $$
   
    $$\Large = \dfrac{0}{1+0}=0 $$


## Exemplo 3 

Determine o limite $\dlim_{x\to +\infty} \dfrac{x^7+8x^2+5x}{4x^3+2x^2+x-6}$. 

??? check "Solução"
    $\Large\text{Temos que o termo de maior grau do denominador, que é}$ $\Large x^3$, $\Large\text{portanto, dividimos toda a expressão por esse termo,}$ 
	
    $$\Large \dlim_{x\to +\infty} \dfrac{ \dfrac{x^7+8x^2+5x}{x^7}}{\dfrac{4x^3+2x^2+x-6}{x^3}} $$
    
    $$\Large = \dlim_{x\to +\infty} \dfrac{x^4+\dfrac{8}{x}+\dfrac{5}{x^2}}{4+\dfrac{2}{x}+\dfrac{1}{x^2}} $$ 
	
    $$\Large = \dfrac{+\infty}{4}=+\infty $$ 


## Exemplo 4 

Determine $\dlim_{x\to -\infty} \dfrac{2x^9+4x^2+x^5}{4x^9+3x^3}$.  

??? check "Solução"
    $\Large\text{Temos que o termo de maior grau do denominador é dado por}$ $\Large x^9$, $\Large\text{logo dividimos toda a expressão por}$ $\Large x^9$: 
	
    $$\Large \dlim_{x\to -\infty} \dfrac{ \dfrac{2x^9+4x^2+x^5}{x^9}}{\dfrac{4x^9+3x^3}{x^9}} $$
    
    $$\Large = \dlim_{x\to -\infty} \dfrac{ 2+\dfrac{4}{x^7}+\dfrac{1}{x^4}}{4+\dfrac{3}{x^6}} $$
    
    $$\Large = \dfrac{2}{4}= \dfrac{1}{2}$$ 


## Exemplo 5 

Determine o limite $\dlim_{x\to -\infty} \dfrac{5x^{100}+7x^2+800x^{2}}{100x^{1000}+2x^{999}+x}$. 

??? check "Solução"
    $\Large\text{Temos,}$
	
	  $$\Large \dlim_{x\to -\infty} \dfrac{ 5x^{100}}{100x^{1000}} $$ 
    
    $$\Large =\dlim_{x\to -\infty} \dfrac{5}{100}\dfrac{1}{x^{900}}=0$$ 


## Exemplo 6 

Determine $\dlim_{x\to +\infty}\dfrac{ \sqrt{x^2+2}}{x+1}$.

??? check "Solução"
    $\Large\text{Dividimos toda a expressão por}$ 

    $$\Large\sqrt{x^2}=|x|= \left\{\begin{array}{cccc}
    x, & \mbox{se} & x\geqslant 0  &\\
    -x, & \mbox{se} & x < 0&
    \end{array}\right.$$

    $$\Large\dlim_{x\to +\infty} \dfrac{\dfrac{\sqrt{x^2+2}}{\sqrt{x^2}}}{\dfrac{x+1}{\sqrt{x^2}}}$$ 
	
    $$ \Large = \dlim_{x\to +\infty} \dfrac{ \sqrt{\dfrac{x^2+2}{x^2}}}{\dfrac{x+1}{|x|}}$$ 
		
    $\Large\text{Como}$ $\Large x\to +\infty$, $\Large |x|=x$ 
	
    $$\Large =\dlim_{x\to +\infty} \dfrac{ \sqrt{1+\dfrac{2}{x^2}}}{1+\dfrac{1}{x}}$$ 
    
    $$\Large = \dfrac{ \sqrt{1+0}}{1+0} = 1$$ 
	
	
## Exemplo 7 

Determine $\dlim_{x\to +\infty} \dfrac{ \sqrt{x^4+2x}}{x^2+5x}$.  

??? check "Solução"
    $\Large\text{Dividimos toda a expressão por}$ $\Large\sqrt{x^4}$, 
	
    $$\Large\dlim_{x\to +\infty} \dfrac{ \dfrac{\sqrt{x^4+2x}}{\sqrt{x^4}}}{\dfrac{x^2+5x}{\sqrt{x^4}}}$$
    
    $$\Large =\dlim_{x\to +\infty} \dfrac{ \sqrt{\dfrac{x^4+2x}{x^4}}}{\dfrac{x^2+5x}{x^2}}$$
	
    $$\Large =\dlim_{x\to +\infty} \dfrac{ \sqrt{ 1+\dfrac{2}{x^3}}}{1+\dfrac{5}{x}}$$
    
    $$\Large = \dfrac{\sqrt{1+0}}{1+0}=1$$ 

## Exemplo 8 

Determine $\dlim_{x\to -\infty} \dfrac{ \sqrt{x^2+2}}{x+1}$.


??? check "Solução"

    $\Large\text{Dividindo toda a expressão por}$ $\Large\sqrt{x^2}$. $\Large\text{Recorde-se também que}$ 
    
    $\Large\sqrt{x^2}=|x|=\left\{\begin{array}{ccc}
    x, & \mbox{se} & x\geqslant 0 \\ 
    -x, & \mbox{se} & x< 0 
    \end{array}\right.$ 


    $\Large\text{Logo, temos}$
	
    $$\Large \dlim_{x\to -\infty} \dfrac{ \dfrac{\sqrt{x^2+2}}{\sqrt{x^2}}}{\dfrac{x+1}{\sqrt{x^2}}}$$ 
    
    $$\Large = \dlim_{x\to -\infty} \dfrac{ \sqrt{ \dfrac{x^2+2}{x^2}}}{\dfrac{x+1}{-x}}$$ 


    $\Large\text{Veja que}$ $\Large\sqrt{x^2}=|x|=-x$, $\Large\text{se}$ $\Large x\to -\infty$. 
	
    $$\Large\dlim_{x\to -\infty} \dfrac{ \sqrt{1+\dfrac{2}{x^2}}}{-1-\dfrac{1}{x}} $$
    
    $$\Large = \dfrac{\sqrt{1+0}}{-1-0} = - 1 $$ 


## Exemplo 9

Determine o seguinte limite $\dlim_{x\to +\infty} (\sqrt{x^2-3x+7}-\sqrt{x^2+1})$. 

??? check "Solução"

    $\Large\text{Fazendo}$ $\Large x\to +\infty$, $\Large\text{temos}$ 

    $$\Large=\dlim_{x\to +\infty} (\sqrt{x^2-3x+7}-\sqrt{x^2+1})=+\infty-\infty \rightarrow \mbox{Indeterminação} $$ 

    $\Large\text{Precisamos retirar a indeterminação, para isso racionalizamos,}$ 

    $$\Large=\dlim_{x\to +\infty}\dfrac{ [(\sqrt{x^2-3x+7}-\sqrt{x^2+1})][ (\sqrt{x^2-3x+7}+\sqrt{x^2+1})]}{ (\sqrt{x^2-3x+7}+\sqrt{x^2+1})}$$ 

    $$\Large=\dlim_{x\to +\infty}\dfrac{ [(\sqrt{x^2-3x+7})^2-(\sqrt{x^2+1})^2]}{ (\sqrt{x^2-3x+7}+\sqrt{x^2+1})}$$

    $$\Large=\dlim_{x\to +\infty}\dfrac{x^2-3x+7-x^2-1}{ (\sqrt{x^2-3x+7}+\sqrt{x^2+1})}$$

    $\Large\text{Simplificando,}$

    $$\Large=\dlim_{x\to +\infty}\dfrac{-3x+6}{ (\sqrt{x^2-3x+7}+\sqrt{x^2+1})}$$

    $\Large\text{Dividindo numerador e denominador por}$ $\Large \sqrt{x^2}$, 

    $$\Large=\dlim_{x\to +\infty}\dfrac{\dfrac{-3x+6}{\sqrt{x^2}}}{\dfrac{ (\sqrt{x^2-3x+7}+\sqrt{x^2+1})}{\sqrt{x^2}}}$$

    $\Large\text{Sabemos que}$ 
    
    $$\Large\sqrt{x^2}=|x|=\left\{\begin{array}{ccc} 
    x, & \mbox{se} & x\geq 0\\ 
    -x, & \mbox{se} & x<0 
    \end{array}\right. $$ 

    $\Large\text{Veja que para}$ $\Large x\to +\infty$, $\Large \sqrt{x^2}=x$. $\Large\text{Logo, temos}$

    $$\Large=\dlim_{x\to +\infty}\dfrac{\dfrac{-3x}{x}+\dfrac{6}{x}}{ \left(\sqrt{\dfrac{x^2-3x+7}{x^2}}+\sqrt{\dfrac{x^2+1}{x^2}}\right)}$$

    $$\Large=\dlim_{x\to +\infty}\dfrac{-3+\dfrac{6}{x}}{ \left(\sqrt{1-\dfrac{3}{x}+\dfrac{7}{x^2}}+\sqrt{1+\dfrac{1}{x^2}}\right)}$$

    $\Large\text{Fazendo}$ $\Large x\to +\infty$, $\Large\text{temos}$

    $$\Large=\dfrac{-3+0}{ \left(\sqrt{1-0+0}+\sqrt{1+0}\right)}=-\dfrac{3}{2}$$


## Propriedades 


+ Para um $a>1$: 


(i)$\dlim_{x\to +\infty} a^{x}=+\infty$ 

(ii)$\dlim_{x\to -\infty} a^{x}=0$ 


<center>
    <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/no_infinito_2_a.png" style="width: 50%; height: auto;"/>
    </small>
</center>

+ Para um $0<a<1$: 
	
(iii) $\dlim_{x\to +\infty} a^{x}=0$ 

(iv) $\dlim_{x\to -\infty} a^{x}=+\infty$ 


<center>
    <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/no_infinito_2_b.png" style="width: 50%; height: auto;"/>
    </small>
</center>


??? check "Limite no infinito"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/obYV7Bp5OPg"></iframe>
    </p>

??? check "Limite no infinito 4"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/Dsdd5cw_oAw"></iframe>
    </p>

??? check "Limite no infinito 5"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/MWy0KqzXqFk"></iframe>
    </p>






