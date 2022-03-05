# ARIA15: Usando **aria-describedby** para fornecer descrições de imagens
* O objetivo desta técnica é fornecer descrições de imagens quando uma alternativa de texto curto não transmite adequadamente a função ou a informação fornecida no objeto.
* Um recurso do **WAI-ARIA** é a capacidade de associar texto descritivo a uma seção, desenho, elemento de formulário, imagem e assim por diante usando a propriedade **aria-describedby**.
* **aria-describedby** não pode fazer referência a descrições fora da página que contém a imagem.
* Assim como **aria-labelledby**, **aria-describedby** pode aceitar vários ids para apontar para outras regiões da página usando uma lista separada por espaços. Também é limitado a ids para definir esses conjuntos.

## Exemplo 1
```html
<img src="ladymacbeth.jpg" alt="Lady MacBeth" aria-describedby="p1">
<p id="p1">Esta pintura data de 1730 e é óleo sobre tela. Foi criado por Jean-Guy Millome, e representa ...</p>
```

## Teste
* Examine cada elemento de imagem em que um atributo descrito por aria esteja presente.
* Examine se o atributo **aria-describedby** associa programaticamente um elemento com sua descrição de texto, por meio do atributo id no elemento onde o texto a ser usado como descrição é encontrado.
* Examine se o equivalente de texto combinado e a descrição de texto associada descrevem com precisão ou fornecem a finalidade equivalente ao objeto.
* Resultado esperado: Verificação #1, #2 e #3 são verdadeiras.

## Referências
* https://www.w3.org/WAI/WCAG21/Techniques/aria/ARIA15