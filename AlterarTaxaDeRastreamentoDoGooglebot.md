# Robot.txt

## Uso adequado

O Google tem algoritmos sofisticados para determinar a velocidade de rastreamento ideal para um site. Nosso objetivo é rastrear o maior número possível de páginas no seu site a cada visita, sem sobrecarregar a largura de banda do servidor.

Se o Google fizer muitas solicitações por segundo para o site e deixar o servidor mais lento, limite a velocidade do processo.

Você pode restringir a taxa de rastreamento para sites no nível raiz, por exemplo, www.example.com e http://subdomain.example.com. A taxa de rastreamento que você definir será o limite máximo permitido ao Googlebot. Isso não garante que ele atingirá essa taxa máxima.

Recomendamos não limitar a taxa de rastreamento, a menos que você note problemas de carregamento do servidor que sejam realmente em função de uma sobrecarga causada pelo Googlebot.

Não é possível alterar a taxa de rastreamento para sites que não estão no nível raiz (por exemplo, www.example.com/pasta).

## Limitação da taxa de rastreamento

Abra a página de configurações da taxa de rastreamento da propriedade.
- Se a taxa for "calculada como ideal", a única maneira de reduzi-la será enviando uma solicitação especial. Não é possível aumentar a taxa de rastreamento.
- Caso contrário, selecione a opção desejada para aplicar o limite. A nova taxa de rastreamento é válida por 90 dias.
- Limitação emergencial do rastreamento


## Veja como proteger o site se a frequência de rastreamento estiver causando problemas de disponibilidade:

- Determine qual rastreador do Google está acessando o site em excesso. Analise os registros do seu site ou use o Relatório de estatísticas de rastreamento.
- Solução rápida:
- Se quiser uma solução simples, use o robots.txt para bloquear o rastreamento do agente que causa a sobrecarga (googlebot, adsbot etc.). No entanto, isso pode levar até um dia para entrar em vigor.
- Caso você consiga detectar e responder ao aumento na demanda de forma dinâmica, retorne o HTTP 5XX/429 quando estiver perto do limite de exibição. No entanto, não retorne 5XX ou 429 por mais de dois ou três dias, porque isso pode fazer com que o Google rastreie o site com menos frequência a longo prazo.
- Mude a taxa de rastreamento usando a página de configurações da taxa de rastreamento, se a opção estiver disponível.
- Dois ou três dias depois, quando a taxa de rastreamento do Google estiver adaptada, remova os bloqueios do robots.txt ou deixe de retornar os códigos de erro da etapa 1.
- Se o site está sobrecarregado com os rastreamentos do AdsBot, é provável que você tenha criado muitas segmentações para anúncios dinâmicos de pesquisa usando URL_Equals ou feeds de páginas. Caso seu servidor não tenha a capacidade necessária para lidar com esses rastreamentos, limite as segmentações de anúncio, adicione URLs em lotes menores ou aumente a capacidade de exibição. Como o AdsBot rastreia suas páginas a cada duas semanas, você precisa corrigir o problema para isso não acontecer novamente.
- Se você tiver usado a página de configurações para limitar a taxa de rastreamento, ela voltará ao ajuste automático após 90 dias

[Artigo original](https://support.google.com/webmasters/answer/48620?hl=pt)