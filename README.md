Para este Tcp , o desafio proposto consiste em desenvolver um jogo interativo em Python chamado "Adivinha o Número", que possui dois *modos de funcionamento*:

# Modos de funcionamneto do Jogo: 
*Modo Computador*: O jogador tenta descobrir um número que foi gerado aleatoriamente pelo programa.
*Modo Jogador:* O jogador pensa em um número, e o computador tenta adivinhar utilizando um método de busca otimizado.
Estrutura do Menu

# Menu
Ao iniciar o programa, é exibido um menu com três opções principais:

1: Jogar no Modo Computador.
2: Jogar no Modo Jogador.
0: Encerrar o programa.
A opção desejada é selecionada pelo jogador através de um comando input, sendo armazenada na variável correspondente.

# Funcionamento por Opção
*Opção 0*: Sair
Quando o jogador escolhe esta opção, o programa exibe uma mensagem de despedida e finaliza a execução.

*Opção 1*: Modo Computador
Neste modo:

O computador gera um número aleatório entre 0 e 100 utilizando a função random.randint.
O jogador faz palpites sucessivos, inserindo números pelo teclado.
O programa informa se o palpite é maior ou menor que o número gerado, ajustando a busca até que o jogador acerte.
Um contador registra a quantidade de tentativas até o acerto.
*Opção 2*: Modo Jogador
Neste modo:

O jogador pensa em um número secreto entre 0 e 100, e o computador tenta adivinhá-lo.
Utilizando a busca binária, o computador faz palpites com base na média do intervalo atual.
O jogador responde com "Acertou", "Maior" ou "Menor", indicando se o palpite está correto ou se o computador precisa ajustar o intervalo.
O processo se repete até que o computador identifique o número, mostrando a quantidade de tentativas realizadas.
Estrutura de Repetição
Em ambos os modos, um loop principal mantém o jogo ativo até que a condição de acerto seja atingida.

# Contador de Tentativas
Cada tentativa é contabilizada, e o total é exibido ao final do jogo, incentivando o jogador a buscar soluções mais eficientes.
Esta estrutura combina lógica de programação com interatividade, promovendo aprendizado e diversão para quem desenvolve e joga.