
# **Teorema do Confronto**

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

Se $f(x) \leqslant g(x) \leqslant h(x)$ e 

$$  \dlim_{x\to a} h(x)=L=\dlim_{x\to a} f(x)$$ então 

$$\dlim_{x\to a} g(x)=L$$ 

## Exemplo 1 

 Mostre que $\dlim_{x\to 0} x^2\cdot \sen\left(\dfrac{1}{x}\right)=0$. 


??? check "Solução"
    
    $\Large\text{Sabemos que}$ 

    $$\Large |\sen(u)|\leqslant 1 \Leftrightarrow -1 \leqslant \sen(u) \leqslant 1$$ 
    
    $\Large\text{Logo, para}$ $\Large u=\dfrac{1}{x}$, $\Large\text{temos}$ 
    
    $$\Large -1\leqslant \sen\left(\dfrac{1}{x}\right) \leqslant 1 $$ 

    $\Large\text{Multiplicando ambos os membros por}$ $\Large x^2$, 

    $$\Large -x^2\leqslant x^2\cdot \sen\left(\dfrac{1}{x}\right)\leqslant x^2$$ 
    
    $\Large\text{Note que}$ $\Large\dlim_{x\to 0} -x^2=0$ $\Large\text{e}$ $\Large\dlim_{x\to 0} x^2=0$. 
    
    $\Large\text{Portanto, pelo Teorema do Confronto,}$  

    $$\Large\dlim_{x\to 0} x^2\cdot \sen\left(\dfrac{1}{x}\right)=0$$ 


## Exemplo 2 

Calcule o $\dlim_{x\to 0} x^4\cdot e^{\cos\left(\dfrac{1}{x}\right)}$. 

??? check "Solução"
    
    $\Large\text{Sabemos que}$ $\Large |\cos(u)|\leqslant 1 \Leftrightarrow -1 \leqslant \cos(u) \leqslant 1$. 
    
    $\Large\text{Para um}$ $\Large u=\dfrac{1}{x}$, $\Large\text{temos}$

    $$\Large -1\leqslant \cos\left(\dfrac{1}{x}\right)\leqslant 1$$ 

    $\Large\text{Aplicando a exponencial natural,}$

    $$\Large e^{-1}\leqslant e^{\cos\left(\dfrac{1}{x}\right)} \leqslant e^{1}$$ 

    $\Large\text{Multiplicando ambos os membros por}$ $\Large x^4$, 

    $$\Large x^4\cdot e^{-1}\leqslant x^4e^{\cos\left(\dfrac{1}{x}\right)} \leqslant e\cdot x^4$$ 

    $\Large\text{Note que}$

    $$\Large \dlim_{x\to 0} x^4\cdot e^{-1}=0$$ 

    $$\Large \dlim_{x\to 0} x^4\cdot e =0 $$ 

    $\Large\text{Portanto, pelo Teorema do Confronto,}$  

    $$\Large\dlim_{x\to 0} x^4\cdot e^{\cos\left(\frac{1}{x}\right)}=0$$ 