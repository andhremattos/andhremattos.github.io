# **Listas de Exercícios - Derivada**

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



## Derivação Implícita 

1. Diferencie as funções implícitas: 

(a) $y=x\sin(y)$ 

(b) $e^{x}\cos(y) = xe^{y} $

(c) $x^{2} + x\arcsin(y) = ye^{x} $

(d) $3y-x^2+\ln{(xy)}=2$ 

(e) $ x\ln{(y)}-y\ln{(x)} = 1 $

(f) $e^{xy}-x^{3}+3y^{2}=11$ 

??? check "Respostas"
  
    $\Large\text{(a)}$ $\Large y'=\frac{\sin(y)}{1-x\cos(y)}$

    $\Large\text{(b)}$  $\Large y' = \frac{ e^{x}\cos(y) - e^{y}}{ e^{x]\sin(y) + xe^{y}}}$

    $\Large\text{\(c)}$ $\Large y'= \frac{ \sqrt{1-y^{2}}(ye^{x} - \arcsin(y) - 2x)}{x-e^{x}\sqrt{1-y^{2}}}$ 

    $\Large\text{(d)}$ $\Large y'=\frac{ (2x^2 -1)y}{x(3y +1)}$

    $\Large\text{(e)}$ $\Large y'=\frac{y^2 -xy\ln{(y)}}{x^2-xy\ln{(x)}}$

    $\Large\text{(f)}$ $\Large y'=\frac{3x^2-ye^{xy}}{xe^{xy}+ 6y}$



2. Determine a equação da reta tangente ao gráfico das funções implícitas definidas por:


(a) $ x^3 + y^3 = 6xy $ , no ponto $ (3,3) $ (Folium de Descartes) 

(b) $ 2(x^2 + y^2)^{2} = 25(x^2 - y^2) $ no ponto $ ( 3,1) $ (Lemiscata de Bernoulli )

\(c) $ y^{2} = x^{2}(x+2). $  no ponto $ \left( -\frac{1}{2} , \frac{1}{2}\sqrt{\frac{3}{2}}\right)$ 

 

??? check "Respostas"
  
    $\Large\text{Algumas respostas podem está simplificadas o ponto que não conferem com as obtidas na sua solução. Se este for o caso, não preocupe-se, você só obteve uma resposta menos simplificada.}$ 
 
		$\Large\text{(a)}$ $\Large x +y= 6 $ 
		$\Large\text{(b)}$  $\Large 13y +9x -40 = 0 $
		$\Large\text{\(c)}$  $\Large 4\sqrt{6}y + 10x - 1 = 0 $


3. Determine a equação da reta tangente e a equação da reta normal ao gráfico da função implícita definida por:
$ (x^2 + y^2)(y^2 + x(x+1)) = 4xy^{2} $ no ponto $ \left( \frac{1}{2}, \frac{1}{2}\right) $.
	
 
??? check "Resposta"
  
    $\Large\text{Reta tangente:}$ $\Large 2y - 4x + 1 = 0.$ 
    
    $\Large\text{Reta normal:}$ $\Large 4y +2x - 3 = 0.$ 

