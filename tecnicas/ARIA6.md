# ARIA6: Usando **aria-label** para fornecer rótulos para objetos
* O objetivo dessa técnica é fornecer um rótulo para objetos que possam ser lidos por tecnologia assistiva. O atributo **aria-label** fornece o rótulo de texto para um objeto, como um botão. Quando um leitor de tela encontra o objeto, o texto aria-label é lido para que o usuário saiba o que é.
* Os autores devem estar cientes de que aria-label pode ser desconsiderada por tecnologias assistivas em situações em que **aria-labelledby** é usada para o mesmo objeto

## Exemplo 1
```html
<div role="navigation" aria-label="Primary">
<ul><li>...uma lista de links aqui ...</li></ul> </div>
<div role="navigation" aria-label="Secondary">
<ul><li>...uma lista de links aqui ...</li> </ul></div>
```

## Teste
* Para cada elemento onde um atributo **aria-label** está presente: Examine se a descrição do texto rotula com precisão o objeto ou fornece uma descrição de sua finalidade ou fornece informações equivalentes.
* Resultado esperado: Verificação #1 é verdadeira.

## ARIA - Precedências
* 1. **aria-labelledby**
* 2. **aria-label**
* 3. elemento **label**
* 4. atributo **placeholder**
* 5. atributo **title**

## Referências
* https://www.w3.org/WAI/WCAG21/Techniques/aria/ARIA6
* https://www.w3.org/TR/html-aapi/#accessible-name-and-description-calculation