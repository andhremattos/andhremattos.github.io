
# **Licença**

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


<center> <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img src="../imagens/CC.jpg" style="width:200px;height:70px"/></a></center>
<center> <p>Esta obra está sob licença <em>Creative Commons</em> CC BY-NC-SA 4.0: esta licença
permite que outros remixem, adaptem e criem a partir do seu trabalho para fins não
comerciais, desde que atribuam o devido crédito e que licenciem as novas criações
sob termos idênticos.</p>

<br> 



