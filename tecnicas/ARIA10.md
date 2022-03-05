# ARIA10: Usando **aria-labelledby** para fornecer uma alternativa de texto para conteúdo não textual
* O objetivo desta técnica é fornecer uma breve descrição de um elemento que pode ser lido por tecnologias assistivas (AT) usando o atributo **aria-labelledby**.
* O atributo **aria-labelledby** associa um elemento a um texto que é visível em outro lugar na página usando um valor de referência de ID que corresponde ao atributo ID do elemento de rotulagem.

## Exemplo 1
```html
<div role="img" aria-labelledby="star_id">
    <img src="fullstar.png" alt=""/>
    <img src="fullstar.png" alt=""/>
    <img src="fullstar.png" alt=""/>
    <img src="fullstar.png" alt=""/>
    <img src="emptystar.png" alt=""/>
</div>

<div id="star_id">4 de 5</div>
```

## Teste
* 1. Examine cada elemento onde o atributo **aria-labelledby** está presente e o elemento não suporta o atributo alt.
* 2. Verifique se o valor do atributo **aria-labelledby** é o id de um elemento na página da web.
* 3. Determine se o texto do elemento identificado pelo atributo **aria-labelledby** rotula com precisão o elemento, fornece uma descrição de sua finalidade ou fornece informações equivalentes.
* Resultado esperado: Verificação #2 e #3 são verdadeiras.

## Referências
* https://www.w3.org/WAI/WCAG21/Techniques/aria/ARIA10