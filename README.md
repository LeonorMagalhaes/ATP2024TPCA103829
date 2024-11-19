## Sistema de Gestão Escolar
Este programa é uma solução simples para organizar e gerir informações de turmas e alunos, com funções para criar turmas, registar alunos, listar informações, e salvar ou carregar dados de arquivos.

# Estrutura de Dados
Turmas: Representadas como uma lista de tuplos, cada uma contendo:

- Nome da turma.
- Lista de alunos pertencentes a essa turma.
- Alunos: Cada aluno é armazenado como uma tupla com:
turma (nome, numero, )

# Nome do aluno.
Identificador único (ID).
Notas (lista de três números).
Funcionalidades do Sistema
# Exibição do Menu:
Apresenta ao usuário as opções disponíveis, como criação de turmas, inserção de alunos, listagem e salvamento de dados.

# Funções:

1. *existeturma(nome_turma, escola)*:
    Garante que não haja duplicidade de nomes ao criar novas turmas.

2. *criarTurma(nome_turma, escola)*:
    Permite inserir novas turmas no sistema após verificação de unicidade.

3. *inserir_aluno(nome_turma, aluno)*:
    Adiciona um aluno a uma turma específica. O ID do aluno é validado para evitar duplicações na turma.

4. *listar(nome_turma)*:
    Mostra os alunos cadastrados em uma turma, incluindo nomes, IDs e notas, ou informa caso a turma não seja encontrada.

5. *consultar_aluno(id_aluno, nome_turma)*:
    Busca por um aluno específico em uma turma, exibindo suas informações ou notificando a ausência do aluno.

6. *guardar_turma(nome_turma, fnome)*:
    Registra os dados de uma turma em um arquivo externo no formato txt.

7. *recuperar_turma(fnome)*: 
    Recupera os dados de uma turma de um arquivo de texto e retorna uma lista de alunos com seus respectivos dados.

9. *Menu()*: 
    Controla o fluxo principal da aplicação, chamando as funções apropriadas de acordo com a escolha do usuário. Permite ao usuário navegar pelas funcionalidades de criação, inserção, listagem, consulta, armazenamento e recuperação de turmas e alunos.



## Funcionamento da Navegação e Controle do 'Menu':
Uma função central organiza o fluxo do programa, chamando as opções selecionadas pelo usuário.

. **Executar o Programa**: Execute o código para iniciar a aplicação. O menu será exibido com as opções disponíveis.

2. **Navegar pelo Menu**:
    - **Criar Turma**: Digite o nome de uma nova turma para adicioná-la à escola.
    - **Inserir Aluno**: Escolha uma turma e insira os dados de um aluno (nome, ID e notas).
    - **Listar Turma**: Liste todos os alunos de uma turma específica.
    - **Consultar Aluno por ID**: Encontre um aluno pelo ID em uma turma específica.
    - **Guardar Turma em Ficheiro**: Salve os dados de uma turma em um arquivo.
    - **Carregar Turma de um Ficheiro**: Carregue uma turma de um arquivo para a memória.
    - **Sair**: Encerre a aplicação.

# Encerramento do Sistema:
Finaliza o programa com uma mensagem de despedida, encerrando o loop principal.

# Instruções de Uso
Navegue pelo Menu:
Escolha opções como criar turmas, cadastrar alunos, listar ou consultar informações, e salvar ou carregar dados.

# Manuseio de Arquivos:
Utilize as funcionalidades de salvamento e recuperação para manter as informações organizadas entre execuções.


# Observações Adicionais

- Interface Simples: Todos os comandos são insensíveis a letras maiúsculas ou minúsculas, simplificando a interação do usuário.
- IDs Exclusivos: Garante que cada aluno tenha um identificador único dentro de sua turma.
- Flexibilidade: O código permite expansão fácil para novas funcionalidades ou melhorias futuras.
- Facilidade de Uso: Nomes de turmas são padronizados para evitar problemas de busca ou armazenamento.
Este sistema foi projetado para ser direto e eficiente, oferecendo uma solução prática para o gerenciamento de informações escolares.