# 🏢 Auditoria de Orçamentos Corporativos (Python)
 
[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)
[![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)]()
 
## 📖 Sobre o Projeto
Este projeto foi desenvolvido como parte da disciplina de Programação de Computadores do curso de Analise e Desenvolvimento de sistemas. O objetivo do script é processar e calcular o orçamento de uma estrutura organizacional complexa (dicionários aninhados) de uma multinacional, aplicando regras de negócio dinâmicas e auditoria de execução.
 
A solução foi arquitetada utilizando conceitos avançados de Python para garantir flexibilidade, performance e rastreabilidade.
 
## 🚀 Funcionalidades
- **Cálculo Hierárquico:** Varredura completa da estrutura corporativa, independentemente do nível de profundidade.
- **Filtros Dinâmicos:** Capacidade de ignorar setores específicos e todos os seus subsetores na hora do cálculo financeiro.
- **Conversão de Câmbio:** Suporte a parâmetros opcionais para conversão de moedas em tempo de execução.
- **Sistema de Auditoria:** Monitoramento automatizado de tempo de execução e registro (logging) dos parâmetros utilizados na transação financeira.
 
## 🛠️ Tecnologias e Conceitos Aplicados
Este projeto foi construído utilizando Python puro (Standard Library), com foco nos seguintes paradigmas e recursos:
* **Funções Recursivas (Recursion):** Utilizadas para a navegação na árvore de dados (dicionários aninhados).
* **Decorators:** Implementação do `@auditor` para injetar comportamentos de log e cronometragem sem modificar a lógica de negócios.
* **Empacotamento de Argumentos (`*args` e `**kwargs`):** Utilizados tanto no decorator quanto na função principal para permitir a passagem dinâmica de departamentos a serem ignorados e taxas de câmbio.
 
## ⚙️ Como Executar
 
### Pré-requisitos
* Python 3.8 ou superior instalado.
 
### Passo a Passo
1. Clone este repositório:
   ```bash
   git clone https://github.com/mavisccp/portfolio-maria-vitoria-pereira-alves/tree/main/sistema_de_auditoria_de_recursos_corporativos.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd sistema_de_auditoria_de_recursos_corporativos
   ```
3. Execute o script principal:
   ```bash
   python main.py
   ```
 
## 🧠 Lógica e Estrutura do Código
Breve explicação de como o código foi organizado:
* `Montei a recursão para que o código conseguisse navegar por todas as camadas da empresa de forma automática: se o programa encontra um novo grupo de dados (um sub-departamento), ele entra nele e repete a mesma lógica de busca.
* Se ele encontra um número, ele adiciona ao total acumulado. Já o decorator eu usei para separar a parte dos logs e do cronômetro. Acoplei ele por "fora" da função para que as mensagens de auditoria e a contagem de tempo apareçam apenas uma vez, no início e no fim,
* deixando o cálculo interno livre de interrupções.`.
* **Dados:** Os dados simulados da empresa foram estruturados em níveis, onde um setor pode ter outros setores (como funções especificas) dentro dele. Usei nomes para identificar cada área e valores numéricos para os orçamentos finais.
* Essa organização permite que o script percorra caminhos curtos ou longos de acordo com setor e departamentos especificos e encontre todos os valores espalhados pela estrutura, independente da quantidade.`.
 
## 👤 Autor
 
* **Maria Vitoria Pereira Alves** * LinkedIn: (https://br.linkedin.com/in/maria-vit%C3%B3ria-94149a213)
* E-mail: mariavitoria_s2_@hotmail.com
 
---
*Projeto acadêmico com foco na aplicação prática de conceitos avançados da linguagem Python.*

[Voltar ao início](https://github.com/mavisccp)
