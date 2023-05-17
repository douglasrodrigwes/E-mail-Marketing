## E-mail-Marketing

<br>

## O que é e-mail marketing?
É um canal de marketing atraente, uma forma de pegar um serviço digital e unir o marketing direto e marketing digital, para assim usá-lo para promover seus produtos, serviços ou marcas da sua empresa. O e-mail marketing pode sugerir itens e ofertas recentes da sua empresa, podendo ser integrado ou automatizado, dependendo da plataforma. Ele pode desempenhar um papel na análise e estratégia de marketing, com geração de leads, reconhecimento da marca, relacionamento e fidelização de futuros clientes, e manter os clientes sempre engajados com diferentes tipos de e-mail marketing para diversos públicos.

<br>

## Vantagens do e-mail marketing
O e-mail tornou- se uma ferramenta indispensável para qualquer usuário, pois sendo quase sempre o usuário forçado a realizar algum tipo de ação. O e-mail sempre estará na caixa de entrada até ser lido, excluído ou arquivado. Com isso, o e-mail marketing conseguimos desenvolver um relacionamento com os clientes, ao mesmo tempo que direciona algum tipo de tráfego que você queira que as pessoas visitem.  

<br>

## Curiosidades
  - O primeiro e-mail foi enviado em 1971 : )<br>
  - Ray Tomlinson foi a primeira pessoa a enviar o primeiro e-mail, mas sendo constatado neste e-mail apenas uma série de letras e números.<br>
  - Ray Tomlinson foi a pessoa que introduziu o uso do símbolo "@" nos endereços de e-mails.<br> 
  - Gary Thuerk, gerente de marketing da <i>Digital Equipment Corp</i>, acabou utilizando deste novo tipo de comunicação direta para enviar o primeiro e-mail comercial, para informar as pessoas sobre um novo produto.<br>
  - A Lei de Proteção de Dados do Reino Unido, por exemplo, foi alterada para exigir uma opção de "cancelamento" para todos os e-mails de marketing, pois algumas pessoas não queriam receber mais aquela propaganda na sua caixa de entrada.    

<br>

## Comentários condicionais
A Microsoft introduziu os comentários condicionais em 1999 no <i>Internet Explorer 5</i>. A ideia é inteligente, pois dentro de um comentário HTML normal (<!-- -->), você pode codificar uma condição que tornará o restante do conteúdo visível se for cumprido. Os comentários condicionais do <i>outlook</i> nos permitem adicionar bits de HTML que são lidos apenas pelas versões do <i>outlook</i> baseadas no Word.

Pontos históricos interessantes que são relevantes para o comentário condicional:
 - <b>Mecanismo de renderização:</b> O ponto inicial começa aqui, onde temos o Windows e seu novo mecanismo de renderização.
 - <b>Primeiro iphone:</b> Em 2007, a Apple lançou o primeiro iPhone.
 - <b>Microsoft:</b> Em 2007, a Microsoft introduziu o <i>outlook</i> 2007 no <i>windows</i> e seu novo mecanismo de renderização HTML e CSS - Word.
 - <b>Apple + futuro:</b> A Apple abre um caminho de possibilidades para seus usuários e desenvolvedores.
 - <b>O outlook:</b> Enquanto isso, o <i>outlook</i> condenou os e-mails em HTML em um código ultrapassado e obsoleto.
 
```
Estrutura do comentário condicional:

<!--[if mso]>
    <table>
      <tr>
        <td>
        /* O conteúdo HTML específico que você quer que pegue no Outlook, vai aqui :) */
        </td>
      </tr>
    </table>
<![endif]-->
```

```
Comentário condicional no css:

<!--[if mso]>
    <style>
        .example-class {
            /* CSS específico que você quer que pegue no Outlook, vai aqui :) */
        }
    </style>
<![endif]-->
```

<br>

## Direcionando versões específicas do outlook
Ao desenvolver e testar e-mails, geralmente usamos < !--[if mso] > para abordar todas as versões do <i>outlook</i>. No entanto, ocasionalmente, ao testar com o litmus, um e-mail pode parecer bom em uma versão do Outlook, mas ficar com problemas em outra. Embora seja raro, isso pode acontecer e existem algumas maneiras de segmentar versões específicas do <i>outlook</i>, excluindo outras.

Versões do Outlook | Códigos
:--: | :--:
Todos os windows outlook | < !--[if mso]> your code <![endif]-- >
Outlook 2000 | < !--[if mso 9]> your code <![endif]-- >
Outlook 2002 | < !--[if mso 10]> your code <![endif]-- >
Outlook 2003 | < !--[if mso 11]> your code <![endif]-- > 
Outlook 2007 | < !--[if mso 12]> your code <![endif]-- >
Outlook 2010 | < !--[if mso 14]> your code <![endif]-- > 
Outlook 2013 | < !--[if mso 15]> your code <![endif]-- >
Outlook 2016 | < !--[if mso 16]> your code <![endif]-- > 

<br>

## Lógica condicional 
Os operadores permitem criar expressões condicionais para segmentar diferentes versões do <i>outlook</i>.

Lógica | Descrição | Códigos
:--: | :--: | :--:
gt | Maior que | < !--[if gt mso 14]> Everything above Outlook 2010 <![endif]-- > 
lt | Menor que | < !--[if lt mso 14]> Everything below Outlook 2010 <![endif]-- >
gte | Melhor que ou igual a | < !--[if gte mso 14]> Outlook 2010 and above <![endif]-- >
lte | Menos que ou igual a | < !--[if lte mso 14]> Outlook 2010 and below <![endif]-- >
l  | Ou | < !--[if (mso 12)|(mso 16)]> Outlook 2007 / 2016 only <![endif]-- >
! | Não | 	< !--[if !mso] >< !-- > All Outlooks will ignore this < !--<![endif]-- >







 
