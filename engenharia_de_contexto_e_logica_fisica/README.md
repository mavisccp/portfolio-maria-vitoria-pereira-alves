# Relatório de Desenvolvimento: Análise de Microclima e Simulação de Evacuação

Este repositório contém dois sistemas distintos desenvolvidos em Python que utilizam lógica de processamento de dados e máquinas de estados para resolver problemas de análise ambiental e navegação estratégica.

---

## 1. Analisador de Microclima Urbano

### Descrição do Projeto
Este algoritmo processa dados ambientais de diferentes localidades urbanas para determinar o índice de conforto e a qualidade do ar. O sistema utiliza uma estrutura de dados matricial para armazenar informações de temperatura, umidade e Índice de Qualidade do Ar (IQA).

### Detalhes Técnicos e Funcionalidades
* **Processamento de Matrizes**: O script itera sobre listas aninhadas contendo dados reais de bairros como Largo de São Mateus, Vila Aricanduva e Vila Carrão.
* **Classificação de Qualidade do Ar (IQA)**: Utiliza a estrutura `match-case` para categorizar a qualidade do ar entre Boa, Moderada, Ruim ou Muito Ruim com base em faixas numéricas.
* **Cálculo de Nota de Conforto Urbano**: Implementa um sistema de pontuação decrescente (iniciando em 10) que aplica penalidades baseadas em desvios de faixas ideais:
    * Temperatura ideal: Entre 20°C e 26°C.
    * Umidade ideal: Entre 50% e 70%.
    * Penalidade por poluição: Redução de pontos caso o IQA ultrapasse 50.
* **Relatório Automático**: Exibe para cada localidade os dados brutos, a classificação do ar e a nota final de conforto.

---

## 2. Simulador de Navegação e Evacuação Espacial

### Descrição do Projeto
Este script simula o comportamento de um agente em um cenário de evacuação, onde é necessário navegar entre diferentes compartimentos, gerenciar energia limitada e interagir com objetos do cenário para progredir.

### Detalhes Técnicos e Funcionalidades
* **Máquina de Estados de Navegação**: O agente transita entre estados lógicos (inicio, direita fechada, tem chave, portao trancado, saida) que definem as possibilidades de movimento.
* **Gestão de Inventário**: Implementa um sistema de coleta de itens. O agente só consegue progredir pelo "Portão" se o item "chave" estiver presente na lista de inventário.
* **Logística de Desvio e Backtracking**: 
    * O sistema detecta rotas bloqueadas ("direita fechada") e força o desvio automático.
    * Caso o agente chegue a um bloqueio sem o item necessário, o algoritmo executa um recuo na posição (`posicao -= 1`) para permitir a busca do item.
* **Controle de Recursos Críticos**: Utiliza um laço `while` que monitora a energia do agente. Cada ação consome 1 unidade, estabelecendo o esgotamento de energia como uma condição de falha da simulação.
* **Feedback de Status**: Monitoramento em tempo real do local atual, estado do ambiente, nível de energia restante e itens coletados.

---

## Tecnologias Aplicadas
* Linguagem: Python 3.10 ou superior.
* Estruturas de Dados: Listas, Matrizes e Listas Dinâmicas (Inventário).
* Estruturas de Controle: Loops (`for`, `while`), Condicionais compostas e `match-case`.

[Voltar ao início](https://github.com/mavisccp)
