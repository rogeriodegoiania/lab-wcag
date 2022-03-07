# Critério de Sucesso 1.1.1 Conteúdo Não Textual
* Nível A
* Todo o conteúdo não textual que é exibido ao usuário tem uma alternativa textual que serve a um propósito equivalente, exceto para as situações indicadas abaixo

## Técnicas Suficientes - Técnicas alternativas de texto curto:
* G94: Fornecer alternativas de texto curto para conteúdo não textual que serve ao mesmo propósito e apresenta as mesmas informações que o conteúdo não textual
* ARIA6: Usando **aria-label** para fornecer rótulos para objetos
* ARIA10: Usando **aria-labelledby** para fornecer uma alternativa de texto para conteúdo não textual
* G196: Usando uma alternativa de texto em um item dentro de um grupo de imagens que descreve todos os itens do grupo
* H2: Combinando **links** de imagem e texto adjacentes para o mesmo recurso
* H37: Usando atributos **alt** em elementos **img**
* H53: Usando o corpo do elemento objeto
* H86: Fornecendo alternativas de texto para arte ASCII, emoticons e linguagem informal

## Técnicas Suficientes - Técnicas alternativas de texto longo:
* G95: Fornecer alternativas de texto curto que forneçam uma breve descrição do conteúdo não textual
* ARIA15: Usando **aria-describedby** para fornecer descrições de imagens
* G73: Fornecer uma descrição longa em outro local com um **link** para ela imediatamente adjacente ao conteúdo não textual
* G92: Fornecer uma descrição longa para conteúdo não textual que serve ao mesmo propósito e apresenta as mesmas informações
* H53: Usando o corpo do elemento objeto
* Observação: Longdesc foi depreciado no HTML e por este motivo não foi indicado aqui.

## Técnicas Suficientes - Técnicas alternativas de texto para controles e entrada:
* G82: Fornecer uma alternativa de texto que identifique a finalidade do conteúdo não textual
* ARIA6: Usando **aria-label** para fornecer rótulos para objetos
* ARIA9: Usando **aria-labelledby** para concatenar um rótulo de vários nós de texto
* H30: Fornecer texto de link que descreva a finalidade de um link para elementos âncora
* H36: Usando atributos alt em imagens usadas como botões de envio
* H44: Usando elementos de rótulo para associar rótulos de texto a controles de formulário
* H65: Usando o atributo title para identificar controles de formulário quando o elemento label não pode ser usado

## Técnicas Suficientes - Técnicas para indicar que alternativas de texto não são necessárias:
* C9: Usando CSS para incluir imagens decorativas
* H67: Usando texto alternativo nulo e nenhum atributo de título em elementos img para imagens que o AT deve ignorar

## Falhas
* F3: Falha do Critério de Sucesso 1.1.1 devido ao uso de CSS para incluir imagens que transmitem informações importantes
* F13: Falha no Critério de Sucesso 1.1.1 e 1.4.1 devido a ter uma alternativa de texto que não inclui informações transmitidas por diferenças de cor na imagem
* F20: Falha do Critério de Sucesso 1.1.1 e 4.1.2 devido à não atualização de alternativas de texto quando ocorrem alterações no conteúdo não textual
* F30: Falha no Critério de Sucesso 1.1.1 e 1.2.1 devido ao uso de alternativas de texto que não são alternativas (por exemplo, nomes de arquivos ou texto de espaço reservado)
* F38: Falha do Critério de Sucesso 1.1.1 devido à não marcação de imagens decorativas em HTML de uma forma que permita que a tecnologia assistiva as ignore
* F39: Falha no Critério de Sucesso 1.1.1 devido ao fornecimento de uma alternativa de texto que não é nula (por exemplo, alt="spacer" ou alt="image") para imagens que devem ser ignoradas pela tecnologia assistiva
* F65: Falha no Critério de Sucesso 1.1.1 devido à omissão do atributo alt ou alternativa de texto em elementos img, elementos de área e elementos de entrada do tipo "imagem"

## Referências
* https://www.w3.org/WAI/WCAG22/Understanding/non-text-content.html