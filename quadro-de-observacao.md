# Quadro de observação

## Referências analisadas

1. **IBM Developer**: [Train a software agent to behave rationally with reinforcement learning](https://developer.ibm.com/articles/cc-reinforcement-learning-train-software-agent/), de M. Tim Jones (estilo: didático corporativo).
2. **Real Python**: [Python AI: How to Build a Neural Network & Make Predictions](https://realpython.com/python-ai-neural-network/), de Déborah Mesquita (estilo: tutorial com código).

## O que observamos

| Elemento | IBM Developer | Real Python |
|---|---|---|
| Título e abertura | Título com subtítulo explicativo; autor logo no topo. | Título direto; autor, data de atualização, tempo de leitura e nível (intermediário) no topo. |
| Introdução | Define aprendizado por reforço e cita um caso real (o jogador de gamão TD-Gammon, de 1992). | Motivação curta e uma lista explícita do que o leitor vai aprender; avisa com honestidade que em produção se usam bibliotecas prontas. |
| Seções e índice | Índice quase vazio; seções de comparação com outros tipos de ML, história, Q-learning, implementação e "indo além". | Índice completo e navegável, com subtítulos descritivos que formam um roteiro do tutorial. |
| Exemplos | Grade 20×20 com obstáculos e um objetivo, próxima do nosso FrozenLake. | Vários exemplos do cotidiano antes da teoria: sudoku, arremesso de dardos (analogia para tentativa e erro), preço de imóveis. |
| Figuras | Quatro diagramas com texto alternativo, mas sem legenda; a fórmula aparece como imagem. | Cada figura tem legenda e texto alternativo e explica uma única ideia; fórmula também como imagem. |
| Código | Em C, comentado, em trechos; código completo no GitHub; mostra a saída do programa. | Em Python, blocos curtos que avançam junto com o texto, saídas visíveis e explicação linha a linha do bloco mais longo; ensina a preparar o ambiente. Não fixa versões das bibliotecas. |
| Termos técnicos | Explicados no texto (taxa de aprendizado, fator de desconto). | Em negrito na primeira aparição, com definição logo em seguida; notas destacadas em caixas. |
| Limitações | Menciona brevemente que estados não explorados ficam sem valor. | Discute overfitting e explica por que o exemplo não serve para produção. |
| Fechamento | Seção "indo além" com algoritmos relacionados; data e tempo de leitura no final. | Conclusão retoma a lista do que foi aprendido; leituras recomendadas, quiz e cartão do autor com foto e bio. |
| Referências | Sem lista de referências; links principalmente para outras páginas da IBM. | Sem lista formal; links ao longo do texto e em "leituras recomendadas". |

## Três decisões do grupo

1. **Vamos abrir com um problema real e dizer o que o leitor vai aprender, porque** o Real Python faz isso e o leitor sabe desde o início aonde vai chegar. A IBM abre com uma definição, que é menos convidativa para quem está começando.

2. **Vamos mostrar a intuição e o exemplo antes da fórmula, e colocar a fórmula em texto dentro de uma caixa de aprofundamento, porque** nosso público tem pouca base em matemática. As duas referências mostram fórmulas como imagem, que não pode ser copiada nem é lida por leitores de tela.

3. **Vamos usar código em Python, em blocos curtos e comentados, com as versões das bibliotecas e um notebook completo à parte, porque** o Real Python mostra que blocos curtos acompanham melhor a explicação, enquanto a IBM usa C, menos familiar para o nosso público. Registramos as versões porque nenhuma das referências faz isso, e as bibliotecas de aprendizado por reforço mudaram nos últimos anos (o Gym virou Gymnasium).

## Uma coisa que decidimos não fazer

**Não vamos implementar o DQN nem outros métodos de aprendizado por reforço profundo, apenas citá-los na seção de limitações.** Eles exigem redes neurais, mais tempo de treino e mais base matemática do que cabe em 15 minutos de apresentação e no nosso público. Preferimos explicar bem um algoritmo a cobrir vários superficialmente.
