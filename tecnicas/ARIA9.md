# ARIA9: Usando **aria-labelledby** para concatenar um rótulo de vários nós de texto

* A propriedade **aria-labelledby** pode ser usada para rotular todos os objetos visuais
* Aplicada a entradas, a propriedade **aria-labelledby** pode ser usada para rotular entradas nativas, bem como elementos não nativos, como entradas de texto personalizadas construídas com **div contenteditable="true"**.
* Um uso específico de **aria-labelledby** é para entradas de texto em situações em que um rótulo significativo deve consistir em mais de uma sequência de rótulos.
* O valor do atributo **aria-labelledby** é então uma lista separada por espaços de todos os ids na ordem em que as strings de rótulos referenciadas devem ser lidas pelos leitores de tela.
* Outra aplicação do **aria-labelledby** é quando não há espaço para fornecer um rótulo visível ao lado da entrada, ou quando o uso de rótulos nativos cria redundância desnecessária.

## ARIA - Precedências
* 1. **aria-labelledby**
* 2. **aria-label**
* 3. elemento **label**
* 4. atributo **placeholder**
* 5. atributo **title**

## Exemplo 1
```html
<form>
    <p>
        <span id="timeout-label">
            <label for="timeout-duration">Estender o tempo limite para</label>
        </span>
        <input type="text" size="3" id="timeout-duration" value="20" aria-labelledby="timeout-label timeout-duration timeout-unit">
        <span id="timeout-unit"> minutos</span>
    </p>
</form>
```

## Exemplo 2
```html
<table>
	<tr>
		<td></td>
		<th id="tpayer">Contribuinte</th>
		<th id="sp">Cônjuge</th>
	</tr>

	<tr>
		<th id="gross">W2 Bruto</th>
		<td><input type="text" size="20" aria-labelledby="tpayer gross" /></td>
		<td><input type="text" size="20" aria-labelledby="sp gross" /></td>
	</tr>
	
	<tr>
		<th id="div">Dividendos</th>
		<td><input type="text" size="20" aria-labelledby="tpayer div" /></td>
		<td><input type="text" size="20" aria-labelledby="sp div" /></td>
	</tr>
</table>
```

## Teste
* 1. Verifique se os ids referenciados em **aria-labelledby** são exclusivos e correspondem aos ids dos nós de texto que juntos fornecem o rótulo.
* 2. Verifique se o conteúdo concatenado dos elementos referenciados por **aria-labelledby** é descritivo para o propósito ou função do elemento rotulado.
* Resultado esperado: Verificação #1 e #2 são verdadeiras.

## Referências
* https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA9
* https://www.w3.org/TR/html-aapi/#accessible-name-and-description-calculation