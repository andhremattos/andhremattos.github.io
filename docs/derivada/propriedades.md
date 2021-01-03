# **Propriedades**

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
</style>



1. Se $f(x)=c$, onde $c \in (-\infty, +\infty)$, então $\frac{\mbox{d}}{\dx}\left[f(x)\right]=0$. 


**Demonstração**: 

Usando a definição de derivada, temos 

$$f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ f(x+\Delta x)-f(x)}{\Delta x}$$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{ c-c}{\Delta x} = 0$$ 

Logo, $f'(x)=0$.


2. Sejam $f$ uma função, $c$ uma constante e $g$ uma função por: 

$$g(x)=c\cdot f(x)$$ 

se $f'(x)$ existe, então 

$$ g'(x)=c\cdot f'(x)$$  

**Demonstração**: 


Por hipótese temos: 
	
$$f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{f(x+\Delta x)-f(x)}{\Delta x} $$ existe. 
	
Portanto, 

$$g'(x)= \displaystyle\lim_{\Delta x\to 0} \frac{g(x+\Delta x)-g(x)}{\Delta x}$$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{c\cdot f(x+\Delta x)-c\cdot f(x)}{\Delta x} $$
	
$$= c\cdot \displaystyle\lim_{\Delta x\to 0} \frac{f(x+\Delta x)- f(x)}{\Delta x} $$


$$= c\cdot f'(x)$$ 


3. Se $f(x)=x^{n}$, então 

$$\frac{\mbox{d}}{\dx}\left[x^{n}\right]=nx^{n-1}$$ 

**Demonstração**: 

$$f'(x)= \displaystyle\lim_{x\to a} \left(x^{n-1}+ax^{n-1}+\cdots + a^{n-1}x+a^{n-1}\right)$$ 
	
$$ = na^{n-1}$$ 

Logo, $a$ foi escolhido arbitrariamente, segue que 
	
$$f'(x)=nx^{n-1}$$ 

4. Sejam $f$ e $g$ funções deriváveis e $h$ definida por $h(x)=f(x)\cdot g(x)$, então $h$ é derivável e sua derivada é: 

$$\frac{\mbox{d}}{\dx}\left[h(x)\right]=f'(x)\cdot g(x)+f(x)\cdot g'(x)$$

**Demonstração**: 

Usando a definição de derivada, temos 

$$h'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ f(x+\Delta x)\cdot g(x+\Delta x)-f(x)\cdot g(x)}{\Delta x}$$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{ f(x+\Delta x)\cdot g(x+\Delta x)-f(x+\Delta x)g(x)+f(x+\Delta x)\cdot g(x)-f(x)\cdot g(x)}{\Delta x}$$ 

$$=\displaystyle\lim_{\Delta x\to 0} f(x+\Delta x)\left[\frac{ g(x+\Delta x)-g(x)}{\Delta x}\right]+\displaystyle\lim_{\Delta x\to 0} g(x)\left[\frac{f(x+\Delta x)-f(x)}{\Delta x}\right]$$ 

$$=f(x)\cdot g'(x)+g(x)\cdot f'(x)$$ 

Logo, 

$$\left[f\cdot g\right]'=f'\cdot g+ g'\cdot f$$ 


5. Sejam $f(x)$ e $g(x)$ funções deriváveis e $h(x)$ definida por $h(x)\frac{f(x)}{g(x)}$, com  $g(x)\neq 0$. Então, $h(x)$ é derivável e sua derivada é: 
 
$$h'(x)=\frac{ f'(x)\cdot g(x)-f(x)\cdot g'(x)}{g(x)^2}$$ 

**Demonstração**: 

Temos, 

$$f'(x)=\frac{ g(x)\cdot f'(x)-f(x)\cdot g'(x)}{[g(x)]^2}$$

$$f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ f(x+\Delta x) - f(x)}{\Delta x} $$ 

$$g'(x)=\lim_{\Delta x\to 0} \frac{g(x+\Delta x)-g(x)}{\Delta x}$$ 

$$h'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ h(x+\Delta x)-h(x)}{\Delta x}$$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{ \frac{f(x+\Delta x)-f(x)}{g(x+\Delta x)-g(x)}}{\Delta x}$$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{1}{\Delta x} \left[\frac{f(x+\Delta x)g(x)-f(x)g(x+\Delta x)}{g(x+\Delta )g(x)}\right]$$ 

Subtraindo e adicionando $f(x)\cdot g(x)$ ao numerador, obtemos 

$$h'(x)= \displaystyle\lim_{\Delta x\to 0} \frac{1}{\Delta x} \left[\frac{ f(x+\Delta x)g(x)-f(x)g(x)+f(x)g(x)-f(x)g(x+\Delta x)}{g(x+\Delta x)g(x)}\right]$$ 

$$= \displaystyle\lim_{\Delta x\to 0 }\frac{ \left[\left(\frac{f(x+\Delta x)-f(x)}{\Delta x}\right)\cdot g(x)-f(x)\cdot\left( \frac{g(x+\Delta x)-g(x)}{\Delta x} \right)\right]}{g(x+\Delta x)g(x)}$$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{ f(x+\Delta x)-f(x)}{\Delta x} \cdot \displaystyle\lim_{\Delta x\to 0} g(x) - \displaystyle\lim_{\Delta x\to 0} f(x)\cdot \displaystyle\lim_{\Delta x\to 0} \frac{ g(x+\Delta x)-g(x)}{\Delta x} $$ 

Portanto, 

$$h'(x)=\frac{ f'(x)g(x)-f(x)g'(x)}{[g(x)]^2} $$


### Exemplo 1 

Derive $y=\frac{x^2-10}{x^3+2x}$. 

??? check "Solução"
  
    $\Large \text{Derivando, temos}$ 

    $$\Large y'=\frac{ 2x(x^3+2x)-(x^2-10)(3x^2+2)}{(x^3+2x)^2}$$ 
	
    $$\Large y'=\frac{2x^4+4x^2-3x^4-2x^2+30x^2+20}{(x^3+2x)^2}$$ 
    
    $\Large \text{Simplificando, }$ 

    $$\Large y'=\frac{-x^4+32x^2+20}{(x^3+2x)^2}$$ 

6. Se $f(x)=a^{x}$, onde $a>0$ e $a\neq 1$, então $f'(x)=a^{x}\ln{(a)}$.  

**Demonstração**: 

Calculando a derivada pela definição, temos 

$$f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ f(x+\Delta )-f(x)}{\Delta x} $$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{ a^{x+\Delta x}-a^{x}}{\Delta x} $$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{a^{x}(a^{\Delta x}-1)}{\Delta x} $$ 

$$= a^{x}\cdot \displaystyle\lim_{\Delta x\to 0} \frac{ a^{\Delta x} -1 }{\Delta x} = a^{x}\cdot \ln{(a)}$$ 

Logo, $f'(x)=a^{x}\cdot \ln{(a)}$. Em particular, se $a=e$, então 

$$f(x)=e^{x} \Rightarrow f'(x)=e^{x}\ln{(e)} = e^{x}$$


### Exemplo 2 

Diferencie $f(x)=4x^2+5x^{10}+\sqrt[3]{4}$. 

??? check "Solução"
  
    $\Large \text{Derivando, temos}$ 
	
    $$\Large f'(x)= (4x^2)'+(5x^{10})'+(\sqrt[3]{4})'$$ 
	
    $$\Large f'(x)= 8x+50x^9$$ 


### Exemplo 3 

Diferencie $f(x)=-x^5+4x^6-7e^{x}$.  

??? check "Solução"
  
    $\Large \text{Derivando, temos}$  

    $$\Large f'(x)= (-x^5)'+(4x^6)'-(7e^x)'$$ 

    $$\Large f'(x)= -5x^4+24x^5-7e^{x} $$


### Exemplo 4 

Diferencie $y=(4x^7+\sqrt{x})\cdot (\sqrt[3]{x}+\pi)$. 

??? check "Solução"
  
    $\Large \text{Temos o produto de duas funções, assim aplicando a regra do produto,}$  
	
    $$\Large\frac{\dy}{\dx} =(4x^7+\sqrt{x})'\cdot (\sqrt[3]{x}+\pi)+ (4x^7+\sqrt{x})\cdot (\sqrt[3]{x}+\pi)'$$ 
	
    $$\Large = \left[(4x^7)'+(\sqrt{x})'\right]\cdot(\sqrt[3]{x}+\pi)+ \left[(4x^7+\sqrt{x})\cdot (\sqrt[3]{x}+\pi)\right] $$ 
    $$\cdots$$ 
	
    $$\Large \frac{\dy}{\dx} = \frac{88}{3}x^{\frac{19}{3}}+\frac{3}{6}x^{-\frac{1}{6}}+28\pi x^6+\frac{\pi}{2}x^{-\frac{1}{2}} $$ 


### Exemplo 5 

Diferencie $y=4^x\cdot x^6$.  

??? check "Solução"
  
    $\Large \text{Derivando usando a regra do produto, temos}$ 
	
    $$\Large\frac{\dy}{\dx}= (4^x\cdot x^6)' = (4^x)'(x^6)+(4^x)(x^6)'$$ 
	
    $$\Large =4^x\ln{(4)}x^6+6x^5\cdot 4^x $$ 
	
    $$\Large =4^x\cdot x^5(\ln{(4)} \cdot x+6)$$ 

### Exemplo 6 

Diferencie $y=\frac{10^x}{20x^2+\sqrt[5]{x}}$.  

??? check "Solução"
  
    $\Large \text{Temos o quociente de duas funções, aplicamos então a regra do quociente,}$  
	
    $$\Large\frac{\dy}{\dx} = \frac{ (10^x)'\cdot (20x^2+\sqrt[5]{x})-(20x^2+\sqrt[5]{x})'(10^x)}{(20x^2+\sqrt[5]{x})^2} $$ 
	
    $$\Large =\frac{10^x\ln{(10)}(20x^2+\sqrt[5]{x})-(10^x)\left(40x+\frac{1}{5}x^{-\frac{4}{5}}\right)}{(20x^2+\sqrt[5]{x})^2} $$ 
	
    $$\Large = \frac{ 10^x \left[(20x^2\ln{(10)}+\sqrt[5]{x}\ln{(10)})-40x-\frac{1}{5}x^{-\frac{4}{5}}\right]}{(20x^2+\sqrt[5]{x})^2} $$ 

### Exemplo 7 

Diferencie $y=\frac{ e^x\cdot 7^x}{7x^2}$. 

??? check "Solução"
  
    $$\Large \frac{\dy}{\dx}= \frac{ (e^x 7^x)'(7x^2)- (7x^2)'(e^x 7^x)}{(7x^2)^2} $$ 
	
    $$\Large = e^{x}7^x \frac{ \left(7x^2+7x^2\ln{(7)}-14x\right)}{49x^4}$$ 

## Derivadas de Funções Trigonométricas 


1. Se $f(x)=\sen(x)$, então 

$$\frac{\mbox{d}}{\dx} \left(\sen(x)\right)= \cos(x)$$  

**Demonstração**: 


Consideremos a seguinte relação trigonométrica 

$$\sen(p)-\sen(q)= 2\cdot \sen\left(\frac{p-q}{2}\right)\cos\left(\frac{p+q}{2}\right)$$ 

Por definição de derivada, temos:  

$$f'(x)= \displaystyle\lim_{\Delta x\to 0} \frac{ \sen(x+\Delta x)-\sen(x)}{\Delta x}$$ 

Aplicando uma identidade do seno da soma, temos 

$$= \displaystyle\lim_{\Delta x\to 0} \frac{ \cos(x)\sen(\Delta x) + \cos(\Delta x)\sen(x)-\sen(x)}{\Delta x} $$ 

Separando os limites, 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{ \cos(x)\sen(\Delta x)}{\Delta x} + \displaystyle\lim_{\Delta x\to 0} \frac{ \sen(x)(\cos(\Delta)-1)}{\Delta x}$$ 

$$=\cos(x)-\sen(x)\cdot \displaystyle\lim_{\Delta x\to 0} \frac{ \cos(\Delta x)-1}{\Delta x}$$ 

Verifique que $\displaystyle\lim_{\Delta x\to 0} \frac{ \cos(\Delta x)-1}{\Delta x} = 0$. 

Logo, 

$$f'(x)=\cos(x)-\sen(x)\cdot 0$$ 

$$f'(x)=\cos(x)$$ 

2. Se $f(x)=\cos(x)$, então 

$$\frac{\mbox{d}}{\dx} \left[ \cos(x)\right] = - \sen(x)$$ 

**Demonstração**: 

Consideremos a seguinte relação trigonométrica 

$$\cos(p)-\cos(q)= -2\cdot \sen\left(\frac{p-q}{2}\right)\sen\left(\frac{p+q}{2}\right)$$ 

Por definição de derivada, temos:

$$f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{ \cos(x+\Delta x)-\cos(x)}{\Delta x} $$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{ \cos(x)\cos(\Delta x)-\sen(x)\sen(\Delta x)-\cos(x)}{\Delta x} $$ 

$$=\displaystyle\lim_{\Delta x\to 0} \frac{ \cos(x)(\cos(\Delta x)-1)}{\Delta x} - \displaystyle\lim_{\Delta x\to 0} \frac{\sen(x)\sen(\Delta x)}{\Delta x} $$ 

$$=-\cos(x)\displaystyle\lim_{\Delta x\to 0} \frac{1-\cos(\Delta x)}{\Delta x} - \sen(x)\displaystyle\lim_{\Delta x\to 0} \frac{ \sen(\Delta x)}{\Delta x} $$ 

$$ =-\cos(x)\cdot 0 - \sen(x)\cdot 1$$ 

$$f'(x)=-\sen(x)$$ 

**Comentário**: 

> Como as demais funções trigonométricas decorrem do seno e do cosseno, podemos derivá-los usando as regras de derivação. 

3. Se $f(x)=\tg(x)$, então 

$$\frac{\mbox{d}}{\dx}[\tg(x)]=\sec^{2}(x)$$ 

**Demonstração**:  

Pela regra do quociente, temos:

$$f(x)=\frac{\sen(x)}{\cos(x)}$$ 

$$f'(x)=\frac{(\sen(x))'(\cos(x))-(\sen(x))(\cos(x))'}{\cos^2(x)}$$ 

$$= \frac{ \cos(x)\cos(x)+\sen(x)\sen(x)}{\cos^2(x)}$$

$$=\frac{ \cos^2(x)+\sen^2(x)}{\cos^2(x)}$$ 

$$=\frac{1}{\cos^2(x)}$$ 

$$f'(x)=\sec^2(x)$$ 

4. Se $f(x)=\sec(x)$, então 

$$\frac{\mbox{d}}{\dx} \left[\sec(x)\right]= \tg(x)\sec(x)$$  

**Demonstração**:  
	
Faça, usando o mesmo raciocínio aplicado para a derivada de $\tg(x)$. 

5. Se $f(x)=\mbox{cossec}(x)$, então 

$$\frac{\mbox{d}}{\dx} [\mbox{cossec}(x)] = -\cotg(x)\mbox{cossec}(x)$$ 
 

6. Se $f(x)=\cotg(x)$, então 

$$\frac{\mbox{d}}{\dx} = -\mbox{cossec}^{2}(x)$$

### Exemplo 

Diferencie $y=\frac{ \cos(x)\cdot 2^{x}}{\sqrt[3]{x}\cdot \sen(x)}$. 

??? check "Solução"
  
    $\Large \text{Podemos reescrever a função,}$ 
	
    $$\Large y=\frac{2^{x}}{\sqrt[3]{x}} \cdot \frac{\cos(x)}{\sen(x)} = \frac{ 2^{x}\cotg(x)}{\sqrt[3]{x}}$$ 
	
    $\Large \text{Diferenciando, temos}$ 

    $$\Large \frac{dy}{\dx}=\frac{(2^{x}\cdot \ln{(2)}\cdot \cotg(x)-2^{x}\mbox{cossec}^{2}(x))\sqrt[3]{x}-2^{x}\cotg(x)x^{-\frac{2}{3}}}{(\sqrt[3]{x})^2}$$ 

    $$\Large \frac{\dy}{\dx}= 2^{x}\left[ x^{-\frac{1}{3}}\ln{(x)}\cotg(x)-\mbox{cossec}^{2}(x)x^{-\frac{1}{3}}-\frac{1}{3}\cotg(x)x^{-\frac{4}{3}}\right]$$ 

## Derivada da Função Composta 

Seja $y=f(x)$ uma função composta, isto é,  uma função $Q$ que pode ser escrita como $y=F(u)$ e $u=\varphi(x)$, ou $y=F[\varphi(x)]$.

**Teorema** 

Se $u$ é uma função derivável no ponto $x$ e $y$ é uma função derivável no ponto correspondente $u$, então a função composta $y=F[\ln{(x)}]$ tem uma derivada no ponto $x$ dada por: 
	
	$$\frac{\dy}{\dx} = \frac{\dy}{\du}\cdot \frac{\du}{\dx}$$ 

	$u$ variável intermediária. 

  ## Regra da Cadeia 

**Teorema**: Se $f(x)$ e $g(x)$ forem diferenciáveis e $F=f\textopenbullet g$ por uma função composta definida por $F(x)=f[g(x)]$, então $F$ é diferenciável e $F'$ é dada por 
	
$$F'(x)=f'[g(x)]\cdot g'(x)$$ 
	
Ou pela notação de Leibnz: 
	
Seja $y=F[g(x)]$, sua derivada, $\frac{\dy}{\dx}$ é dada por: 
	
$y=F[u], \quad u=g(x)$. 
	
$$\frac{\dy}{\dx}=\frac{\dy}{\du}\cdot \frac{\du}{\dx}= F'[u]\cdot g'(x)$$ 
	
$$\frac{\dy}{\dx}=F'[g(x)]\cdot g'(x)$$ 

### Exemplo 

Diferencie $y=\cos(2x)$.

??? check "Solução"
  
    $\Large \text{Façamos}$ $\Large y=\cos(u); \quad u=2x$ 
	
    $$\Large \frac{\dy}{\dx}= \frac{\dy}{\du}\cdot \frac{\du}{\dx} = -\sen(u)\cdot 2 $$ 
	
    $$\Large \frac{\dy}{\dx} = -2\sen(2x)$$ 


### Exemplo 

Diferencie $y=\sen^{3}(x)$. 

??? check "Solução"
  
    $\Large \text{Façamos}$ $\Large y=\varphi^{3}; \quad \varphi = \sen(x)$ 
	
    $$\Large \frac{\dy}{\dx}=\frac{\dy}{\mbox{d}\varphi}\cdot \frac{\mbox{d}\varphi}{\dx}$$ 
  
    $$\Large = 3\varphi^{2}\cdot \cos(x)$$ 
	
    $$\frac{\dy}{\dx} = 3\cos(x)\sen^2(x)$$ 


### Exemplo 

Diferencie $y=e^{(7x^2-2x)}$.  


??? check "Solução"
  
    $\Large \text{Façamos}$  $\Large y=e^{\varphi}; \quad \varphi = 7x^2-2x$ 
	
    $$\Large \frac{\dy}{\dx}=\frac{\dy}{\du}\cdot \frac{\du}{\dx} $$ 
	
    $$\Large \frac{\dy}{\dx}= e^{\varphi}\cdot (14x-2)$$ 
    $$\Large \frac{\dy}{\dx}= e^{(7x^2-2x)} \cdot (14x-2)$$ 


### Exemplo 

	Diferencie $y=(x^2-x+1)^{23}$. 
	

??? check "Solução"
  
    $\Large \text{Façamos}$ $\Large y=\varphi^{23}; \quad \varphi= x^2-x+1$ 
	
    $$\Large \frac{\dy}{\dx}=\frac{\dy}{\mbox{d}\varphi}\cdot \frac{\mbox{d}\varphi}{\dx}$$ 
    
    $$\Large = 23\varphi^{22}\cdot (2x-1)$$ 
	
    $$\Large \frac{\dy}{\dx} = 23(x^2-x+1)^{22}\cdot (2x-1)$$ 


### Exemplo 

Diferencie $y=\sqrt{x^3+\mbox{cossec}(x)}$ 

??? check "Resposta"
  
    $$\frac{\dy}{\dx}=\frac{3x^2-\mbox{cossec}(x)\cotg(x)}{2\sqrt{x^3+\mbox{cossec}(x)}}$$ 


###  Exemplo 

Diferencie $y=\sqrt[3]{x^2+1}$ 


??? check "Solução"
  
    $\Large \text{Temos}$  $\Large y=\sqrt[3]{x^2+1}$, $\Large \text{reescrevendo a função, temos}$
	
    $$\Large y=\left(x^2+1\right)^{\frac{1}{3}} $$ 
	
    $\Large \text{Fazendo uma mudança de variável:}$  
	
    $$\Large y=\left(\xi\right)^{-\frac{1}{3}}; \quad \xi=x^2+1$$ 
	
    $$\Large \frac{\dy}{\dx}= \frac{\dy}{\mbox{d}\xi} \cdot \frac{\mbox{d}\xi}{\dx}$$ 
  
    $$ = \frac{1}{3} (\xi)^{-\frac{2}{3}}\cdot (2x) $$ 
	
    $$\Large \frac{\dy}{\dx}=\frac{2x}{3\sqrt[3]{(x^2+1)^2}}$$ 



### Exemplo 

Diferencie $y=2^{(x^2+1)}$. 

??? check "Solução"
  
    $\Large \text{Fazendo uma mudança de variável, temos}$ 
	
    $$\Large y=2^{u}; \quad u=x^2+1$$ 
	
    $$\Large \frac{\dy}{\dx}=\frac{\dy}{\du}\cdot \frac{\du}{\dx}$$ 
    
    $$\Large = 2^{u}\ln{(2)}\cdot (2x)$$ 
	
    $$\Large \frac{\dy}{\dx}= 2^{(x^2+1)}\ln{(2)}(2x)$$ 


### Exemplo 

Diferencie $y=\sen(\cos(x))$.


??? check "Solução"
  
    $\Large \text{Fazendo uma mudança de variável, temos}$ 
	
    $$\Large y=\sen(\xi); \quad \xi = \cos(x)$$ 
	
    $$\Large \frac{\dy}{\dx}=\frac{\dy}{\mbox{d}\xi}\cdot \frac{\mbox{d}\xi}{\dx}= \cos(\xi)(-\sen(x))$$ 
	
    $$\Large \frac{\dy}{\dx}=-\cos(\cos(x))\sen(x) $$ 


### Exemplo 

Diferencie $y=\mbox{cossec}(\sqrt{x})\cdot \mbox{cotg}(2x)$. 



??? check "Solução"
  
    $\Large \text{Temos o produto de duas funções compostas, assim chamando}$ $\Large u=\sqrt{x}$ $\Large\text{e}$ $\Large v=2x$. 
	
    $$\Large \frac{\du}{\dx}=\frac{1}{2}x^{-\frac{1}{2}}$$ 
    
    $$\Large = \frac{1}{2\sqrt{x}}\quad \mbox{e} \quad \frac{\dv}{\dx}=2$$

    $\Large \text{Daí, temos}$ 

    $$\Large y=\mbox{cossec}(u)\cdot \mbox{cotg}(v)$$ 

    $\Large \text{Usando a regra do produto e a regra da cadeia, temos:}$  
	
    $$\Large \frac{\dy}{\dx}=\left[\mbox{cossec}(u)\right]'\cdot \mbox{cotg}(v)+\mbox{cossec}(u)\cdot \left[\mbox{cotg}(v)\right]'$$ 
	
    $$\Large = -\mbox{cossec}(u)\cdot \mbox{cotg}(u)u'\cdot \mbox{cotg}(v)+\mbox{cossec}(u)\left[-2\mbox{cossec}^2(v)\right]\cdot v'$$ 

    $\Large \text{Substituindo}$ $\Large u'$ e $\Large v'$ $\Large \text{e retornando para a variável}$ $\Large x$, $\Large \text{temos}$  
	
    $$\Large \frac{\dy}{\dx}=-\frac{ \mbox{cossec}(\sqrt{x})\cdot \mbox{cotg}(\sqrt{x})\mbox{cotg}(2x)}{2\sqrt{x}}-2\mbox{cossec}(\sqrt{x})\mbox{cossec}^2(2x)$$ 


### Exemplo 

Diferencie $y=e^{\sen(x)} \cdot \cos(\tg(x))$. 
	

??? check "Solução"
  
    $\Large \text{Temos um produto de funções, logo aplicamos a regra do produto,}$ 
	
    $$\frac{\dy}{\dx}= (e^{\sen(x)})'\cdot [\cos(\tg(x))]+(e^{\sen(x)})\cdot [\cos(\tg(x))]'$$ 
	
    $\Large \text{Veja que temos nas derivadas funções compostas, portanto, devemos aplicar a regra da cadeia. Calculando separadamente.}$ 
	
    $\Large \text{Seja}$ $y_1=e^{\sen(x)}$. $\Large \text{Fazendo uma mudança de variável,}$ $y_1=e^{u}; \quad u=\sen(x)$ 
	
    $$\Large \frac{\dy_1}{\dx} = \frac{\dy_1}{\du} \cdot \frac{\du}{\dx}= e^{u}\cdot \cos(x)$$ 
	
    $$\Large \frac{\dy}{\dx}= e^{\sen(x)}\cos(x)$$ 
	
    $\Large \text{Agora calculando a derivada de}$  $y_2=\cos(\tg(x))$. $\Large \text{Fazendo uma mudança de variável,}$ $y_2=\cos(\varphi); \quad \varphi=\tg(x)$ 
	
    $$\Large \frac{\dy_2}{\dx}=\frac{\dy_2}{\mbox{d}\varphi}\cdot \frac{\mbox{d}\varphi}{\dx} = -\sen(\varphi)\cdot \sec^2(x)$$ 
	
    $$\Large \frac{\dy_2}{\dx}= -\sen(\tg(x))\sec^{2}(x)$$

    $\Large \text{Portanto, temos}$ 
	
    $$\Large \frac{\dy}{\dx} =(e^{\sen(x)}\cos(x))[\cos(\tg(x))]+(e^{\sen(x)})[-\sen(\tg(x))\sec^{2}(x)] $$ 
	
    $\Large \text{Veja que para simplificar, basta colocar}$ $e^{\sen(x)}$ $\Large \text{em evidência, logo}$  
	
    $$\Large \frac{\dy}{\dx} =e^{\sen(x)} \cdot \{\cos(x)[\cos(\tg(x))]-[\sen(\tg(x))\sec^{2}(x)]\}$$


## Derivada de Uma Função Exponencial Composta 


Seja $y=u^{v},$ onde $u=u(x)$ e $v=v(x)$ são funções de $x$, deriváveis em um intervalo $I$, com $u(x)>0, \forall x \in I$. Então,

$$y'=v\cdot u^{v-1}\cdot u+u^{v}\cdot v'\cdot \ln{(u)}$$ 


**Demonstração:**

Temos que $y=u^{v}$, usando as propriedades de logaritmo, escrevemos 
	
$$y=e^{v\cdot \ln{(u)}}$$ 

Chamando $w=v\cdot \ln{(u)}$, segue que $y=e^{w}$.  

Pela regra da cadeia, temos: 

$$\frac{\dy}{\dx}=\frac{\dy}{\mbox{d}w}\cdot \frac{\mbox{d}w}{\dx}= e^{w}\cdot \left[v'\cdot \ln{(u)}+v\frac{1}{u}u'\right]$$ 

$$= u^{v}\left[v'\cdot \ln{(u)}+v\cdot u^{-1}\cdot v'\right]$$ 

$$= v\cdot u^{v-1}\cdot u'+u^{v}\cdot v'\ln{(u)}$$


### Exemplo 

Diferencie $y=(2x^2+1)^{\frac{x^3}{3}+1}$. 



??? check "Solução"
  
    $\Large \text{Chamando}$ $\Large u=2x^2+1$ $\Large \text{e}$ $\Large v=\frac{x^3}{3}+1$, 
	
    $\Large\text{Temos}$ $\Large y=u^{v}$. $\Large \text{Assim,}$  
	
    $$\Large y'=v\cdot u^{v-1}\cdot u'+u^{v}\cdot v'\ln{(u)}$$ 
	
    $$\Large = \left(\frac{x^3}{3}+1\right)\left(2x^2+1\right)^{\frac{x^3}{3}}\cdot (4x)+\left(2x^2+1\right)^{\frac{x^3}{3}+1}\cdot x^2\cdot \ln{(2x^2+1)}$$ 


## Derivada da Função Inversa 

**Teorema:** 
(Teorema de Funções Inversas). Seja $y=f(x)$ uma função definida em um intervalo aberto $]a,b[$. Suponho que $f$ admita, uma função inversa $x=g(y)$ contínua. Se $f'(x)$ existe e $f'(x)\neq 0 \forall x \in ]a,b[,$ então $g=f^{-1}$ é derivável 
	
$$g'(y)= \frac{1}{f'(x)} = \frac{1}{f'(g(y))} $$ 



### Exemplo 

Determinar a inversa de $y=2x-3$.  

??? check "Solução"
  
    $\Large \text{Temos}$ 


    $$x=g(y)= \frac{y+3}{2}$$

    $\Large \text{Temos ainda}$ $\Large f(x)=2$ $\Large \text{e}$  

    $$\Large g'(y)=\frac{1}{2}$$ 

    $\Large \text{Portanto,}$ 

    $$\Large g'(x)=\frac{1}{f'(x)}$$ 

### Exemplo 

Seja $f(2, +\infty) \rightarrow (-2, + \infty)$, definida por $f(x)= x^2-4x-2$. Determinar $(f^{-1})(3)$.  


??? check "Solução"
  
    $\Large \text{Temos}$ 

    $$\Large f'(x)= 2x-4 \neq 0, \forall x \in (2, +\infty)$$ 

    $\Large \text{Para}$ $\Large y=3$, $\Large \text{segue que}$ 
	
    $$\Large x^2-4x-2= 3 \Leftrightarrow x^2-4x-5=0 $$ 
	
    $\Large \text{Que tem como raízes,}$ 

    $$\Large x_1=5 ~\mbox{e}~ x_2=-1$$ 
	
    $\Large \text{Como só a raiz}$ $\Large x_1$ $\Large\text{está dentro do intervalo aberto, temos pelo teorema da função inversa,}$ 

    $$\Large \left(f^{-1}\right)(y)= \frac{1}{f'(x)}= \frac{1}{2x-4}$$ 

    $\Large \text{Assim,}$ $\Large\left(f^{-1}\right)(3)= \frac{1}{f'(5)}= \frac{1}{10-4}=\frac{1}{6}$. 


## Derivada da Função Exponencial 

Seja $y=a^{x}, ~a\neq 0 , a>0$  

Temos que sua derivada é dada por: 

$$y'=a^x\ln{(a)}$$ 


### Exercícios 


1. Diferencie as seguintes funções: 

(a) $ y = 3^{\arcsin(x^3)} $

(b) $ y = e^{-3x} $ 

\(c) $ y = e^{4x+5} $ 

(d) $ y = a^{x^2} $ 

(e)  $ y= 7^{x^2 + 2x} $

(f)  $ y = e^{x}(1-x^2) $ 

(g) $ y = \frac{e^{x} -1}{ e^{x} + 1} $

(h) $ y = x^{1/x} $ 

(i)  $ y = x^{\pi}\pi^{x} $

(j) $ y = e^{^-7x}\tan(\sqrt{x}) $ 


??? check "Respostas"
  
    $\Large \text{Algumas respostas podem está simplificadas ao ponto que não conferem com as obtidas na sua solução. Se este for o caso, não preocupe-se, você só obteve uma resposta menos simplificada.}$ 

    (a)$ y' = \frac{3x^2\ln{(3)}3^{\arcsin(x^3)}}{\sqrt{1-x^{6}}}$

		(b)$ y'=-3e^{-3x} $

		\(c)$ y'= 4e^{4x+5} $

		(d)$y'=2xa^{x^{2}}\ln{(a)} $

		(e) $y'= 2\ln{(7)}(x+1)7^{x^2+2x}$

		(f)$ y' = e^{x}( 1-2x-x^{1}) $

		(g) $ y'= \frac{2e^{x}}{(e^{x} +1)^{2}} $

		(h) $ y' = x^{1/x}\frac{ 1-\ln{(x)}}{x^{2}} $

		(i)$ y'=\pi x^{\pi - 1} \pi^{x} + x^{\pi} \pi^{x}\ln{(\pi)} $

		(j) $ y' = \frac{ e^{-7x}\sec^{2}(\sqrt{x})}{2\sqrt{x}} - 7e^{-7x}\tan(\sqrt{x}) $ 



## Derivada da Função Logarítmica 

Se $f(x)=\log_{a}{(x)}$, então 

$$\frac{\mbox{d}f }{\dx} = \frac{1}{x\ln{(a)}} $$ 
\textbf{Demonstração:} Aplicando a derivada pela definição, temos 

$$f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{\log_{a}{(x+\Delta)}-\log_{a}{(x)}}{\Delta x} $$ 

$$f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{1}{\Delta x} \left[\log_{a}{\left(\frac{x+\Delta x}{x} \right)}\right]$$ 

$$f'(x)=\displaystyle\lim_{\Delta x\to 0} \frac{1}{\Delta x} \left[\log_{a}{\left(1+\frac{\Delta x}{x} \right)}\right]$$ 

Fazendo uma mudança de variável: $u=\frac{\Delta x}{x} \Rightarrow \Delta x=u\cdot x $. 

Quando $\Delta x\to 0 \Rightarrow u\to 0$. 

Reescrevendo, 
$$f'(x)=\displaystyle\lim_{u\to 0} \frac{1}{u\cdot x} \log_{a}{\left(1+u\right)}$$ 

$$f'(x)= \frac{1}{x}\cdot \displaystyle\lim_{u\to 0} \frac{1}{u}\cdot \log_{a}{\left(1+u\right))} $$ 

$$f'(x)=\frac{1}{x}\cdot \displaystyle\lim_{u\to 0} \log_{a}{\left[\left(1+u\right)^{\frac{1}{u}}\right]} $$ 
	
$$f'(x)=\frac{1}{x}\cdot \log_{a}{\left[\underbrace{\displaystyle\lim_{u\to 0} (1+u)^{\frac{1}{u}}}_{=e}\right]} $$ 

$$f'(x)=\frac{1}{x}\cdot \log_{a}{(e)} $$ 

$$f'(x)=\frac{1}{x}\cdot \frac{ \ln{(e)}}{\ln{(a)}} $$ 

$$f'(x)=\frac{1}{x\ln{(a)}}$$ 

**Comentário**: 

> Em particular, se $f(x)=\ln{(x)}$, então 
	$$f'(x)=\frac{1}{x}\cdot \frac{1}{\ln{(e)}} \Rightarrow f'(x)= \frac{1}{x}$$ 


### Exemplo 

Diferencie $y=2^{x}\ln{(x)}$.



??? check "Solução"
  
    $\Large \text{Aplicando a derivada do produto, temos}$ 
	
    $$\Large y'=2^{x}\ln{(2)}\ln{(x)}+ 2^{x}\frac{1}{x}$$ 
	
    $$\Large y'=2^{x}\left(\ln{(2)}\ln{(x)}+\frac{1}{x}\right)$$ 


### Exercícios 

1. Determine a derivada das seguintes funções compostas: 

(a) $y=\omega^3\cdot \log_{7}{(3-2\omega)}$ 

(b) $y=\ln{[\cos(\tg(x))]}$ 

\(c) $y=\log_{3}(x)\cdot \cos(x)$

??? check "Respostas"
  
    (a) $\Large y'=\omega^2\left[3\omega\log_{7}{(3-2\omega)}-\frac{2\omega}{(3-2\omega)\ln{(7)}}\right]$ 
	
    (b) $\Large \frac{\dy}{\dx}= \frac{-\sec^{2}(x)\sen(\tg(x))}{\cos(\tg(x))}$ 
	
    \(c)$\Large y'= $ 

2. Diferencie as seguintes funções: 

 	
(a) $ y = \ln{|ax + b|}$ 

(b) $ y = \log_{a}{(x^2 + 1)}$ 

\c) $ y = \ln{\left[ \frac{e^{x}}{1+e^{x}}\right]}$  	

(d) $ y = \ln{\left[\frac{1+x^2}{1-x^2}\right]}$ 	

(e) $ y = \ln{| x^2 + 2x|}$ 

(f) $ y = \log_{9}{[(3x^2 +2)^{5}]}$

(g) $ y = x\ln{(x)}$ 

(h) $ y = [\ln{(x)}]^{3}$ 

(i) $ y = \log_{4}{[\ln{(x)}]}$ 

(j) $ y = \ln{\left[\arctan(x^2)\right]}$

(l) $ y = \ln{\left[ \ln{(\sec(2x))}\right]}$


??? check "Respostas"
  
    $\Large \text{Algumas respostas podem está simplificadas ao ponto que não conferem com as obtidas na sua solução. Se este for o caso, não preocupe-se, você só obteve uma resposta menos simplificada.}

    (a) $y^{'}= \left( \frac{ a }{ ax + b}\right)$	

    (b) $y^{'} = \left[ \frac{ 2x }{ (x^2 + 1)\ln{(a)}}\right]$ 

    \(c) $y^{'} = \left( \frac{ 1}{ 1 + e^{x}}\right)$  

    (d)$y^{'} = \left( \frac{4x}{1-x^{4}}\right)$	

    (e) $y^{'} = \left(\frac{ 2x +1}{x^2 + x}\right)$

    (f) $y^{'} = \left(\frac{30x}{ (3x^2 + 2)\ln{(9)}}\right)$

    (g)  $y^{'} = 1+\ln{(x)}$

    (h) $y^{'} = \left(\frac{3[\ln{(x)}]^{2}}{x}\right)$ 

    (i) $y^{'} = \left(\frac{1}{ x\ln{(x)}2\ln{(2)}}\right)$

    (j) $y^{'} = \frac{ -2x}{(1+x^4)\arctan(x^2)}$

    (l) $y^{'} = \frac{ 2\tan(2x)}{\ln{\left[\sec(2x)\right]}}$ 



## Derivadas de Ordem Superiores 

Significa o cálculo de derivadas sucessivas até uma determinada ordem $n$.


### Exemplo 

Determinar a derivada de $f(x)=5x^2+4x^4$. 


??? check "Solução"
  
    $\Large \text{Cálculo de derivada bastante simples,}$ 

    $$f'(x)=10x+16x^3$$


### Exemplo 

Diferencie $g(x)=10x+16x^3$. 

??? check "Solução"
  
    $\Large \text{Outro cálculo de derivada bastante simples,}$ 
	
    $$\Large g'(x)=10+48x^2$$ 
    
    $\Large \text{Fazendo}$ $\Large h(x)=10+48x^2$ 
    
    $\Large \text{Derivando,}$ 
    
    $$\Large h'(x)=96x $$ 
    
    $\Large \text{Fazendo}$ $\Large \omega(x)=96x$ 
    
    $$\Large \omega'(x)= 0 $$ 
	
    $\Large \text{Assim, para}$ $\Large f^{(n)}(x)=0,$ $\Large \text{se}$ $\Large n\geqslant 5 $. $\Large \text{Ou seja, a partir da quinta derivada, a função derivada será sempre zero.}$  



A derivada $n-\mbox{ésima}$ de $f$ é denotada por $f^{(n)}$ e é obtida diferenciando a função $f$ $n$ vezes. 

Notação: $f^{(n)} (x)=\frac{ \mbox{d}^{n}y}{\dx^{n}} $.


### Exemplo 

Seja $f(x)=e^{3x}$. Determine a $n-\mbox{ésima}$ derivada de $f$. 


??? check "Solução"
  
    $\Large \text{Calculando as derivadas, temos}$ 
	
    $$f'(x)=3e^{3x}$$ 
	
    $$f''(x)=3\cdot 3 e^{3x}= 3^2e^{3x}$$ 
	
    $$f'''(x)=3^2\cdot 2 e^{3x} = 3^{3}e^{3x}$$ 
	
    $$f^{(4)}(x)= 3^{3}\cdot 3 e^{3x} = 3^{4}e^{3x} $$ 
	
    Assim, 
	
    $$f^{(n)}(x)= 3^{n}e^{3x}$



### Exemplo 

Determine $\frac{\mbox{d}^{6}y}{\mbox{d}x^{6}}$ sabendo que $y=4x^2+5x^{7}$.  

??? check "Solução"
  
    $\Large \text{Calculando as derivadas, temos}$ 
	
    $$y'=8x+35x^6$$ 
	
    $$y''=8+210x^5$$ 
	
    $$y'''=150x^4$$ 
	
    $$y^{(4)}=4200x^3 $$ 
	
    $$ y^{(5)}=12600x^2$$ 
	
    $$y^{(6)}=25200x$$ 


## Diferenciação Implícita 

### Função Implícita 

uponha que as variáveis $x$ e $y$ estejam relacionadas por uma equação do tipo 

$$\begin{equation}\label{eq.1} 
F(x,y)=0
\end{equation}$$

Se $y=f(x)$ é tal que $F(x,f(x))=0$, então $y=f(x)$ é uma função implícita, definida pela equação \eqref{eq.1}.


Por exemplo: 

$$x^2+y^2-a^2=0$$

onde obtemos $y_1=\sqrt{a^2-x^2}$ e $y_2=-\sqrt{a^2-x^2}$, são duas funções implícitas definida pela \eqref{eq.1}. Nem sempre é possível obter a forma explícita da função dada na forma implícita. 

Exemplos: 

$$y^2-y-x^2=0$$ 

$$y-x-\frac{1}{4}\sen(y)=0$$ 


### Método do Cálculo da Função Implícita 


Dada uma equação que define $y$ implicitamente como uma função derivável de $x$ , calcula-se $y^{'}$ do seguinte modo:

1. Deriva-se ambos os lados da equação em relação a $x$ , termo a termo. Ao fazê-lo, tenha em mente que $y$ é uma função de $ x $ e use a REGRA DA CADEIA, quando necessário, para derivar as expressões nas quais figure $y$ . 

2. O resultado será uma equação onde figue não somente $x$ e $y$ , mas também $y^{'}$ . Expresse $y^{'}$ em função de $x$ e $y$.


3.  Tal processo é chamado explicitar $y^{'}$ . Tal processo é chamado explicitar $y^{'}$.


### Exemplo 

Diferencie $x^2+y^2=25$. 

??? check "Solução"
  
    $\Large \text{Veja que temos uma função implícita, logo}$ 

    $$\Large \frac{\mbox{d}}{\dx} (x^2+y^2)= \frac{\mbox{d}}{\dx}(25)$$ 

    $$\Large 2x+2y\frac{\dy}{\dx}=0 $$ 

    $\Large\text{Isolando a derivada,}$ $\Large\frac{\dy}{\dx}$, $\Large \text{temos}$ 

    $$\Large \frac{\dy}{\dx}=-\frac{2x}{2y} $$ 

    $$\Large\frac{\dy}{\dx}= - \frac{x}{y}$$  

### Exemplo 

Determine a derivada de $y^3+5xy^2+5e^{x}=0$. 


??? check "Solução"
  
    $\Large \text{Diferenciando implicitamente, temos}$ 
	
    $$\Large 3y^2y'+ 5y^2+5x2yy'+5e^{x}=0 $$ 
	
    $\Large \text{Colocando}$ $\Large y'$ $\Large \text{em evidência, temos}$
	
    $$\Large y'\left[3y^2+10xy\right]=-5y^2-5e^{x}$$ 
	
    $$\Large y'=\frac{-5y^2-5e^{x}}{3y^2+10xy} $$ 

### Exercício 

Ache $\frac{\dy}{\dx}$, sabendo que $2y^3e^{y}+4x^2\ln{(y)}=\sen(y)+\cos(x)$. 

??? check "Resposta"
  
    $$Large \frac{\dy}{\dx}=\frac{-8x\ln{(y)}-\sen(x)}{6y^2e^{y}+2y^3e^{y}+4x^2y^{-1}-\cos(y)}$$


### Exemplo 

Seja $y=f(x), x\in \R$, a função dada implicitamente pela equação $y^3+y=x$. Determine a derivada e a equação da reta tangente ao gráfico no ponto $(10,f(10))$. 


??? check "Solução"
  
    $\Large \text{Calculando a derivada,}$ 
	
    $$\Large 3y^2\frac{\dy}{\dx}+\frac{\dy}{\dx}=1$$ 
	
    $$\Large\frac{\dy}{\dx}=\frac{1}{3y^2+1}$$ 
	
    $\Large\text{Sabendo que}$ $\Large y=f(x)$, $\Large\text{temos`}$ 
	
    $$\Large\frac{\dy}{\dx}= \frac{1}{3(f(x))^2+1} $$ 
	
    $\Large\text{Determinando a equação da reta tangente. Sabemos que}$ $\Large y-f(x_0)=f'(x_0)(x-x_0)$ $\Large\text{é a equação da reta tangente.}$ 

    $$\Large f'(10)=\frac{1}{3(f(10))^2+1}$$ 
	
    $\Large\text{Note que}$ $\Large f(x)$ $\Large\text{satisfaz}$ 
	
    $$\Large [f(x)]^3+f(x)=x$$ 
	
    $$\Large [f(10)]^3+f(x)=10$$ 
	
    $\Large \text{Temos que}$  
	
    $$\Large\begin{array}{ccc} 
    p \in \mbox{D}(10) \\ 
    q \in \mbox{D}(1) 
    \end{array}\Rightarrow 
    \frac{p}{q} \left\{ \pm 2, \pm 5 , \pm 10 \right\}$$ 

    $\Large\text{Como}$ $\Large f(10)=2$. $\Large\text{Assim,}$ 
	
    $$\Large f'(10)= \frac{1}{3\cdot 2^2+1} = \frac{1}{13}$$ 
    
    $\Large\text{Logo, a equação da reta tangente,}$  

    $$\Large y-f(10)=f'(10)(x-10)$$ 

    $$\Large y-2=\frac{1}{13}(x-10)$$ 

    $$\Large y=\frac{x}{13}-\frac{10}{13}+2$$ 

    $$\Large y=\frac{x+16}{13}$$ 


### Exemplo 

Diferencie a seguinte função $ \sin(x + y) = y^{2}\cos(x)$. 


??? check "Solução"
  
    $\Large \text{Derivando ambos os membros da igualdade,}$ 
    
    $$\Large\cos(x+y) + y^{'}\cos(x+y) = 2yy^{'}\cos(x) - y^{2}\sin(x)$$
	
    $\Large\text{Explicitando}$ $\Large y'$
    
    $$\Large y^{'}\cos(x+y) - 2yy^{'}\cos(x) =  - \cos(x+y) - y^{2}\sin(x)$$
    
    $$\Large\Rightarrow y^{'}[\cos(x+y) -  2y\cos(x)] =  -( \cos(x+y) + y^{2}\sin(x))$$
	
    $$\Large\Rightarrow y^{'} = \frac{( \cos(x+y) + y^{2}\sin(x))}{2y\cos(x)-\cos(x+y)}$$
	
    $\Large\text{O processo de derivar implicitamente pode ser usado somente se a função determinada pela forma implícita é derivável.}$ 



### Exemplo 

Diferencie a seguinte função $  x^2 + xy + x\sin(y) = y\sin(x) $. 


??? check "Solução"
  
    $\Large \text{Derivando ambos os lados da igualdade, temos}$ 

    $$\Large 2x + y + xy^{'} + \sin(y) + x\cos(y)y^{'} = y^{'}\sin(x) + y\cos(x)$$

    $\Large\text{Explicitando}$ $\Large y^{'}$ 

    $$\Large xy^{'} +  x\cos(y)y^{'}  - y^{'}\sin(x)  = y\cos(x) - 2x - y - \sin(y)$$ 


    $$\Large\Rightarrow   xy^{'} +  x\cos(y)y^{'}  - y^{'}\sin(x)  = y\cos(x) - 2x - y - \sin(y)$$

    $$\Large\Rightarrow y^{'}[x + x\cos(y) - \sin(x)] = y\cos(x) - 2x - y - \sin(y) \Rightarrow$$


    $$\Large y^{'} = \frac{y\cos(x) - 2x - y - \sin(y)}{x + x\cos(y) - \sin(x)}$$ 	


## Diferenciação Logarítmica 


Os cálculos de derivadas de funções complicadas envolvendo produto, quociente ou potências podem muitas vezes ser simplificadas tomando se os logaritmos. 


### Exemplo 

Diferencie $y=\frac{x^{\frac{3}{4}}\sqrt{x^2+1}}{(3x+2)^5}$.  

??? check "Solução"
  
    $\Large \text{Aplicando o logaritmo natural em ambos os membros de}$ $\Large y$, $\Large\text{temos}$ 
	
    $$\Large\ln{(y)}=\ln{\left[\frac{x^{\frac{3}{4}\sqrt{x^2+1}}}{(3x+2)^5}\right]}$$ 

    $\Large\text{Usando a propriedade do logaritmo do quociente, temos}$

    $$\Large\ln{(y)}=\ln{(x^{\frac{3}{4}}\cdot \sqrt{x^2+1})}-\ln{\left[(3x+2)^5\right]}$$ 
    	
    $$\Large\ln{(y)}= \ln{(x^{\frac{3}{4}})}+\ln{[(x^2+1)^{\frac{1}{2}}]}-5\ln{(3x+2)}$$ 
    
    $$\Large\ln{(y)}=\frac{3}{4}\ln{(x)}+\frac{1}{2}\ln{(x^2+1)}-5\ln{(3x+2)}$$ 
    
    $\Large\text{Derivando ambos os lados implicitamente,}$ 

    $$\Large y'\frac{1}{y}=\frac{3}{4}\frac{1}{x}+\frac{1}{2}\frac{2x}{x^2+1}-\frac{5\cdot 3}{3x+2}$$ 
    
    $$\Large y'=y\left(\frac{3}{4x}+\frac{x}{x^2+1}-\frac{15}{3x+2}\right)$$ 

    $$\Large y'=\left(\frac{x^{\frac{3}{4}}\sqrt{x^2+1}}{(3x+2)^5}\right)\left[\frac{3}{4x}+\frac{x}{x^2+1}-\frac{15}{3x+2}\right]$$ 


### Passos para Diferenciação Logarítmica 

+ Tome o logaritmo natural aos ambos os lados de uma equação $y=f(x)$ e usando as propriedades dos logarítmicos para simplificar. 

+ Diferencie implicitamente em relação a $x$ ou $y$. 

+  Resolva a equação resultante para $y'$. 

### Exemplo 

Diferencie a seguinte função $y=x^{x}$. 


??? check "Solução"
  
    $\Large \text{Aplicando o logaritmo natural,}$  
	
    $$\Large\ln{(y)}=\ln{(x^{x})}$$ 

    $\Large\ln{(y)}=x\ln{(x)}$$ 
	
    $$\Large y'\frac{1}{y}=\ln{(x)}+x\frac{1}{x}$$ 
	
    $$\Large y'=y\left(\ln{(x)}+1\right)$$ 
	
    $$\Large y'=x^{x}\left(\ln{(x)}+1\right)$$ 