- Algoritmo de Auditoria de Dados
  
 Descrição do Projeto:
Este projeto consiste em uma ferramenta de monitoramento e auditoria financeira desenvolvida para identificar anomalias em fluxos de vendas.
O objetivo principal é automatizar a detecção de valores atípicos (outliers) e garantir que a média de transações permaneça dentro de parâmetros de segurança pré-estabelecidos.

O sistema analisa entradas de vendas, calcula médias dinâmicas e aciona alertas de "Quarentena" ou "Revisão Manual" caso detecte desvios significativos (como uma venda individual ser 500% superior à média atual). 
Além disso, o algoritmo possui uma lógica de ajuste adaptativo, atualizando o limite de segurança com base no comportamento real dos dados processados.

Figura 1: Fluxo lógico do algoritmo de detecção de anomalias e ajuste de limites.

 Tecnologias Utilizadas
 Linguagem: Python 3.x
 
 Ambiente de Desenvolvimento: Google Colab / Local Python Environment
 
 Paradigma: Programação Estruturada e Lógica Condicional
 
Funcionalidades e Regras de Negócio:
O algoritmo opera sob três pilares fundamentais de auditoria:

Monitoramento de Média Global: Se a média das vendas atuais ultrapassar o LIMITE_SEGURANCA (inicialmente definido como 100.000), o sistema entra em estado de Quarentena.

Detecção de Outliers: O sistema compara cada venda individual com a média calculada. Se uma única venda for maior que $5 \times$ a média, uma Revisão Manual é solicitada imediatamente.

Atualização Dinâmica: O limite de segurança não é estático; ele é reajustado automaticamente para a média da última operação, permitindo que o sistema aprenda o volume transacional atual.

Figura 2: Exemplo de interface de monitoramento e alertas de revisão.

Como Executar:
Certifique-se de ter o Python instalado em sua máquina ou utilize o Google Colab.

Clone este repositório ou baixe o arquivo projeto_algoritmo_de_auditoria_de_dados.py.

Execute o script:Bashpython projeto_algoritmo_de_auditoria_de_dados.py

Insira os valores das três vendas solicitadas no console para visualizar o relatório de auditoria.


[Voltar ao início](https://github.com/mavisccp)
