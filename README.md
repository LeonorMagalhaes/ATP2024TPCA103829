## Sistema de Análise Climática
# Introdução
Este programa é uma aplicação desenvolvida em Python para processar e analisar dados climáticos diários. Permite ainda calcular estatísticas e visualizar informações meteorológicas de forma gráfica, com base em uma tabela que armazena dados como temperaturas e precipitação.


# Principais Funções:
A aplicação organiza suas operações em um menu interativo, com as seguintes opções:

1. **Cálculo da Temperatura Média Diária:** Determina a média da temperatura diária, considerando as temperaturas mínima e máxima.
2. **Salvar Dados Meteorológicos:** Permite salvar a tabela de dados em um arquivo de texto.
3. **Carregar Dados Meteorológicos:** Importa dados salvos previamente de um arquivo de texto.
4. **Identificação da Menor Temperatura Mínima:** Exibe o menor valor de temperatura mínima registrado.
5. **Cálculo da Amplitude Térmica Média:** Determina a variação média entre as temperaturas máxima e mínima diárias.
6. **Registro da Maior Precipitação:** Mostra o dia com maior precipitação e o valor registrado.
7. **Dias com Precipitação Superior a um Valor:** Lista os dias onde a precipitação excedeu um valor especificado pelo usuário.
8. **Período de Baixa Precipitação:** Determina o maior intervalo consecutivo de dias com precipitação abaixo de um valor informado pelo usuário.
9. **Geração de Gráficos:** Cria gráficos de linha para as temperaturas mínima e máxima e um gráfico de barras para a precipitação diária.
10. **Sair:** Finaliza o programa.

# Estrutura dos Dados
Os dados climáticos são armazenados em uma lista de tuplos, onde cada entrada possui o seguinte formato:

((ano, mês, dia), temperatura mínima, temperatura máxima, precipitação)

tabMeteo1 = [
    ((2023, 11, 15), 5, 18, 0.5),
    ((2023, 11, 16), 7, 19, 0),
    ((2023, 11, 17), 6, 20, 1.2)]


1. **Configuração Inicial**: Executa o código fornecido para iniciar o programa e exibir o menu.
2. **Selecionar Opções**: No menu, escolhe a opção desejada digitando o número correspondente.
3. **Parâmetros para Precipitação (`p`)**: Para as opções 7 e 8, o utilizador deverá fornecer um valor de precipitação (`p`).
4. **Visualizar Gráficos**: A opção 9 exibe gráficos de temperatura mínima e máxima ao longo do tempo e de precipitação diária.

### Funções Principais

- **mostrar_menu**: Exibe o menu de opções.
- **medias(tabMeteo)**: Calcula a média diária da temperatura.
- **guardatabMeteo(t, fnome)**: Guarda a tabela meteorológica em um arquivo de texto.
- **carregatabMeteo(fnome)**: Carrega a tabela meteorológica a partir de um arquivo de texto.
- **minMin(tabMeteo)**: Encontra a temperatura mínima mais baixa.
- **amplTerm(tabMeteo)**: Calcula a amplitude térmica diária.
- **maxChuva(tabMeteo)**: Identifica o dia e o valor da precipitação máxima.
- **diasChuvosos(tabMeteo, p)**: Lista os dias com precipitação superior ao valor `p`.
- **maxPeriodoCalor(tabMeteo, p)**: Calcula o maior número consecutivo de dias com precipitação abaixo do valor `p`.
- **grafTabMeteo(t)**: Gera gráficos de temperatura mínima e máxima e de precipitação.











