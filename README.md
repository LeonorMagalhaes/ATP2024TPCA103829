# Introdução
Este README aborda as soluções implementadas para os exercícios propostos nos TPCs 1, 2 e 3. Segue a reestruturação do conteúdo apresentada de maneira clara e objetiva:


## TPC1
*** a. Determinação de elementos não comuns em duas listas: ***
Combinações de compreensões de lista são usadas para identificar:
Elementos de lista1 que não estão na lista2.
Elementos de lista2 que não estão na lista1.
nao_comuns: Cria uma única lista com todos os elementos de ambas as listas (lista1 + lista2), mas inclui apenas aqueles que não pertencem a ambas ao mesmo tempo.
Ambas as abordagens retornam os elementos que aparecem apenas em uma das listas, sem duplicatas. 

*** b. Criação de uma lista de palavras com mais de três letras: ***
O texto é dividido usando split().
Apenas palavras com mais de 3 letras são armazenadas na nova lista.

*** c. Impressão de palavras com índice ajustado: ***
Itera pela lista de palavras, imprimindo o índice incrementado de cada elemento (para evitar começar em 0) junto com a palavra correspondente.


## TPC2
*** a.Contagem de ocorrências de uma substring: ***
A função recebe uma string e uma substring e verifica quantas vezes a substring ocorre na string principal.

*** b.Produto dos três menores números de uma lista: ***
Ordena a lista em ordem crescente (sort()).
Calcula o produto dos três menores valores e retorna o resultado.

*** c.Redução de um número a um único dígito: ***
Soma os dígitos repetidamente até obter um único dígito.
O processo é realizado enquanto o número for maior ou igual a 10.

*** d.Localização de uma substring em uma string: ***
Retorna a posição da primeira ocorrência de uma substring (usando index()), ou -1 caso não seja encontrada.


## TPC3
*** a. Contagem de posts: ***
Retorna a quantidade de posts presentes em uma rede social representada por uma lista.

*** b.Contagem de posts de um autor específico: ***
Pesquisa a lista que retorna o número de posts, de acordo com um autor especificado.

*** c. Adição de novos autores: ***
Insere o nome do autor na lista apenas se ele ainda não estiver presente.

*** d.Criação de novos posts: ***
Recebe informações como conteúdo, autor, data e quantidade inicial de comentários.
Gera um ID único e adiciona o post à lista de posts existente, de acordo com a introdução dos parâmetros:

redeSocial: Lista que armazena os posts.
conteudo: O texto do post.
autor: Nome do autor do post.
dataCriacao: Data de criação do post.
comentarios: Número inicial de comentários.

*Criação do novo post:*
O post é representado por um dicionário com as seguintes chaves:
'id': Gera um identificador único para o post, no formato 'pX', onde X é o número total de posts incrementado em 1 (assumindo que a função quantosPost retorna o total de posts atuais).
'conteudo': Texto do post.
'autor': Nome do autor.
'dataCriacao': Data em formato string.
'comentarios': Quantidade inicial de comentários.
Adiciona o post à rede social:
O novo post é adicionado à lista redeSocial com o método .append().

*Output:*
A função retorna a lista redeSocial atualizada. 

*** e.Remoção de posts por ID: ***
Localiza o post com base no identificador único e o remove da lista.

*  Parâmetros: 
redeSocial: Uma lista de dicionários, onde cada dicionário representa um post com uma chave 'id'.
id: O identificador ('id') do post que deve ser removido.

Iteração pela lista:A função percorre cada elemento (post) em redeSocial.Compara a chave 'id' do post atual com o valor fornecido em id.
Remoção do post: Se o 'id' do post corresponder ao valor especificado, o post é removido da lista usando o método .remove(post).

*Output:* :A função retorna a lista atualizada (redeSocial) com o post removido. 

*** f.Listagem de autores e posts: ***
Cria uma lista de tuplas contendo o autor e o post completo para cada entrada na rede social.

* Parâmetros:
redeSocial: Uma lista de dicionários, onde cada dicionário representa um post com várias informações, incluindo o autor (chave 'autor').
Processo: Cria uma lista vazia chamada lista.
Percorre cada post na lista redeSocial.Para cada post, adiciona à lista lista uma tupla contendo:
O autor do post (post['autor']). O post inteiro.

*Output*: A função retorna a lista de tuplas, onde cada tupla tem a forma (autor, post). 

*** g.Busca de comentários de um autor: ***
Identifica os posts que contêm comentários feitos por um autor específico.
Retorna os posts relevantes.

* Parâmetros:
redeSocial: Uma lista de dicionários, onde cada dicionário representa um post e inclui uma lista de comentários (na chave 'comentarios').
autor: Nome do autor dos comentários que você deseja buscar.
Processo: Inicializa uma lista vazia lista para armazenar os posts relevantes.
Percorre cada post em redeSocial.
Dentro de cada post, percorre a lista de comentários (post['comentarios']).
Verifica se o autor do comentário (comentario['autor']) corresponde ao autor fornecido.
Se encontrar um comentário do autor especificado, adiciona o post à lista lista.

*Output:*: A função retorna a lista lista, contendo os posts nos quais o autor especificado fez comentários.