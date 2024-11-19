## Introdução:
# Descrição do Sistema de Gerenciamento de Cinema
Este programa é uma aplicação simples para a gestão de cinemas, permitindo o controle de salas, filmes e vendas de bilhetes. O objetivo é proporcionar uma interface funcional para gerir exibições e lugares de forma eficiente.

## Estrutura Principal
# Salas de Cinema
Cada sala é representada como uma estrutura contendo:

*Capacidade máxima:* Total de lugares disponíveis na sala.
*Lista de lugares vendidos:* Inicialmente vazia, é atualizada com os lugares ocupados.
*Filme exibido:* Nome do filme associado à sala.

## Funcionalidades Principais
# MostrarMenu
Apresenta um menu interativo com as opções disponíveis, como listar filmes, comprar bilhetes ou adicionar salas.

# reset
Reinicia o sistema, limpando todas as salas e filmes já registados.

# existesala(cinema, sala)
Verifica se já existe uma sala com um filme específico em exibição, impedindo duplicidade.

# inserirsala(cinema, sala)
Adiciona uma nova sala ao cinema, garantindo que o filme ainda não está em exibição.

# listar(cinema)
Exibe uma lista de todos os filmes em exibição, acompanhados das respectivas capacidades das salas.

# disponivel(cinema, filmecin, lugar)
Confirma se um determinado lugare está disponível para venda numa sala específica.

# venderBilh(cinema, filmecin, lugar)
Processa a venda de bilhetes, verificando a disponibilidade de lugares e atualizando o registro da sala.

# listardisponibilidades(cinema)
Exibe o número de lugares ainda disponíveis para cada filme em exibição.

# cria_sala(cinema, filmecin, lugares)
Cria uma nova sala para exibição de um filme, definindo sua capacidade máxima de assentos.

# sair
Finaliza o programa com uma mensagem de despedida.

## Fluxo de Operação
A função principal *Menu* consiste em gerir as interações do utilizador, sendo apenas deixado de exibir quando o utilizador selecione a opção 'Sair'.

*Menu* permite ações como:
- Verificar a lista de filmes e suas capacidades.
- Criar novas salas ou filmes.
- Comprar bilhetes para assentos específicos.
- Consultar a disponibilidade de assentos.
- Inclui validações para evitar erros, como criar duas salas para o mesmo filme ou vender assentos já ocupados.

# Conslusão/Finalidade
Este programa é ideal para simular uma aplicação de gestão básica de um cinema, proporcionando ao utilizador um controle completo sobre as operações relacionadas às salas, filmes e vendas de bilhetes.











O ChatGPT pode cometer erros. Consider