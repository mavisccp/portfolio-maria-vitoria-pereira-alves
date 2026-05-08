# Algoritmo CaixaMercado: Sistema de Vendas e Cálculo de Troco Otimizado

## Descrição do Projeto
Este projeto apresenta o desenvolvimento de um algoritmo para simular a operação de um caixa de supermercado. O sistema gerencia o registro de produtos, calcula o total da compra, permite a aplicação de descontos e finaliza a transação com o cálculo detalhado do troco.

O projeto foi documentado através de fluxogramas para a modelagem visual da lógica e pseudocódigo (Portugol) para a estruturação detalhada do algoritmo.

### Funcionalidades Principais
* Registro de Produtos: Permite a entrada de valores de produtos até que um valor zero seja inserido para encerrar a compra.
* Cálculo do Total: Soma automaticamente o valor de todos os produtos registrados no laço de repetição.
* Aplicação de Desconto: Oferece a opção de aplicar um valor de desconto ao total da compra caso o usuário selecione a opção correspondente.
* Validação de Pagamento: Verifica se o valor entregue pelo cliente é suficiente para cobrir o valor final.
* Cálculo de Troco Detalhado: Calcula a quantidade exata de cédulas de R$ 100, R$ 50, R$ 10, R$ 5 e R$ 1 necessárias para compor o troco de forma otimizada.

## Estrutura do Projeto
O projeto está estruturado em duas frentes de documentação técnica conforme os arquivos modularizacao1.jpg, modularizacao2.jpg, modularizacao3.jpg, modularizacao4.jpg e modularizacao5.jpg:

### 1. Modelagem Lógica
Os fluxogramas detalham o fluxo do sistema, incluindo o registro e soma de produtos, a decisão condicional para descontos e a lógica sequencial para a separação das notas do troco.

### 2. Pseudocódigo
O algoritmo foi estruturado em Portugol, utilizando os seguintes elementos técnicos:
* Variáveis: Declaração de inteiros para produtos, totais, descontos, valores entregues e quantidades de notas.
* Estruturas de Controle: Uso de "Enquanto" para o loop de produtos e "Se/Senao" para decisões de pagamento e desconto.
* Operadores Aritméticos: Emprego de DIV (divisão inteira) e MOD (resto da divisão) para isolar a quantidade de cada nota no troco.

## Resultados e Aprendizados
Com base nas notas de auditoria do projeto presentes no arquivo modularizacao3.jpg:
* Redução de Complexidade: Foi utilizada uma divisão por etapas para desenvolver o cálculo do troco de forma lógica.
* Aplicação de Operadores: O uso de DIV e MOD foi essencial para garantir a continuidade dos cálculos das notas até que o valor do troco fosse zerado.
* Identificação de Melhorias: Foi anotada a importância de declarar as variáveis de forma mais precisa no fluxograma para alinhar com o código.
* Adaptação Lógica: O projeto migrou de uma ideia inicial de laços de repetição para uma estrutura condicional sequencial para o troco, visando maior clareza na execução.

## Como Executar
1. Analise a lógica de fluxo no arquivo modularizacao1.jpg e modularizacao2.jpg.
2. Siga a estrutura de dados e as condicionais descritas no pseudocódigo dos arquivos modularizacao5.jpg e modularizacao4.jpg.
3. Utilize os operadores de divisão inteira e resto conforme demonstrado no arquivo modularizacao4.jpg para replicar a lógica de distribuição de cédulas.

---
[Voltar ao início](https://github.com/mavisccp)
