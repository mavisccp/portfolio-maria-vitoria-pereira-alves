

## Descrição do Projeto
Este repositório reúne uma coleção de algoritmos desenvolvidos em Python voltados para a automação de tarefas cotidianas e análise de dados em quatro áreas distintas: varejo, monitoramento climático, educação e finanças pessoais. Cada script foi projetado para interagir com o usuário, processar entradas lógicas e aplicar regras de negócio específicas para gerar relatórios e alertas automáticos.

## Tecnologias Utilizadas
* Linguagem: Python 3.x
* Paradigma: Programação Estruturada e Funcional
* Interface: Interface de Linha de Comando (CLI)

## Funcionalidades e Scripts

### 1. Processamento de Vendas e Descontos (Código 1)
Algoritmo para gestão de PDV (Ponto de Venda) que automatiza o cálculo de subtotais e aplicação de descontos progressivos.
* Registro de múltiplos produtos com validação de preços e quantidades.
* Regra de Desconto: Aplica 10% de desconto para compras acima de R$ 500,00 e 5% para compras acima de R$ 200,00.
* Relatório final com contagem total de itens e valor líquido a pagar.

### 2. Analisador Climático Semanal (Código 2)
Ferramenta de monitoramento ambiental para processamento de dados térmicos.
* Cálculo da média de temperatura em um período de 7 dias.
* Detecção de dias quentes (acima de 35°C).
* Sistema de Alerta Extremo: Aciona aviso de perigo para temperaturas fora da margem de segurança (abaixo de -5°C ou acima de 45°C).

### 3. Gestão de Notas Acadêmicas (Código 3)
Sistema para controle de desempenho escolar de turmas.
* Processamento individualizado por aluno com cálculo de média aritmética simples.
* Classificação Automática: Define o status do aluno entre "Aprovado" (Média >= 7.0), "Recuperação" (Média >= 5.0) ou "Reprovado".

### 4. Simulador de Investimentos e Poupança (Código 4)
Calculadora financeira para projeção de rendimentos com juros compostos.
* Simulação baseada em saldo inicial, taxa de juros mensal e aportes variáveis.
* Monitoramento de Metas: Notifica o usuário automaticamente ao atingir o marco de R$ 10.000,00 acumulados.
* Demonstrativo mensal de evolução patrimonial.

## Resultados e Aprendizados
O desenvolvimento deste pacote de scripts permitiu consolidar conhecimentos fundamentais em:
* Estruturas de Repetição: Uso de laços `for` e `range` para processamento de listas e períodos de tempo.
* Lógica Condicional: Implementação de múltiplos níveis de decisão com `if`, `elif` e `else`.
* Tratamento de Dados: Manipulação de tipos de entrada (float, int, str) e formatação de saídas numéricas para o padrão monetário e decimal.
* Monitoramento de Flags: Uso de variáveis booleanas para controle de alertas de segurança e metas.

## Como Executar
1. Certifique-se de ter o Python 3 instalado.
2. Cada funcionalidade pode ser executada chamando sua respectiva função dentro do arquivo principal:
   * Para vendas: `processar_vendas()`
   * Para clima: `analisar_clima()`
   * Para notas: `sistema_notas_turma()`
   * Para poupança: `simulador_poupanca()`
3. Siga as instruções que aparecerão no terminal para inserir os dados solicitados.

---
[Voltar ao início](https://github.com/seu-usuario/seu-repositorio)
