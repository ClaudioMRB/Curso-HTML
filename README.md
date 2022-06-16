# Curso-HTML



**Um pseudo-elemento CSS é uma palavra-chave adicionada a um seletor que permite que você estilize uma parte específica do elemento selecionado.**

https://developer.mozilla.org/pt-BR/docs/Web/CSS/Pseudo-elements

**Uma pseudoclasse CSS é uma palavra-chave adicionada a um seletor que especifica um estado especial do(s) elemento(s) selecionado(s).**

https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes



A [pseudo-classe CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes) **`:root`** se equipara à raíz de uma árvore, que por sua vez representa o documento. Aplicado ao HTML, `:root` representa o elemento [``](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/html) e é identico ao seletor html, exceto que sua [especificidade](https://developer.mozilla.org/pt-BR/docs/Web/CSS/Specificity) é mais alta.

https://developer.mozilla.org/pt-BR/docs/Web/CSS/:root

**CSS selectors**

https://www.w3schools.com/cssref/css_selectors.asp

**mudar cor do texto** ex: #styles.css --> h1 { color: red;}

------------------------------------------------------------------------------------------------

**mudar cor do paragráfo** #styles.css --> p { color: red;}

--------------------------------------------------------------------------------------------

**.class - seleciona todos os elementos com class = "intro"**

​							index.html		ex: <.h2 class="cor-laranja"> Categorias <./h2>

​							#styles.css 		ex: .cor-laranja { color: orange;}

**.class1 .class2 - seleciona todos os elementos com name1 e name2 definidos dentro de seu atributo de classe.**

index.html Ex: <.div class="card"> img <./div>

​							<.div class="card"> texto<./div>div>

**todo seletor que tiver um img dentro de um card.**

#styles.css Ex:  .card img { width: 200px; height: 200px}

------------------------------------------------------------------------------------------------------------------------------

**mudar a cor quando passa o mouse em cima.**

#styles.css Ex: .cor-laranja:hover { color: aqua;}

​					Ex2: .card h1:hover{ color: aqua;}

-------------------------------------------------------------------------------------------------------------------------

**mudar cor de fundo quando o seletor for um (id="")**

index.html Ex1: <.section id="titles">

#styles.css Ex2: #titles { background-color: cor;}

-------------------------------------------------------------------------------------------------------------------------------------

(*) **é um seletor que adiciona as modificações para todo o projeto.**

#styles.css Ex1:  * { font-size: 1-px}

**Colocar bordas, margem e padding.**

**Ex:**  .card img{ border: 1px solid "cor" padding: 10px margin: 20px}



margin-bottom (margem inferior)

margin-left (margem esquerda)

margin-right (margem direita)

margin-top (margem superior)

**ex:** margin-top: 20px;

----------------------------------------------------------------------------------------------------------------------------------------

**Flexbox**

https://www.alura.com.br/artigos/css-guia-do-flexbox?gclid=CjwKCAjwqauVBhBGEiwAXOepka2LMOkXEzJrjCAE8LkWJ51po-HDOmFTfkWT9l9jGS53RRP9he5m1hoCs3kQAvD_BwE



**Display flex só se aplica ao pai dos elementos**

**Exemplo:**

<.div class="containers-dos-blocos"> **elemento pai dos blocos **

​			<.div> **blocos filhos**

​			<./div>**fim dos bloco filhos**

<./div> **fim do elemento pai dos blocos **

**style.css** .containers-dos-blocos{ display: flex;}

.flex-container {    flex-wrap: nowrap | wrap | wrap-reverse;  }

.flex-container {    flex-flow: row nowrap | row wrap | column nowrap | column wrap;  }

.flex-container {    justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;  }
