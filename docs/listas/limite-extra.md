
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


## Lista Extra - Cálculo Diferencial e Integral I 

### **Questão 1 -** Prove cada proposição usando a definição de limite.

??? question "Questão"
    (a) $\huge\dlim_{x \to 2} 3x-2=4$

    (b) $\huge\dlim_{x \to 4} 5-2x=-3$

    \(c) $\huge\dlim_{x \to 2} x^2-4x+5=1$

    (d) $\huge\dlim_{x \to 1} \dfrac{x^2-1}{x-1} = 2$

    (e) $\huge\dlim_{x \to 5} \dfrac{1}{2-x} = -\dfrac{1}{3}$

    (f) $\huge\dlim_{x \to 9^-} \sqrt[4]{9-x}=0$.

??? check "Respostas"
    Questões de demostrações.

### **Questão 2 -** Determine, se possível, as constantes reais $a$ e/ou $b$ de modo que $\dlim_{x\to k} f(x)$ exista, sendo:

??? question "Questão"
    (a) $\huge f(x) = \left\{\begin{array}{rl} 3ax^2+2 ,& x<1 \\ x-2 ,& x \geq 1 \end{array} \right.$, $\huge k=1$

    (b) $\huge f(x) = \left\{\begin{array}{rl} 3x-2 ,& x>-1 \\ 3 ,& x=-1\\ 5-ax ,&x<-1 \end{array} \right.$, $\huge k=-1$

    \(c) $\huge f(x) = \left\{\begin{array}{rl} 4x+3 ,& x\leq-2 \\ 3x+a ,& x>-2 \end{array} \right.$, $\huge k=-2$

    (d) $\huge f(x) = \left\{\begin{array}{rl} \dfrac{3x^2-5x-2}{x-2} ,& x<2 \\ 3-ax-x^2 ,& x\geq2 \end{array} \right.$, $\huge k=2$

??? check "Respostas"
    (a) $4$;

### **Questão 3 -** Calcule os limites a seguir, justificando cada passagem através das suas propriedades.


(a) $\dlim_{x \to 4} 5x^2-2x+3$

(b) $\dlim_{x \to 3} (x^3+2)(x^2-5x)$

\(c) $\dlim_{x \to -1} \dfrac{x-2}{x^2+4x-3}$

(d) $\dlim_{x \to 1} \left(\dfrac{x^4+x^2-6}{x^4+2x+3}\right)^2$

(e) $\dlim_{u \to -2} \sqrt{u^4+3u+6}$

(f) $\dlim_{t \to -2} (t+1)^9(t^2-1)$

??? check "Respostas"
    (a) $4$;

## Limites e Indeterminações 

### **Questão 4 -** Prove que o $\dlim_{x \to 0}\dfrac{|x|}{x}$ não existe.

### **Questão 5 -** Seja 
$f(x)= \left\{\begin{array}{rcl}
\sqrt{x-4} &,& \mbox{ se } x>4 \\
8-2x &,& \mbox{ se } x \leq 4\end{array}\right.$ 

e determine, se possível, o $\dlim_{x \to 4} f(x)$.

??? check "Respostas"
    (a) $4$;

### **Questão 6 -** Verifique se existe os limites indicados, se não existir indique a razão disto.

(a) $\dlim_{t \to -4} \dfrac{|t+4|}{t+4}$

(b) $f(x) =
\left\{\begin{array}{rl}
\sqrt{x^2-9},&  \mbox{ se } x \leq -3; \\
\sqrt{9-x^2},&  \mbox{ se } -3 < x < 3; \\
\sqrt{x^2+6x+9},&  \mbox{ se } x \geq 3.
\end{array}\right.$


$\dlim_{x \to -3} f(x)$ e $\dlim_{x \to 3} f(x)$.

??? check "Respostas"
    (a) $\nexists$;

    (b) $\dlim_{x\to -3} f(x)=0$ e $\nexists\dlim_{x\to 3}$.

### **Questão 7 -** Calcule, se possível, os limites.

(a) $\dlim_{x\to-2} \dfrac{4-x^2}{2+x}$

(b) $\dlim_{x \to -3}\dfrac{x^2-x-12}{x+3}$

\(c) $\dlim_{x\to 1} \dfrac{x^2+2x-3}{3x-3}$

(d) $\dlim_{x \to -2}\dfrac{x+2}{x^2-x-6}$

(e) $\dlim_{x \to 3}\dfrac{x^2+x-12}{x^2-x-6}$

(f) $\dlim_{x\to 3} \dfrac{x^2-4x+3}{x^2-x-6}$

(g) $\dlim_{x \to 4} \dfrac{3x^2-17x+20}{4x^2-25x+36}$

(h) $\dlim_{x\to 1} \left(\dfrac{2x^2-3x+1}{3x-3}\right)^2$

(i) $\dlim_{x \to 1} \dfrac{x^3-1}{x^2-1}$

(j) $\dlim_{x\to 1} \dfrac{x^3-1}{5x-5}$

(k) $\dlim_{x \to -2} \dfrac{x^3+8}{x^2-4}$

(l) $\dlim_{t \to -2} \dfrac{t^3+4t^2+4t}{(t+2)(t+3)}$

(m) $\dlim_{x\to -2} \sqrt[3]{\dfrac{x^3-3x+2}{x^2+3x+2}}$

(n) $\dlim_{x\to 2} \dfrac{x^4-16}{8-x^3}$

(o) $\dlim_{x\to 1} \dfrac{x^3-3x+2}{x^4-4x+3}$;

??? check "Respostas"
    (a) $4$;

    (b) $-7$;

    \(c) $\frac{4}{3}$;

    (d) $-\frac{1}{5}$;

    (e) $\frac{7}{5}$;

    (f) $\frac{2}{5}$;

    (g) $1$;

    (h) $\frac{1}{9}$;

    (i) $\frac{3}{2}$;

    (j) $\frac{3}{5}$;

    (k) $-3$;

    (l) $0$;

    (m) $\sqrt[3]{-9}$;

    (n) $\frac{8}{3}$;

    (o) $\frac{1}{2}$;

### **Questão 8 -** Calcule, se possível, os limites.

(a) $\dlim_{x \to 1} \dfrac{\sqrt{x}-1}{x-1}$

(b) $\dlim_{x \to 0} \dfrac{\sqrt{x+1}-\sqrt{1-x}}{3x}$

\(c) $\dlim_{x \to -1} \dfrac{1-x^2}{x+\sqrt{2+x}}$

(d) $\dlim_{x \to 1} \dfrac{\sqrt{x+2}-\sqrt{3}}{x^3-1}$

(e) $\dlim_{t \to 9} \dfrac{9-t}{3-\sqrt{t}}$

(f) $\dlim_{t \to 0} \dfrac{\sqrt{2-t}-\sqrt{2}}{t}$

(g) $\dlim_{t \to 0} \dfrac{\sqrt{25-3t}-5}{t}$

(h) $\dlim_{x \to 7} \dfrac{2-\sqrt{x-3}}{x^2-49}$

(i) $\dlim_{x\to 4} \dfrac{3-\sqrt{5+x}}{1-\sqrt{5-x}}$

(j) $\dlim_{h \to 0} \dfrac{\sqrt[3]{8+h}-2}{h}$

(k) $\dlim_{x\to 0} \dfrac{\sqrt[3]{2x-1}+1}{x}$

(l) $\dlim_{x\to 1} \dfrac{\sqrt[3]{2x+1}-\sqrt[3]{3}}{1-\sqrt[3]{x}}$

??? check "Respostas"
    (a) $\frac{1}{2}$;

    (b) $\frac{1}{3}$;

    \(c) $\frac{4}{3}$;

    (d) $\frac{1}{6\sqrt{3}}$;

    (e) $6$;

    (f) $-\frac{\sqrt{2}}{4}$;

    (g) $-\frac{3}{10}$;

    (h) $\frac{-1}{56}$;

    (i) $-\frac{1}{3}$;

    (j) $\frac{1}{12}$;

    (k) $\nexists$;

    (l) $-\frac{2}{\sqrt[3]{9}}$.

### **Questão 8 -** Determine cada limite, através do gráfico da função $f(x)$, caso exista.

<center>
  <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/grafico_11.png" style="width: 50%; height: auto;"/>
  </small>
</center>

(a) $\dlim_{x\to 1^-} f(x)$

(b) $\dlim_{x\to 1^+} f(x)$

\(c) $\dlim_{x\to 1} f(x)$

(d) $\dlim_{x\to -\infty}f(x)$

(e) $\dlim_{x\to +\infty}f(x)$

(f) $\dlim_{x\to 2} f(x).$

??? check "Respostas"
    (a) $1$;

    (b) $1$;

    (c) $1$;

    (d) $-\infty$;

    (e) $\infty$;

    (f) $0$.

### **Questão 9 -** Determine cada limite, através do gráfico da função $f(x)$, caso exista.

<center>
  <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/grafico_12.png" style="width: 50%; height: auto;"/>
  </small>
</center>

(a) $\dlim_{x\to 3^-} f(x)$

(b) $\dlim_{x\to 3^+} f(x)$

\(c) $\dlim_{x\to 3} f(x)$

(d) $\dlim_{x\to -\infty}f(x)$

(e) $\dlim_{x\to +\infty}f(x)$

(f) $\dlim_{x\to 4} f(x).$

??? check "Respostas"
    (a) $-1$;
    (b) $3$;
    \(c) $\nexists$;
    (d) $-1$;
    (e) $3$;
    (f) $3$.

### **Questão 10 -** Determine cada limite, através do gráfico da função $f(x)$, caso exista.

<center>
  <p><small> Gráfico de f(x). </small></p><br>
    <img src="../imagens/grafico_13.png" style="width: 50%; height: auto;"/>
  </small>
</center>

(a) $\dlim_{x\to 1^-} f(x)$

(b) $\dlim_{x\to 1^+} f(x)$

\(c) $\dlim_{x\to 1} f(x)$

(d) $\dlim_{x\to -\infty}f(x)$

(e) $\dlim_{x\to +\infty}f(x)$

(f) $\dlim_{x\to 0} f(x).$

??? check "Respostas"
    (a) $\frac{1}{2}$;

    (b) $+\infty$;

    (c) $\nexists$;

    (d) $-\infty$;

    (e) $\frac{1}{2}$;

    (f) $-\frac{1}{2}$.

### **Questão 11 -** Mostre que o $\dlim_{x \to 0} x^2 \cdot \cos(20 \pi x) = 0$.

### **Questão 12 -** Use o teorema do confronto para mostrar que
$$\dlim_{x \to 0} \sqrt{x^2+ x^3} \sin \left(\dfrac{\pi}{x}\right) = 0$$


### **Questão 13 -** A função sinal, denotada por $\operatorname{sgn}$, está definida por
$$\operatorname{sgn} (x) = \left\{
\begin{array}{rcl}
-1 &,& \mbox{ se } x<0 \\
 0 &,& \mbox{ se } x=0 \\
 1 &,& \mbox{ se } x>0
\end{array}\right.$$

(a) Esboce o gráfico dessa função.

(b) Encontre ou explique por que não existe cada um dos limites que se seguem.

i. $\dlim_{x \to 0^+} \operatorname{sgn}(x)$

ii. $\dlim_{x \to 0^{-}} \operatorname{sgn}(x)$

iii. $\dlim_{x \to 0} \operatorname{sgn}(x)$

??? check "Respostas"
    (b) i. $1$; ii. $-1$; iii. $\nexists$.


### **Questão 14 -** Seja
$$h(x)= \left\{\begin{array}{rcl}
x &,& \mbox{ se } x < 0 \\
x^2 &,& \mbox{ se } 0 < x \leq 2 \\
8-x &,& \mbox{ se } x > 2
\end{array}\right.$$

(a) Calcule, se existirem, os limites.

 i. $\dlim_{x \to 0^+} h(x)$


 ii. $\dlim_{x \to 0^-} h(x)$


 iii. $\dlim_{x \to 0}h(x)$


 iv. $\dlim_{x \to 2^{-}} h(x)$


 v. $\dlim_{x \to 2^{+}} h(x)$


 vi. $\dlim_{x \to 2} h(x)$


(b) Esboce o gráfico da função $h$.

??? check "Respostas"
    (a) i. $0$; ii. $0$; iii. $0$; iv. $4$; v. $6$; vi. $\nexists$.


### **Questão 15 -** Considere a função $f(x)=\dfrac{x^2-1}{|x-1|}$.

(a) Determine $\dlim_{x \to 1^+} f(x)$ e $\dlim_{x \to 1^{-}}f(x)$.

(b) Existe $\dlim_{x \to 1}f(x)$?

\(c) Esboce o gráfico de $f$.

??? check "Respostas"
    (a) $2$ e $-2$.

### **Questão 15 -** Calcule o limite: $\dlim_{x \to 0} \dfrac{\cos(x) - \sqrt[3]{\cos(x)}}{\sin^2(x)}$.

??? check "Resposta"
    $\huge -\frac{1}{3}.$

### **Questão 15 -** Esboce o gráfico da função a seguir e use-o para determinar os valores de $a$ para quais os $\dlim_{x \to a} f(x)$ existe:

$$g(x) = \left\{\begin{array}{rcl}
x  &,& \mbox{ se } x\leq 1\\
3  &,& \mbox{ se } x=1\\
2-x^2 &,& \mbox{ se } 1< x\leq 2\\
x-3 &,& \mbox{ se } x>2\\
\end{array}\right.$$

