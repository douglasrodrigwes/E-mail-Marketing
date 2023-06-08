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

## E-mail como imagem?

O uso do e-mail marketing como uma imagem chapada (ou seja, uma imagem única exportado seu corpo como um .png .jpg ou qualquer outro arquivo sem conteúdo de texto) pode não ser uma boa prática pelas seguintes razões:

 - <b>Acessibilidades:</b> Muitos usuários de e-mail têm configurações que bloqueiam imagens por padrão ou as exibem apenas quando solicitadas. Se o seu e-mail for composto principalmente por uma imagem, os destinatários podem não receber a mensagem que você deseja transmitir e ir direto para a caixa de spam.
 - <b>Mensagens bloqueadas:</b> Alguns servidores de e-mail ou programas de filtro podem bloquear e-mails com muitas imagens ou considerá-los suspeitos de spam. Isso pode fazer com que seu e-mail não alcance a caixa de entrada dos destinatários e com isso não ter a mensagem visualizada.
 - <b>Carregamento lento:</b> Dependendo da conexão de internet do destinatário ou das configurações do dispositivo, as imagens podem demorar a ser carregadas. Se a imagem for a parte principal da mensagem e não for exibida rapidamente, o destinatário pode perder o interesse ou até mesmo excluir o e-mail sem lê-lo.
 - <b>Dificuldade de leitura:</b> Se o conteúdo principal estiver incorporado em uma imagem, os destinatários não poderão pesquisar o texto, copiar trechos importantes ou traduzi-lo facilmente. Isso pode dificultar a compreensão da mensagem e a interação com o conteúdo. É importante salientar que o usuário não irá conseguir acessar os links de textos caso o e-mail possua, pois como é uma imagem não será possível o usuário clicar.

Para obter melhores resultados no e-mail marketing, é recomendável utilizar uma combinação equilibrada de imagens e texto. Isso garante que sua mensagem seja acessível, legível e capaz de transmitir informações importantes, mesmo que as imagens não sejam carregadas corretamente, mas claro que sempre pensando em um e-mail que atenda as boas práticas e acessibilidade para um bom e-mail profissional.

<br>

## Estrutura do e-mail marketing

<br>

## CSS no e-mail marketing 

<br>

## Responsividade 

<br>

## Boas práticas do e-mail marketing

<br>

## Péssimas práticas do e-mail marketing

<br>

## Comentários condicionais
A Microsoft introduziu os comentários condicionais em 1999 no <i>Internet Explorer 5</i>. A ideia é inteligente, pois dentro de um comentário HTML normal (< !-- -- >), você pode codificar uma condição que tornará o restante do conteúdo visível se for cumprido. Os comentários condicionais do <i>Outlook</i> nos permitem adicionar bits de HTML que são lidos apenas pelas versões do <i>Outlook</i> baseadas no Word.

Pontos históricos interessantes que são relevantes para o comentário condicional:
 - <b>Mecanismo de renderização:</b> O ponto inicial começa aqui, onde temos o Windows e seu novo mecanismo de renderização.
 - <b>Primeiro iphone:</b> Em 2007, a Apple lançou o primeiro iPhone.
 - <b>Microsoft:</b> Em 2007, a Microsoft introduziu o <i>Outlook</i> 2007 no <i>Windows</i> e seu novo mecanismo de renderização HTML e CSS - Word.
 - <b>Apple + futuro:</b> A Apple abre um caminho de possibilidades para seus usuários e desenvolvedores.
 - <b>O Outlook:</b> Enquanto isso, o <i>Outlook</i> condenou os e-mails em HTML em um código ultrapassado e obsoleto.
 
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

## Tabelas fantasmas 
Uma abordagem comum para lidar com problemas de renderização no <i>Outlook</i> é o uso de tags MSO para criar "tabelas fantasmas". Essas tabelas são criadas para evitar que os e-mails híbridos se desintegrem no <i>Outlook</i>. No design híbrido, usamos propriedades CSS como inline-block, max-width e min-width para empilhar as colunas da tabela. No entanto, o <i>Outlook</i> não oferece suporte a essas propriedades CSS, então recorremos às tags MSO para criar essas "tabelas fantasmas" que aplicam uma largura fixa somente para o Outlook. Isso nos permite garantir uma renderização consistente do conteúdo nos diferentes clientes de e-mail.

```
Tabela fantasma:

<!--[if mso]>
  <table role="presentation" cellspacing="0" cellpadding="0" border="0" width="100%">
    <tr>
      <td width="340">
        <![endif]-->
            <div style="display:inline-block; width:100%; min-width:200px; max-width:340px;">
              O Outlook não pode renderizar o CSS neste DIV, mas outros clientes de e-mail podem, então agrupamos isso em 
              uma tabela fantasma que replica o estilo de área de trabalho da DIV. Neste caso, um contêiner de 340px de largura.
            </div>
        <!--[if mso]>
      </td>
    </tr>
  </table>
<![endif]-->
```

<br>

## Direcionando versões específicas do Outlook
Ao desenvolver e testar e-mails, geralmente usamos < !--[if mso] > para abordar todas as versões do <i>Outlook</i>. No entanto, ocasionalmente, ao testar com o litmus, um e-mail pode parecer bom em uma versão do <i>Outlook</i>, mas ficar com problemas em outra. Embora seja raro, isso pode acontecer e existem algumas maneiras de segmentar versões específicas do <i>Outlook</i>, excluindo outras.

Versões do Outlook | Código
:--: | :--:
Todos os windows Outlook | < !--[if mso]> your code <![endif]-- >
Outlook 2000 | < !--[if mso 9]> seu código <![endif]-- >
Outlook 2002 | < !--[if mso 10]> seu código <![endif]-- >
Outlook 2003 | < !--[if mso 11]> seu código <![endif]-- > 
Outlook 2007 | < !--[if mso 12]> seu código <![endif]-- >
Outlook 2010 | < !--[if mso 14]> seu código <![endif]-- > 
Outlook 2013 | < !--[if mso 15]> seu código <![endif]-- >
Outlook 2016 | < !--[if mso 16]> seu código <![endif]-- > 

<br>

## Lógica condicional 
Os operadores permitem criar expressões condicionais para segmentar diferentes versões do <i>Outlook</i>.

Lógica | Descrição | Código
:--: | :--: | :--:
gt | Maior que | < !--[if gt mso 14]> Tudo acima do Outlook 2010 <![endif]-- > 
lt | Menor que | < !--[if lt mso 14]> Tudo acima do Outlook 2010 <![endif]-- >
gte | Melhor que ou igual a | < !--[if gte mso 14]> Outlook 2010 e superior <![endif]-- >
lte | Menos que ou igual a | < !--[if lte mso 14]> Outlook 2010 e superior <![endif]-- >
l  | Ou | < !--[if (mso 12) l (mso 16)] > Outlook 2007 / 2016 apenas < ![endif]-- >
! | Não | 	< !--[if !mso] >< !-- > Todos os Outlooks irão ignorar isso < !--<![endif]-- >

<br>

## LTR

<br>

## Links para consultas









 
