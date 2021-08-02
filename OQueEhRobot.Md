# Robots.txt

## Saiba o que é o Robots.txt e como usá-lo


### Você sabe o que é o Robots.txt? Nós te mostramos tudo sobre esse arquivo e como ele é importante para o seu site

##### Rock Content

## Robots Txt

Garantir que seu site apareça nas buscas dos usuários é essencial para o sucesso de qualquer estratégia de Marketing Digital.

Para conquistar este objetivo é comum que você invista em estratégias de SEO, Marketing de Conteúdo e uma série de outras ações capazes de atrair a atenção das ferramentas de busca e, com isso, aumentar o tráfego de sua página.

Porém há páginas de seu site que você não deseja que sejam rastreadas pelas ferramentas de busca, como as páginas de login e outras que possuam arquivos de acesso exclusivo a clientes ou membros de sua equipe.

Para ajudá-lo a ocultar estas páginas é que existe o robots.txt.

## O que é robots.txt?

O robots.txt é um arquivo deve ser salvo na pasta raiz do seu site, e indica para os robôs de busca do Google, Bing e muitas outras quais as páginas de seu site você não deseja que sejam acessadas por estes mecanismos de pesquisa.

E como o próprio nome dá a entender, o robots .txt é um arquivo no formato .txt que pode ser criado no próprio bloco de notas de seu computador, excluindo a necessidade de uma ferramenta para sua criação.

O robots.txt usa o formado do Protocolo de Exclusão de Robôs padrão, um conjunto de comandos que são usados pelos robôs de busca quais os diretórios e páginas de seu site não devem ser acessados por eles.

Como o arquivo é salvo diretamente na pasta raiz do site, acessar os arquivos robots.txt de outras páginas é bem simples: basta digitar o endereço da página no seu navegador e adicionar o comando “/robots.txt” ao final da URL.

Fazer isso pode te dar insights interessantes, além de permitir que você conheça alguns endereços que seus concorrentes desejam esconder de suas páginas.

## Para que serve o robots.txt?

Como já dissemos, o robots.txt serve para dar ordens específicas para os robôs de busca.

Para que você entenda um pouco melhor, listamos suas funções específicas.

## Controla o acesso a arquivos de imagem

O robots.txt é capaz de impedir que os arquivos de imagem de sua página sejam exibidos nos resultados de busca.

Isso ajuda a controlar o acesso de algumas informações importantes, como infográficos e detalhes técnicos de produtos.

Por não serem exibidas nos resultados de busca, o usuário terá a obrigação de acessar a sua página, o que pode ser mais interessante para sua empresa.

Porém é importante destacar que o robots.txt não impede que outras páginas e usuários copiem e compartilhem os links de suas imagens.

Existem outras ferramentas para ajudá-lo neste objetivo.

## Controla o acesso às páginas da web

Sua página também é composta por aquivos que não são de imagem, que são as próprias páginas da web de sua página.

Além de impedir que os robôs de busca acessem a páginas de acesso restrito ou irrelevantes para sua estratégia, o uso do robots.txt ajuda a evitar que o servidor que hospeda seu site fique sobrecarregado com os acessos dos robôs de busca, ajudando a sua empresa a economizar dinheiro.

Porém é importante lembrar que, assim como no caso das imagens, os usuários ainda podem localizar algumas de suas páginas se tiverem o link de acesso direto a elas.

## Bloquear acessos a arquivos de recursos

Além do bloqueio de imagens e de suas páginas da web, o robots.txt pode ser útil para bloquear o acesso a outros arquivos de script e de estilo menos importantes, poupando os seus servidores.

Porém você também deve usar esta função com cautela, principalmente se estes recursos forem indispensáveis para o carregamento correto de sua página, o que pode dificultar o trabalho dos rastreadores, prejudicando a análise de sua página.

## Guia do SEO 2.0

### Como criar um arquivo robots.txt

Criar um arquivo robots.txt é bem simples, exigindo apenas o conhecimento de poucos comandos específicos.

Este arquivo pode ser criado no bloco de notas de seu computador ou outro editor de texto de sua preferência.

Você vai precisar também do acesso à pasta raiz de seu domínio.

Para criar um arquivo robots.txt, você precisa acessar a raiz do seu domínio, onde você irá salvar o arquivo que você criou.

Após isso, você precisará conhecer um pouco da sintaxe e os comandos do robots.txt

## Os comandos do robots.txt

Os comandos no robots.txt funcionam de forma semelhante ao HTML e as diversas linguagens de programação existentes no mercado.

Existem comandos que serão seguidos pelos robôs para navegar e encontrar as páginas de seu site.

Veja alguns dos principais comandos do arquivo robots.txt:

## O comando User-agent

Você pode inserir ordens específicas para cada robô de busca existente no mercado em seu arquivo robots.txt, bastando usar o comando User-agent para determinar qual robô de busca você está se referindo.

Para conhecer o nome de cada User-agent você pode consultar o Web Robots Database, que lista os robôs das principais ferramentas de busca do mercado.

O principal robô de busca do Google é o Googlebot.

Se você quisesse dar ordens específicas para ele, o comando inserido em seu robots.txt seria esse:

'''
User-agent: Googlebot
'''

Se quisesse deixar ordens específicas para o robô de busca do Bing, o comando seria este:

'''
User-agent: Bingbot
'''

Como você pode ver, basta apenas que você altere o nome do User-agent.

E caso você queira inserir um direcionamento geral para ser seguido por todos os robôs de busca, basta substituir o nome do User-agent por um asterisco. Seria assim:

'''
User-agent: *
'''


## O Comando Disallow

O comando Disallow é o responsável por descrever quais as páginas diretórios ou sites não devem ser incluídas nos resultados de busca.

Assim como o comando User-agent, basta inserir o endereço da página após o comando.

Para orientar os robôs a não acessarem a página “beta.php” de seu site o comando seria esse:

'''
Disallow: /beta.php
'''

Você ainda pode impedir o acesso à pasta específicas.

Se precisasse bloquear o acesso à pasta “arquivos”, o comando seria esse:

'''
Disallow: /arquivos/
'''

Existe também a possibilidade de bloquear o acesso a conteúdos que comecem com uma letra específica.

Para bloquear o acesso a todos as pastas e arquivos que comecem com a letra “a”, o comando seria esse:

'''
Disallow: /a
'''

## O Comando Allow

O comando Allow permite que você determine para os robôs de busca quais as páginas ou diretórios de seu site você deseja que sejam indexadas.

Por padrão todas as páginas de seu site serão indexadas, exceto quando você usar o comando Disallow.

Sendo assim, o uso do comando Allow é recomendado apenas quando você precisar bloquear uma pasta ou diretório por meio do comando Disallow, mas gostaria de ter indexado um arquivo ou pasta específico que está dentro do diretório bloqueado.

Se você quiser bloquear o acesso à pasta “arquivos”, mas precisar liberar o acesso à página “produtos.php”, o comando seria assim:

'''
Disallow: /arquivos/

Allow: /arquivos/produtos.php
'''

Se você quiser bloquear o acesso à pasta “arquivos”, mas precisar liberar o acesso à pasta “projetos”, o comando seria assim:

'''
Disallow: /arquivos/

Allow: /arquivos/projetos/
'''

## O Comando Sitemap

Outro comando útil para um arquivo robots.txt é a indicação do sitemap de sua página, muito útil para auxiliar os robôs de busca a identificarem todas as páginas existentes em seu site.

Porém é um comando que tem caído em desuso, principalmente por conta do Google Webmaster Tools, ferramenta para Webmasters do Google que permite informar o local de seu arquivo sitemap de forma rápida, além de outras funções.

Para inserir o endereço de seu sitemap você precisa ter salvo o arquivo de seu sitemap salvo na pasta raiz de seu site. O comando para inserir este endereço em seu site é este:

Sitemap: https://www.seusite.com.br/sitemap.xml

## Guia do Google Search Console

### Quais são as limitações do robots.txt

Apesar de ser muito útil para direcionar o acesso dos robôs de busca a sua página, é preciso reconhecer que o robots.txt possui algumas limitações.

Conhecê-las é importante, principalmente para identificar a necessidade de utilizar outros artifícios para que suas URLs não sejam encontradas facilmente nas buscas.

### As instruções do arquivo robots.txt são apenas diretivas

Embora o uso do robots.txt seja um padrão do mercado, as ferramentas de busca não são obrigadas a seguir todas as suas ordens.

Isso quer dizer que por mais que os robôs de busca do Google sigam as instruções do arquivo robots.txt, outras ferramentas de busca podem não fazer o mesmo.

Por isso é importante que além do arquivo robots.txt você use outros métodos em conjunto para ocultar suas páginas do Google, como o acesso protegido por senha ou uso das meta tags noindex em seu código html.

## Cada robô de busca pode interpretar a sintaxe de maneiras diferentes

Apesar de seguir um padrão internacional, os comandos inseridos no robots.txt podem ser interpretados de forma diferente por robô de busca.

Por isso, para garantir a sua correta utilização é preciso conhecer a sintaxe ideal para atender cada ferramenta de busca.

Isso quer dizer que, além de compreender como o Google interpreta as informações do robots.txt, pode ser necessário que você aprenda também a metodologia do Bing, Yahoo e qualquer outra ferramenta de busca do mercado.

## Os direcionamentos do robots.txt não impedem que outros sites façam referências a suas URLs

Um erro muito comum é achar que um conteúdo bloqueado pelo robots.txt não pode ser encontrado de outras formas pelos usuários e até mesmo por seus concorrentes.

Por este motivo, caso uma URL restrita possa ser divulgada em outros sites ou blog esta página ainda pode aparecer nos resultados de busca.

Por isso é indispensável inserir a tag noindex e até mesmo bloquear o acesso através de senha para garantir que ninguém tenha acesso à sua página.

## Pode ser necessário dar ordens específicas para cada robô de busca

Alguns robôs de busca seguem regras e lógicas próprias, o que pode obrigar que você determine regras específicas para cada um deles no seu arquivo robots.txt.

E além de aumentar seu volume de trabalho, isso pode gerar erros na criação de seus arquivos.

Portanto tenha muito cuidado ao definir regras para robôs específicos, tendo certeza de que as instruções estão claras para cada um deles.

Agora que você já sabe o que é e como criar um arquivo robots.txt, o trabalho de gestão de seu site será facilitado, garantindo que apenas as páginas importantes para seu negócio sejam visitadas pelos robôs de busca.

Se quiser saber mais sobre como otimizar o seu site para os robôs de busca, confira nosso KIT Domine o Google!

[Artigo original](https://rockcontent.com/br/blog/robots-txt/)