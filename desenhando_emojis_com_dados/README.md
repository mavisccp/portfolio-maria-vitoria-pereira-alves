

## 1. Processamento de Matriz de Pixels (Emoji Data)

### Descrição do Projeto
Este algoritmo simula um editor de imagens básico que atua diretamente na grade de cores de um ícone digital. O objetivo é realizar um ajuste de luminosidade (escurecimento) em pixels específicos de um emoji representado por uma matriz RGB.

### Detalhes Técnicos
* **Manipulação de Cores**: O script percorre uma grade de 5x5 pixels. Cada pixel é uma tupla `(R, G, B)`.
* **Lógica de Filtro**: Identifica pixels de cor amarela `(255, 255, 0)` e aplica uma operação de divisão inteira (`//2`) em cada canal, reduzindo o brilho pela metade.
* **Preservação de Dados**: Pixels que não correspondem à cor alvo (como os olhos e boca pretos) permanecem inalterados, preservando o design original.

---

## 2. Transposição de Matrizes Musicais

### Descrição do Projeto
Este script foca na reestruturação de dados de frequências sonoras armazenadas em uma biblioteca musical. O algoritmo realiza a transposição de matrizes de frequências associadas a diferentes estados emocionais ("Alegre" e "Triste").

### Detalhes Técnicos
* **Estrutura Aninhada**: Manipula uma lista de dicionários onde as chaves são os estados e os valores são matrizes de frequências.
* **Algoritmo de Transposição**: O código reconfigura as listas originais, trocando as posições de linhas por colunas dentro de uma estrutura de tuplas fixa.
* **Atualização Dinâmica**: Utiliza o método `.update()` para sobrescrever os dados antigos com a nova estrutura transposta, mantendo a integridade da biblioteca musical.

---

## 3. Curadoria e Tratamento de Galeria Digital

### Descrição do Projeto
Um sistema de gerenciamento de metadados para uma galeria de artes digitais. O algoritmo foca na limpeza de atributos temporários e na organização hierárquica das obras de arte.

### Detalhes Técnicos
* **Iteração e Inspeção**: Percorre a galeria para extrair e exibir os valores de cada pixel individual das obras cadastradas.
* **Limpeza de Metadados**: Utiliza o método `.pop()` para remover tags temporárias ("temp") que não devem constar na versão final do banco de dados.
* **Gestão de Inventário**: Emprega o método `.insert(0, ...)` para adicionar um novo elemento de "Capa" no início da lista, demonstrando controle sobre a indexação e priorização de elementos na galeria.

---

## Tecnologias e Conceitos Aplicados
* **Estruturas de Dados**: Dicionários, Listas e Tuplas imutáveis.
* **Operações de Coleção**: Métodos como `.items()`, `.keys()`, `.pop()`, `.append()` e `.insert()`.
* **Lógica de Programação**: Laços de repetição aninhados, condicionais e aritmética de pixels.

[Voltar ao início](https://github.com/mavisccp)
