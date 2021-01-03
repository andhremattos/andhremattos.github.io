
# **Conjuntos Numéricos**

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

input[type='checkbox'] { display: none; } .wrap-collabsible { margin: 1.2rem 0; } .lbl-toggle { display: block; font-weight: bold; font-family: monospace; font-size: 1.2rem; text-transform: uppercase; text-align: center; padding: 1rem; color: #DDD; background: #0069ff; cursor: pointer; border-radius: 7px; transition: all 0.25s ease-out; } .lbl-toggle:hover { color: #FFF; } .lbl-toggle::before { content: ' '; display: inline-block; border-top: 5px solid transparent; border-bottom: 5px solid transparent; border-left: 5px solid currentColor; vertical-align: middle; margin-right: .7rem; transform: translateY(-2px); transition: transform .2s ease-out; } .toggle:checked+.lbl-toggle::before { transform: rotate(90deg) translateX(-3px); } .collapsible-content { max-height: 0px; overflow: hidden; transition: max-height .25s ease-in-out; } .toggle:checked + .lbl-toggle + .collapsible-content { max-height: 350px; } .toggle:checked+.lbl-toggle { border-bottom-right-radius: 0; border-bottom-left-radius: 0; } .collapsible-content .content-inner { background: rgba(0, 105, 255, .2); border-bottom: 1px solid rgba(0, 105, 255, .45); border-bottom-left-radius: 7px; border-bottom-right-radius: 7px; padding: .5rem 1rem; } .collapsible-content p { margin-bottom: 0; }
</style>



## Conjunto dos Números Naturais 

Os registros históricos de números encontrados denotam que os símbolos eram utilizados para registar a quantidade de animais. 

O Conjunto dos números naturais é composto por: 

$$ \N = \{0, 1, 2, 3, 4, 5, ...\},$$ 

e ainda o conjunto dos números naturais sem o zero. 

$$ \N^{*} = \{1, 2, 3, 4, 5, ...\},$$ 

Ainda se discute dentro da matemática se o zero pertence ou não ao conjunto dos números naturais. 

Veja que as operações de adição ($+$) e multiplicação ($\times$) estão bem definidas neste conjunto, no entanto a subtração ($-$) e a divisão ($\div$) não estão. 


## Conjunto dos Números Inteiros

Neste conjuntos temos a inserção dos números negativos, sua forma é dada por: 

$$\Z = \{..., -5, -4, -3, -2, -1, 0, 1, 2, 3, 4, 5, ...\},$$ 

Observe que $\N \subset \Z$. E ainda que no conjunto dos números inteiros temos bem definidas as operçaões de soma ($+$) e subtração ($-$). 

## Conjunto dos Números Racionais 

O conjunto dos números racionais ($\Q$) é formado por todos os números que podem ser escrito em forma de fração, ou seja, o conjunto dos números que podem ser obtidos como resultado de alguma divisão, representamos o conjunto da seguinte forma: 

$$ \Q = \displaystyle\left\{ \dfrac{a}{b} | a, b \in \Z ~\text{e} ~ b \neq 0 \right\}$$ 




