
# **Listas de Exercícios - Limite**

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

input[type='checkbox'] { display: none; } .wrap-collabsible { margin: 1.2rem 0; } .lbl-toggle { display: block; font-weight: bold; font-family: monospace; font-size: 1.2rem; text-transform: uppercase; text-align: center; padding: 1rem; color: #DDD; background: #0069ff; cursor: pointer; border-radius: 7px; transition: all 0.25s ease-out; } .lbl-toggle:hover { color: #FFF; } .lbl-toggle::before { content: ' '; display: inline-block; border-top: 5px solid transparent; border-bottom: 5px solid transparent; border-left: 5px solid currentColor; vertical-align: middle; margin-right: .7rem; transform: translateY(-2px); transition: transform .2s ease-out; } .toggle:checked+.lbl-toggle::before { transform: rotate(90deg) translateX(-3px); } .collapsible-content { max-height: 0px; overflow: hidden; transition: max-height .25s ease-in-out; } .toggle:checked + .lbl-toggle + .collapsible-content { max-height: 350px; } .toggle:checked+.lbl-toggle { border-bottom-right-radius: 0; border-bottom-left-radius: 0; } .collapsible-content .content-inner { background: rgba(0, 105, 255, .2); border-bottom: 1px solid rgba(0, 105, 255, .45); border-bottom-left-radius: 7px; border-bottom-right-radius: 7px; padding: .5rem 1rem; } .collapsible-content p { margin-bottom: 0; }
</style>


## Definição de Limite  

### **Questão 1 -** Usando a definição de limite, prove que:

??? question "Questão"
    (a) $\huge\dlim_{x\to -1} \left(\dfrac{1}{x+5}\right)=\dfrac{1}{4}$. 

    (b) $\huge\dlim_{x\to -2} (x^3-3x+2)=0$.

    \(c) $\huge\dlim_{x\to 0} 2x^2+5x+6=6$.

    (d) $\huge\dlim_{x\to 4} 7-3x=5$.

    (e) $\huge\dlim_{x\to 2} \dfrac{ x^3-8}{x-2}=12$. 


??? check "Respostas"
    Questões de demostrações.


### **Questão 2 -** Seja $f$ definida em: 

$\R$ tal que $\forall x \in \R$, tem-se que $|f(x)-3|\leqslant 2|x-1|$. Calcule $\dlim_{x\to 1} f(x)$ e justifique sua resposta.

??? check "Resposta"
    Em breve.


## Limites indeterminados 

### **Questão 3 -** Usando as propriedades de limites e/ou alguns artifícios algébricos, se necessário, calcule os seguintes limites: 


??? question "Questão"
    
    (a) $\Large\dlim_{x\to 2} \dfrac{ \sqrt[3]{2x+1}-\sqrt[3]{5}}{x-2}$ 
    
    (b) $\Large\dlim_{x\to 1} \left[\dfrac{1}{x-1}+\dfrac{1}{x^2-3x+2}\right]$
    
    \(c) $\Large\dlim_{x\to -2} \dfrac{x^3-2x+4}{x^2+5x+6}$ 
    
    (d) $\Large\dlim_{x\to -1} \dfrac{\sqrt[3]{x+2}-1}{x+1}$ 
    
    (e) $\Large\dlim_{x\to 0} \dfrac{ \sqrt[3]{a+x}-\sqrt[3]{a}}{x} ~ a>0$ 
    
    (f) $\Large\dlim_{x\to 2} e^{\mbox{arctg}\left(\dfrac{3x^2-12}{6x^2-12x}\right)}$ 
    
    (g) $\Large\dlim_{x\to 0} \dfrac{1}{x\sqrt{1+x}}-\dfrac{1}{x}$ 
    
    (h) $\Large\dlim_{x\to 1} \dfrac{ \sqrt[3]{x+7}-2}{x-1}$ 
    
    (i) $\Large\dlim_{x\to 2} \mbox{arctg} \left(\dfrac{x^2-4}{3x^2-6x}\right)$

## Limites no infinito 

### **Questão 4 -** Determine os seguintes limites: 

??? question "Questão"

    (a) $\Large\dlim_{x\to -\infty} \dfrac{2x+1}{\sqrt{2x^2+1}}$

    (b) $\Large\dlim_{x\to -\infty} \dfrac{3-2x}{\sqrt{x^2-1}}$ 

    (c) $\Large\dlim_{x\to +\infty} \dfrac{ \sqrt{9x^2+2x}}{x+2}$ 

    (d) $\Large\dlim_{x\to +\infty} \sqrt{x^2+4x+1}-x$ 


### **Questão 5 -** Sabendo-se que 

$\dlim_{x\to +\infty} \dfrac{ ax^3+bx^2+cx+4}{\sqrt{4x^2+3}}=5$, determine o valor de $a, b$ e $c$. 


### **Questão 6 -** 

Determine se o que esta estabelecido é falsou ou verdadeiro. Se verdadeiro, explique por quê. Se falso, explique por quê ou dê um contra-exemplo do que está estabelecido.


??? question "Questão"

    (a) $\Large\dlim_{x\to +\infty} \dfrac{\sqrt{4x^2+2x}}{4x+5}=0.$ 

    (b) $\Large\text{O limite}$ $\Large\dlim_{x\to +\infty} \dfrac{3x^3+5x+2}{5x^2+x-9x^3}=-\dfrac{1}{3}$


### **Questão 7 -** 

A arrecadação mundial total pela exibição de um filme de grande sucesso de bilheteria é aproximado pela função $A(x)=\dfrac{120x^2}{x^2+4}$, em que $A(x)$ é medido em milhões de dólares e $x$ é o número de meses do filme em cartaz. Pergunta-se:  

??? question "Questão"

    $\Large\text{(a) Qual é a arrecadação de bilheteria após o primeiro e o segundo mês?}$
    
    $\Large\text{(b) Qual será a arrecadação do filme a longo prazo?}$ 


## Limites infinitos 

### **Questão 8 -** 

Determine se o que esta estabelecido é falsou ou verdadeiro. Se verdadeiro, explique por quê. Se falso, explique por quê ou dê um contra-exemplo do que está estabelecido.


??? question "Questão"

    (a) $\Large\dlim_{x\to \frac{\pi}{2}} ( 1+\tg^2(x))^{3\mbox{cotg}^2(x)}=+\infty$ 
    
    (b) $\Large\dlim_{x\to 5^{+}} \dfrac{6}{(x-5)^2}=+\infty$, $\Large\text{nesse caso, dizemos que a reta}$ $\Large x=1$ $\Large\text{é uma assíntota horizontal.}$ 


## Assíntotas 

### **Questão 9 -** Encontre as assíntotas horizontais e verticais da curva: 


??? question "Questão"

    (a) $\Large y=\dfrac{-x^2+2x}{x^2-1}$
    
    (b) $\Large y=\dfrac{x^3-x}{x^2-6x+5}$
    
    (c) $\Large y= - \dfrac{ 3x^2+1}{2x^2-7x}$. 


## Continuidade 

### **Questão 10 -** Sobre a função $f$, definida abaixo, sabe-se que ela é contínua em todos os pontos do seu domínio. Baseado nessa informação, determine o valor de $a+c$, sendo  

??? question "Questão"

    $$\Large f(x)=\left\{\begin{array}{cccc} 
    ax^2-10x+c, & \mbox{se} & x\geqslant 3 ~ \mbox{ou}~ x\leqslant \dfrac{1}{3} \\ 
    2, & \mbox{se} & \dfrac{1}{3}<x< 3 
    \end{array}\right.$$ 

### **Questão 11 -** 

Dada a função 

$$f(x)=\left\{\begin{array}{cccc} 
-2x, & \mbox{se} & x<0\\ 
3, & \mbox{se} & x=0\\ 
4x-x^2, & \mbox{se} & 0<x<2 \\ 
\log_{2}{(x)}, & \mbox{se} & x\geqslant 2 
\end{array}\right.$$ 

Pede-se: 

??? question "Questão"

    $\Large\text{(a) Determinar}$ $\Large\dlim_{x\to -\infty} f(x)$, $\Large\dlim_{x\to 0} f(x)$, $\Large\dlim_{x\to 2} f(x)$ e $\Large\dlim_{x\to +\infty} f(x)$

    $\Large\text{(b) Determinar, se existirem, os pontos onde}$ $\Large f$ $\Large\text{é descontínua (não contínua).}$ 

    $\Large\text{(c) Esboçar o gráfico de}$ $\Large f$


### **Questão 12 -** 

Dada a função $f:\R \rightarrow \R$, definida por 

$$f(x)=\left\{
\begin{array}{ccc}
2^{x+1}, & \mbox{se} & x<-1\\ 
2, & \mbox{se} & x=-1\\ 
\dfrac{x^2+x}{x+1}, & \mbox{se} & x>-1 
\end{array}\right.$$ 

Pede-se: 

??? question "Questão"

    $\Large\text{(a) Determine}$ $\Large\dlim_{x\to -\infty} f(x)$, $\Large\dlim_{x\to -1^{-}} f(x)$, $\Large\dlim_{x\to -1^{+}} f(x)$ e $\Large\dlim_{x\to +\infty} f(x)$. 

    $\Large\text{(b) Verifique se}$ $\Large f$ $\Large\text{é contínua no ponto}$ $\Large x_1=-1$. $\Large\text{E no ponto}$ $\Large x_2=0$. $\Large\text{Justifique.}$ 

    $\Large\text{(c) Esboçar o gráfico de}$ $\Large f$.


### **Questão 13 -** 

Determine se o que está estabelecido é falso ou verdadeiro. Se verdadeiro, explique por quê. Se falso, explique por quê ou dê um contra-exemplo do que está estabelecido. 


??? question "Questão"

    $\Large\text{(a) A função}$ $\Large f(x)=\dfrac{\sqrt[4]{x}-1}{x-1}$ $\Large\text{tem uma descontinuidade removível em} $\Large x=1$ $\Large\text{e}$ $\Large f$ $\Large\text{pode ser redefinida como uma nova função contínua em}$ $\Large 1$ $\Large\text{por:}$ 
    
    $\Large g(x)=\left\{\begin{array}{ccc}
    \dfrac{\sqrt[4]{x}-1}{x-1}, & \mbox{se} & x\neq 1 \\ 
    \dfrac{1}{4}, & \mbox{se} &  x=1
    \end{array}
    \right.$ 
    
    $\Large\text{(b)}$ $\Large \dlim_{x\to \frac{1}{2}^{-}} \dfrac{2x-1}{|2x^3-x^2|}=0$. 

    $\Large\text{(c)}$ $\Large\dlim_{x\to -1^{-}} \dfrac{4x^2+5x+1}{|x+1|}$ $\Large\text{não existe.}$ 
    
    $\Large\text{(d) A função}$ $\Large f(x)=\dfrac{\sqrt[3]{x^2-x-1}-\sqrt[3]{3x^2-4x-3}}{x^3-4x^2+8}$ $\Large\text{tem uma descontinuidade removível em}$ $\Large x=2$, $\Large\text{além disso podemos definir uma nova função dada por}$ 
        
    $\Large g(x)= \left\{
    \begin{array}{ccc}
    f(x), & \mbox{se} & x\neq 2 \\ 
    -6, & \mbox{se} & x=2 
    \end{array}\right.$ que é contínua em $2$. 

### **Questão 14 -** Considere a função definida por 

$$f(x)=\left\{
\begin{array}{ccc}
\mbox{arccos}\left(\dfrac{\cos^2(x)+1}{2\sqrt{2(x^2+1)}}\right),& \mbox{se} & x\leqslant 0 \\ 
\mbox{arcsen} \left(\dfrac{\sqrt{x+1}-1}{x}\right),& \mbox{se} & 0<x\leqslant 3 \\ 
\dfrac{x^2-9}{9x^3-243}, & \mbox{se} & x>3 
\end{array}\right.$$ 

??? question "Questão"

    $\Large\text{(a) Encontre os pontos nos quais}$ $\Large f$ $\Large\text{é descontínua. Em quais desses pontos}$ $\Large f$ $\Large\text{é contínua à direita, à esquerda ou em nenhum deles?}$

    $\Large\text{(b) Verifique se a reta}$ $\Large y=0$ $\Large\text{é uma assíntota horizontal.}$ 

    $\Large\text{(c) Esboce o gráfico de}$ $\Large g$. 
    $$\Large g(x)=\left\{
    \begin{array}{ccc}
    1+x^2, & \mbox{se} & x\leqslant 0 \\ 
    1+\sen(x), & \mbox{se} & 0< x \leqslant \dfrac{\pi}{2} \\ 
    x^2-1, & \mbox{se} & x> \dfrac{\pi}{2} 
    \end{array}\right. $$ 

## Teorema do Valor Intermediário 

### **Questão 15 -**

Determine se o que está estabelecido é falso ou verdadeiro. Se verdadeiro, explique por quê. Se falso, explique por quê ou dê um contra-exemplo do que está estabelecido. 

(a) A equação $x^3-\dfrac{1}{1+x^4}=0$ não admite nenhuma solução real.

(b) Não existe nenhum número real $c \in (0,1)$ tal que seja uma raiz da equação $\Large\displaystyle\sqrt[3]{x}=1-x$. 


### **Questão 16 -** 

A equação $x^6-2x^4-3x^2+2=0$ possui **pelo menos** duas raízes reais no intervalo aberto $(-1,1)$. Verdadeiro ou falso? Justifique sua resposta.

## Teorema do Confronto 


#### **Questão 17 -** 

Determine o valor do número real $\rho$, sabendo-se que $\rho=\dlim_{x\to 0} 10e^{x^2\cos\left(\frac{x^2+1}{x^2}\right)}$.

#### **Questão 18 -** 

Mostre que o $\dlim_{x\to 0}\sqrt{x^2+x^3}\cdot e^{\cos\left(\dfrac{\pi}{x}\right)}=0$. 


### **Questão 19 -** 

Sendo $f:\R \rightarrow \R$, dada por 

$$f(x)=\left\{
\begin{array}{ccc}
10x^3\sen\left(\dfrac{1}{x}\right), & \mbox{se} & x\neq 0 \\ 
10, & \mbox{se} & x=0 
\end{array}\right.$$ 

Calcule $\dlim_{x\to 0} \dfrac{f(x)}{x}$. 

## Limites Fundamentais 

### **Questão 20 -** Determine os seguintes limites fundamentais trigonométricos:

(a) $\dlim_{x\to 0} \dfrac{ \sen(\alpha x)+\sen(\beta x)}{\alpha \beta x}$ 

(b) $\dlim_{x\to 0} \dfrac{ \sec(x)-1}{x^2\sqrt{x+1}}$ 	

\(c) $\dlim_{x\to \frac{\pi}{6}} \dfrac{ \sen\left(x-\dfrac{\pi}{6}\right)}{\mbox{cotg}^3(x)-3\mbox{cotg}(x)}$

### **Questão 21 -** Determine os seguintes limites fundamentais logarítmicos: 

(a) $\dlim_{\omega \to 0} \dfrac{e^{10\omega}-1}{\sen(\omega)}$ 

(b) $\dlim_{x\to 0} \dfrac{ e^{4x}+4\sen(4x)-1}{2x}$ 

\(c) $\dlim_{x\to 0} \dfrac{ e^{-ax}-e^{-bx}}{\sen(ax)-\sen(bx)}$ 

### **Questão 22 -**

Mostre que $\dlim_{x\to +\infty} e^{x(2^{\frac{1}{x}}-1)}=2$.


### **Questão 23 -**

Determine os seguintes limites fundamentais exponenciais: 

??? question "Questão"
    
    $\Large\text{(a)}$ $\Large\dlim_{x \to 0} \left(\dfrac{x-1}{x+1}\right)^{x}$ 

    $\Large\text{(b)}$ $\Large\dlim_{x\to -\infty} \left(\dfrac{x+2}{x}\right)^{2-x}$ 

    $\Large\text{(c)}$ $\Large\dlim_{x\to +\infty} (x+1)\left[\ln{(2x+3)}-\ln{(2x+1)}\right]$ 

    $\Large\text{(d)}$ $\Large\dlim_{x\to +\infty} \left(1+\dfrac{1}{x}\right)^{x+10}$ 

    $\Large\text{(e)}$ $\Large\dlim_{x\to 0} \left(\dfrac{ \sen(x)}{x}\right)^{\dfrac{ \sen(x)}{x-\sen(x)}}$ 

    $\Large\text{(f)}$ $\Large\dlim_{x\to 0} \dfrac{\ln{(\cos(x))}}{x^2}$ 

    $\Large\text{(g)}$ $\Large\dlim_{x\to \frac{\pi}{2}} \dfrac{ \ln{(\sen(x))}}{(\pi-2x)^2}$ 

??? check "Respostas"
    Em breve.

### **Questão 24 -**

Sabemos que se uma quantia $A_0$ é investida a uma taxa $r$ de juros compostos, capitalizados $m$ vezes ao ano, o saldo $A(t)$, após $t$ anos é dado por $A(t)=A_0\left(1+\dfrac{r}{m}\right)^{mt}$. Se os juros forem capitalizados continuamente. O saldo deverá ser?