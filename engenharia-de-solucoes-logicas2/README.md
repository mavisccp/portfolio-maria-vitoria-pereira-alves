 Sistema de Triagem de Saúde (Pseudocódigo e Fluxograma)

 Descrição do Projeto
Este projeto apresenta um sistema de triagem lógica para classificação de risco de saúde, representado através de um fluxograma e de um pseudocódigo correspondente. O objetivo é receber parâmetros vitais básicos de um paciente e categorizar o nível de risco em três níveis coloridos (Vermelho, Amarelo e Verde).

O sistema processa as seguintes entradas: Pressão Arterial, Batimentos por Minuto (BPM) e Temperatura Corporal. Com base nessas informações, aplica regras condicionais para determinar a gravidade da situação.

Figura 1: Fluxograma manuscrito detalhando a lógica do sistema de triagem.

 Tecnologias e Conceitos
Lógica de Programação: Estruturas condicionais aninhadas (Se/Então/Senão).

Representação Algorítmica: Uso de fluxogramas (diagramas de bloco) e pseudocódigo.

Conceitos de Saúde: Implementação de regras de negócio simples para parâmetros de saúde (hipertensão, taquicardia, febre).

 Pseudocódigo Corrigido e Otimizado
Abaixo está o pseudocódigo que representa fielmente a lógica do fluxograma apresentado na imagem. O código original foi ajustado para corrigir erros de sintaxe (como a falta de operadores lógicos e estruturas de controle completas) e para garantir que todas as variáveis fossem devidamente declaradas e utilizadas.

Delphi

programa sistema_triagem_saude
var
    temperatura, bpm, pressao : Real
    pessoa_idosa : Logico

inicio

    Escreva("Digite a pressão (valor numérico): ")
    Leia(pressao)
    Escreva("Digite o BPM: ")
    Leia(bpm)
    Escreva("Digite a temperatura: ")
    Leia(temperatura)
    Escreva("A pessoa é maior de 60 anos? (Sim=Verdadeiro, Não=Falso): ")
    Leia(pessoa_idosa)

    Se (pressao >= 140) OU (bpm >= 160) Entao
        Se (pessoa_idosa = Verdadeiro) Entao
            Escreva("Risco: Vermelho")
        Senao
            Escreva("Risco: Amarelo")
        Fimse
    Senao
        Se (temperatura >= 38) Entao
            Escreva("Risco: Amarelo")
        Senao
            Escreva("Risco: Verde")
        Fimse
    Fimse
Fim

[Voltar ao início](https://github.com/mavisccp)
