## Container

Neste primeiro post veremos as propriedades que ficam no elemento pai dos nossos itens, o container. Teremos basicamente um container com três itens dentro.

Copiar

```html
<div class="container" >
	<div class="item" ></div>
	<div class="item" ></div>
	<div class="item" ></div>
</div>
```

# margin

## [Experimente](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#experimente)

A propriedade **`margin`** do [CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS) define a [área de margem](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model) nos quatro lados do elemento. É uma abreviação que define todas as margens individuais de uma só vez: [`margin-top`](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin-top), [`margin-right` (en-US)](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-right), [`margin-bottom`](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin-bottom), e [`margin-left` (en-US)](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-left).

<iframe class="interactive is-default-height" height="200" src="https://interactive-examples.mdn.mozilla.net/pages/css/margin.html" title="MDN Web Docs Interactive Example" loading="lazy" style="box-sizing: border-box; border: 1px solid var(--border-primary); max-width: 100%; width: 753.578px; background-color: var(--background-secondary); border-radius: var(--elem-radius); color: var(--text-primary); height: 375px; margin: 1rem 0px; padding: 0px;"></iframe>

## [Sintaxe](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#sintaxe)

```
/* Aplica para todos os quatro lados */
margin: 1em;

/* vertical | horizontal */
margin: 5% auto;

/* topo | horizontal | inferior */
margin: 1em auto 2em;

/* topo | direita | inferior | esquerda */
margin: 2px 1em 0 auto;

/* Valores globais */
margin: inherit;
margin: initial;
margin: unset;
```

Copy to Clipboard

A propriedade `margin` pode ser especificada usando um, dois, três ou quatro valores. Cada valor deve ser um `<length>`, uma `<percentage>`, ou a palavra-chave `auto`. Cada valor pode ser positivo, zero ou negativo.

- Quando **um** valor é especificado, a mesma margem é aplicada para **todos os quatro lados**.

- Quando **dois** valores são especificados, a primeira margem é aplicada aos **lados** **superior e inferior,** e a segunda aos **lados** **esquerdo e direito**.

- Quando **três** valores são especificados, a primeira margem é apliacada ao **topo**, a segunda aos **lados** **esquerdo e direito**, e a terceira ao **lado** **inferior**.

- Quando **quatro** valores são especificados, as margens são aplicadas aos lados **superior**, **direito**, **inferior** e **esquerdo**, nesta ordem (sentido horário).

  ### [Valores](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#valores)

  - **[`length` (en-US)](https://developer.mozilla.org/en-US/docs/Web/CSS/length)**

    O tamanho da margem como um valor fixo.

  - [`percentage` (en-US)](https://developer.mozilla.org/en-US/docs/Web/CSS/percentage)

    O tamanho da margem como um percetual, relativo à *largura* do bloco em que o elemento está contido.

  - `auto`

    O navegador seleciona uma margem adequada para utilizar. Por exemplo, em alguns casos este valor pode ser utilizado para centralizar o elemento.

  ### [Sintaxe formal](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#sintaxe_formal)

  ```
  [ (en-US) <length> (en-US) | (en-US) <percentage> (en-US) | (en-US) auto ] (en-US){ (en-US)1,4} (en-US)
  ```

  ## [Exemplos](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#exemplos)

  ### [Exemplo simples](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#exemplo_simples)

  #### HTML

  ```
  <div class="center">Este elemento está centralizado.</div>
  
  <div class="outside">Este elemento está posicionado fora de seu bloco recipiente.</div>
  ```

  Copy to Clipboard

  #### CSS

  ```
  .center {
    margin: auto;
    background: lime;
    width: 66%;
  }
  
  .outside {
    margin: 3rem 0 0 -3rem;
    background: cyan;
    width: 66%;
  }
  ```

  Copy to Clipboard

  

  ### [Mais exemplos](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#mais_exemplos)

  ```
  margin: 5%;                 /* todos os lados: margem de 5% */
  
  margin: 10px;               /* todos os lados: margem de 10px */
  
  margin: 1.6em 20px;         /* topo e inferior:    margem de 1.6em */
                              /* esquerda e direita: margem de 20px  */
  
  margin: 10px 3% 1em;        /* topo:               margem de 10px */
                              /* esquerda e direita: margem de 3%   */
                              /* inferior:           margem de 1em  */
  
  margin: 10px 3px 30px 5px;  /* topo:     margem de 10px */
                              /* direita:  margem de 3px  */
                              /* inferior: margem de 30px */
                              /* esquerda: margem de 5px  */
  
  margin: 2em auto;           /* topo e inferior: margem de 2em          */
                              /* caixa está horizontalmente centralizada */
  
  margin: auto;               /* topo e inferior: margem de 0            */
                              /* caixa está horizontalmente centralizada */
  ```

  Copy to Clipboard

  ## [Notas](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#notas)

  ### [Centralização horizontal](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#centralização_horizontal)

  Para centralizar algo horizontalmente em navegadores modernos, você pode utilizar `display: flex; justify-content: center;`

  Contudo, em navegadores antigos, como IE8-9 que não suporta layout flexbox, estes não estão disponíveis. Para centralizar um elemento dentro de seu pai, use `margin: 0 auto;` .

  ### [Colapso de margens](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#colapso_de_margens)

  Às vezes, as margens superior e inferior de elementos são colapsadas em uma única margem que é igual à maior das duas margens. Veja [Dominando margin collapsing](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing) para mais informações.

  ## [Especificações](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#especificações)

  | Especificação                                                | Status                   | Comentário                               |
  | :----------------------------------------------------------- | :----------------------- | :--------------------------------------- |
  | [CSS Box Model The definition of 'margin' in that specification.](https://drafts.csswg.org/css-box-3/#margin) | Candidata a Recomendação | Nenhuma mudança significativa.           |
  | [CSS Transitions The definition of 'margin' in that specification.](https://drafts.csswg.org/css-transitions/#animatable-css) | Rascunho atual           | Define `margin` como animável.           |
  | [CSS Level 2 (Revision 1) The definition of 'margin' in that specification.](https://www.w3.org/TR/CSS2/box.html#margin-properties) | Recomendação             | Remove seu efeito em elementos *inline*. |
  | [CSS Level 1 The definition of 'margin' in that specification.](https://www.w3.org/TR/CSS1/#margin) | Recomendação             | Definição inicial.                       |

  

  | [Initial value](https://developer.mozilla.org/pt-BR/docs/Web/CSS/initial_value) | as each of the properties of the shorthand: [`margin-bottom`](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin-bottom): `0`[margin-left (en-US)](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-left): `0`[margin-right (en-US)](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-right): `0`[`margin-top`](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin-top): `0` |
  | :----------------------------------------------------------- | ------------------------------------------------------------ |
  | Aplica-se a                                                  | all elements, except elements with table [`display`](https://developer.mozilla.org/pt-BR/docs/Web/CSS/display) types other than `table-caption`, `table` and `inline-table`. It also applies to [`::first-letter`](https://developer.mozilla.org/pt-BR/docs/Web/CSS/::first-letter) and [`::first-line`](https://developer.mozilla.org/pt-BR/docs/Web/CSS/::first-line). |
  | [Inherited](https://developer.mozilla.org/pt-BR/docs/Web/CSS/inheritance) | não                                                          |
  | Percentages                                                  | refer to the width of the containing block                   |
  | [Computed value](https://developer.mozilla.org/pt-BR/docs/Web/CSS/computed_value) | as each of the properties of the shorthand: [`margin-bottom`](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin-bottom): the percentage as specified or the absolute length[margin-left (en-US)](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-left): the percentage as specified or the absolute length[margin-right (en-US)](https://developer.mozilla.org/en-US/docs/Web/CSS/margin-right): the percentage as specified or the absolute length[`margin-top`](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin-top): the percentage as specified or the absolute length |
  | Animation type                                               | a [length](https://developer.mozilla.org/en-US/docs/Web/CSS/length#interpolation) |

  

  ## [Compatibilidade com navegadores](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin#browser_compatibility)

  [Report problems with this compatibility data on GitHub](https://github.com/mdn/browser-compat-data/issues/new?mdn-url=https%3A%2F%2Fdeveloper.mozilla.org%2Fpt-BR%2Fdocs%2FWeb%2FCSS%2Fmargin&metadata= MDN+page+report+details<%2Fsummary> *+Query%3A+`css.properties.margin` *+Report+started%3A+2022-06-16T20%3A03%3A16.584Z <%2Fdetails>&title=css.properties.margin+-+&template=data-problem.yml)

  |          |     desktop     |          mobile          |                 |                         |                   |                 |                  |                     |                    |                 |                   |                  |
  | :------- | :-------------: | :----------------------: | :-------------: | :---------------------: | :---------------: | :-------------: | :--------------: | :-----------------: | :----------------: | :-------------: | :---------------: | ---------------- |
  |          |     Chrome      |           Edge           |     Firefox     |    Internet Explorer    |       Opera       |     Safari      |  Chrome Android  | Firefox for Android |   Opera Android    |  Safari on iOS  | Samsung Internet  | WebView Android  |
  | `margin` | 1Toggle history |     12Toggle history     | 1Toggle history |     3Toggle history     | 3.5Toggle history | 1Toggle history | 18Toggle history |   4Toggle history   | 10.1Toggle history | 1Toggle history | 1.0Toggle history | 1Toggle history  |
  | `auto`   | 1Toggle history | 12footnoteToggle history | 1Toggle history | 6footnoteToggle history | 3.5Toggle history | 1Toggle history | 18Toggle history |   4Toggle history   |  14Toggle history  | 1Toggle history | 1.0Toggle history | 37Toggle history |

  ### Legend

  
