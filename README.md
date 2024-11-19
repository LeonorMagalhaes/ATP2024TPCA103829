# Introdução:
Este README descreve o funcionamento do jogo proposto, implementado com várias funções em Python.
Abaixo segue um resumo das principais funções implementadas no código para o desafio proposto:

# Funções principais:
*exibirMenu:* Mostra as opções disponíveis no programa, como criar uma lista ou encerrar a aplicação.

*gerarListaAleatoria:* Cria uma lista contendo números aleatórios com o tamanho definido pelo usuário.

*criarListaManual:* Permite ao usuário adicionar elementos manualmente à lista, inserindo números por meio de inputs.

# Funções de cálculo:

*calcularSoma:* Retorna a soma dos elementos da lista.
*calcularMedia:* Calcula e exibe a média dos valores presentes na lista.
*encontrarMaior:* Identifica e retorna o maior número da lista.
*encontrarMenor:* Localiza o menor valor da lista.

# Análise de ordenação:

*verificarCrescente:* Avalia se a lista está organizada em ordem crescente.
*verificarDecrescente:* Confirma se os elementos estão em ordem decrescente.
*buscarElemento:* Permite procurar um valor específico na lista e retorna sua posição, caso seja encontrado.

*encerrarPrograma:* Finaliza a execução do programa quando o usuário escolhe a opção correspondente no menu.

#  Estrutura principal (menuPrincipal):
A função principal, menuPrincipal, utiliza um loop que apresenta continuamente o menu ao usuário e processa suas escolhas. Com base na seleção:

A criação de listas pode ser feita de forma manual ou automática.
Operações como soma, média, maior ou menor valor são executadas usando a lista atual.
Caso o usuário deseje verificar a ordenação da lista, as funções apropriadas são chamadas.
A busca por elementos específicos também pode ser realizada.
Escolher a opção "Sair" encerra o loop, exibindo uma mensagem antes de finalizar o programa.
Essa organização garante que todas as funcionalidades sejam acessíveis de maneira clara e intuitiva.
