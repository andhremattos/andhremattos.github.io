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



## Propriedades do Limite de uma Função
 
 
+  $\displaystyle\lim_{x\to a} k = k ; ~ k \in \mathbb{R}$ 

$$\displaystyle\lim_{x\to 5} -\pi^{7}= - \pi^{7}$$ 

+ $\displaystyle\lim_{x\to a} k \cdot f(x)= k\cdot \displaystyle\lim_{x\to a} f(x)$ 

$$\displaystyle\lim_{x\to \frac{\pi}{4}} -\sqrt{7}\cdot \text{cotg}(x) $$ 

$$ = -\sqrt{7}\cdot \displaystyle\lim_{x\to \frac{\pi}{4}} \text{cotg}(x)$$ 

+ $\displaystyle\lim_{x\to a} \left[f(x)\pm g(x)\right]=\displaystyle\lim_{x\to a} f(x) \pm \displaystyle\lim_{x\to a} g(x)$

$$\displaystyle\lim_{x\to -1} \left[ 2^{x}+x^{3}\right]$$ 
   
$$= \displaystyle\lim_{x\to -1} 2^{x} + \displaystyle\lim_{x\to -1} x^{3} $$ 

+  $\displaystyle\lim_{x\to a} \left[f(x)\cdot g(x)\right]= \displaystyle\lim_{x\to a} f(x)\cdot \displaystyle\lim_{x\to a} g(x)$ 

$$\displaystyle\lim_{x\to \frac{\pi}{6}} (x^2+1)\cdot \mbox{arctg}(x)$$ 

$$=\displaystyle\lim_{x\to \displaystyle\frac{\pi}{6}} (x^2+1)\cdot \displaystyle\lim_{x\to \frac{\pi}{6}} \mbox{arctg}(x)$$ 

+ $\displaystyle\lim_{x\to a} \displaystyle\frac{f(x)}{g(x)} = \displaystyle\frac{\displaystyle\lim_{x\to a}f(x)}{\displaystyle\lim_{x\to a} g(x)}; \displaystyle\lim_{x\to a} g(x) \neq 0$

$$\displaystyle\lim_{x\to 1} \displaystyle\frac{x^3+4x^2+1}{x^2+1}$$ 

$$=\displaystyle\frac{ \displaystyle\lim_{x\to 1} x^3+4x^2+1}{\displaystyle\lim_{x\to 1}x^2+1} =3$$ 

+ $\displaystyle\lim_{x\to a} \left[f(x)\right]^{n} = \left[\displaystyle\lim_{x\to a} f(x)\right]^{n},~n \in \mathbb{N}^{*}$ 

$$\displaystyle\lim_{x\to 2 } (x^3+1)^{10} = \left[\displaystyle\lim_{x\to 1}x^3+1\right]^{10} $$ 

+ $\displaystyle\lim_{x\to a } \sqrt[n]{f(x)} = \displaystyle\sqrt[n]{\displaystyle\lim_{x\to a}f(x)}$ 
 	
$$\displaystyle\lim_{x\to 5} \sqrt[3]{x^2+1} = \sqrt[3]{\displaystyle\lim_{x\to 5}(x^2+1)}$$ 
 

## Limite de uma Função Racional Inteira (Polinomial)


Seja $f(x)=a_0x^n+a_1x^{n-1}+\cdots + a_n$, então 
$\displaystyle\lim_{x\to b } f(x)$ 

$$= \displaystyle\lim_{x\to b} a_0x^n+a_1x^{n-1}+\cdots + a_n$$ 

$$= ab^n+a_1b^{n-1}+\cdots+a_n = f(b)$$


## Propriedades de limite

**Calcule**: 

$$\dlim_{x\to 1} 3x^2 + x - 1$$ 

??? check "Limite função racional"
    <p style="text-align: center;">
    <iframe width="720" height="345" src="https://www.youtube.com/embed/0IqJ7OK_7cg"></iframe>
    </p>


