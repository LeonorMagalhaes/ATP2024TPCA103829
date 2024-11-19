# Introdução:
Este README descreve o funcionamento do jogo proposto, baseado em fósforos, implementado com várias funções em Python.
Abaixo segue um resumo das principais funções implementadas no código para o desafio proposto:

 # 1. Função MostrarMenu()
Exibe um menu principal com três opções:
*Modo Normal:* O jogador joga primeiro, e o computador sempre vence seguindo uma estratégia específica.
*Modo Computador:* O computador joga primeiro, sem uma estratégia otimizada.
*Sair:* Encerra o jogo.

# 2. Função sair()
Imprime uma mensagem de despedida e encerra o programa.

# 3. Função modonormal()
Este é o modo onde o jogador inicia, mas o computador usa uma estratégia para garantir a vitória:

O jogo começa com 21 fósforos.
O jogador escolhe entre 1 e 4 fósforos para remover. Qualquer entradas inválida ou não suportada é rejeitada.
Se o número de fósforos restantes for 'zero' após a jogada do jogador, o jogador perde.
O computador então faz uma jogada estratégica, garantindo que a soma dos fósforos removidos por ambos em uma rodada seja sempre 5.
O jogo prossegue até restar apenas um fósforo, garantindo a vitória do computador.

# 4. Função modocomputador()
Neste modo, o computador joga primeiro:

O computador remove de 1 a 4 fósforos aleatoriamente usando 'random.randint()'.
Após a jogada, o número de fósforos restantes é atualizado.
O jogador faz sua jogada com as mesmas regras do modo anterior.
O jogo termina quando alguém remove o último fósforo, definindo o perdedor.

# 5. Função menu()
Gere o fluxo do jogo:

Exibe o menu inicial com *MostrarMenu()*.
Permite ao jogador escolher uma das opções:

1: Chama modonormal().
2: Chama modocomputador().
0: Chama sair().

Para além disto, valida a entrada do jogador para evitar valores inválidos.











