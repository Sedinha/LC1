1. O que são Fórmulas?
Uma fórmula, na linguagem da lógica, é o análogo de uma proposição em linguagem natural, sendo o "portador" de verdade ou falsidade em nosso sistema formal. Pense nelas como as "sentenças declarativas" que podem ser qualificadas como verdadeiras (V) ou falsas (F), mas nunca ambas ao mesmo tempo.
As fórmulas são construídas de forma indutiva (ou recursiva) a partir de um conjunto de regras:
• Proposições Atômicas (ou Fórmulas Atômicas): São as sentenças mais simples, que não podem ser decompostas em proposições menores conectadas por operadores lógicos. Elas são representadas por letras sentenciais (ou variáveis proposicionais), geralmente minúsculas, como p, q, r, s, .... No contexto da Lógica de Predicados, estas seriam predicados com aridade zero.
• Proposições Compostas (ou Fórmulas Moleculares): São sentenças formadas pela combinação de uma ou mais proposições atômicas utilizando operadores lógicos (ou conectivos). Os cinco operadores verofuncionais principais são:
    1. Negação (¬): Um operador unário que inverte o valor-verdade de uma proposição. Se H é uma fórmula, então (¬H) é uma fórmula.
    2. Disjunção (∨): Representa o "ou" inclusivo. Se H e G são fórmulas, então (H ∨ G) é uma fórmula.
    3. Conjunção (∧): Representa o "e". Se H e G são fórmulas, então (H ∧ G) é uma fórmula.
    4. Implicação (→): Representa "se... então...". Se H e G são fórmulas, então (H → G) é uma fórmula, onde H é o antecedente e G é o consequente.
    5. Equivalência (↔): Representa "se, e somente se" (bicondicional). Se H e G são fórmulas, então (H ↔ G) é uma fórmula.
É crucial a utilização de parênteses para evitar ambiguidades na estrutura das fórmulas, tal como na expressão ¬(p → q) versus (¬p → q).
Exemplo Prático de Construção de Fórmulas: Vamos construir a fórmula (P → Q) ∧ (Q ∨ R):
1. Pela regra 1, P, Q, R são fórmulas (proposições atômicas).
2. Pela regra 5 (implicação), (P → Q) é uma fórmula.
3. Pela regra 3 (disjunção), (Q ∨ R) é uma fórmula.
4. Pela regra 4 (conjunção), ((P → Q) ∧ (Q ∨ R)) é uma fórmula.
2. Tabelas-Verdade
As tabelas-verdade são métodos mecânicos para avaliar o valor de verdade de uma fórmula composta. Elas listam todas as possíveis combinações de valores de verdade (Verdadeiro ou Falso) para as proposições atômicas e o valor de verdade resultante para a fórmula completa.
Como Funciona uma Tabela-Verdade:
• Para cada proposição atômica (por exemplo, P, Q), atribuímos todas as combinações possíveis de V e F. Se há n proposições atômicas distintas, haverá 2<sup>n</sup> linhas na tabela.
• As colunas são preenchidas passo a passo, avaliando as subfórmulas mais simples primeiro, até chegar à fórmula principal.
Exemplo Prático de Tabela-Verdade para P → Q: | P | Q | P → Q | | :-: | :-: | :-----: | | V | V | V | | V | F | F | | F | V | V | | F | F | V |
Importante: Na Lógica de Predicados, nem sempre é possível usar tabelas-verdade diretamente, especialmente com quantificadores e domínios infinitos, pois não há como preencher as colunas com T ou F de forma exaustiva.
--------------------------------------------------------------------------------
II. Função Interpretação e Definição de Verdade
Entender como as fórmulas ganham significado é a essência da semântica.
1. A Função Interpretação (I)
A interpretação I é uma função binária total que associa valores de verdade (Verdadeiro ou Falso) a cada elemento sintático da linguagem.
• Domínio: O conjunto de todas as fórmulas bem-formadas da Lógica Proposicional.
• Contradomínio: O conjunto {T, F} (Verdadeiro, Falso).
As regras para a função interpretação são as seguintes:
1. Para cada símbolo proposicional P, I[P] é T ou F (Princípio da Bivalência ou Terceiro Excluído).
2. Se H é uma fórmula: I[¬H] = T se e somente se I[H] = F; caso contrário, I[¬H] = F.
3. Se H e G são fórmulas: I[(H ∨ G)] = T se e somente se I[H] = T ou I[G] = T; caso contrário, I[(H ∨ G)] = F.
4. Se H e G são fórmulas: I[(H ∧ G)] = T se e somente se I[H] = T e I[G] = T; caso contrário, I[(H ∧ G)] = F.
5. Se H e G são fórmulas: I[(H → G)] = T se e somente se I[H] = F ou I[G] = T; caso contrário, I[(H → G)] = F.
6. Se H e G são fórmulas: I[(H ↔ G)] = T se e somente se I[H] = I[G]; caso contrário, I[(H ↔ G)] = F.
Exemplo Prático de Interpretação: Considere uma interpretação I onde I[P] = T, I[Q] = F, I[R] = T, I[S] = F. Então:
• I[¬P] = F
• I[P ∨ Q] = T (porque I[P] = T)
• I[P ∧ Q] = F (porque I[Q] = F)
• I[S → R] = T (porque I[S] = F, o antecedente é falso, tornando a implicação verdadeira).
2. Princípio da Composicionalidade e Definição de Verdade
Um conceito fundamental na Lógica é a distinção entre objetos sintáticos (os símbolos e fórmulas) e sua interpretação (o significado). Na LP, essa distinção é clara: a interpretação de uma fórmula depende da interpretação de suas partes constituintes e da forma como essas partes se combinam. Isso é conhecido como o Princípio da Composicionalidade. Os conectivos são, portanto, funções de verdade, cujo valor pode ser calculado a partir dos valores de verdade de suas subfórmulas.
A definição de verdade na Lógica Proposicional Clássica é a seguinte: Uma fórmula H é verdadeira em uma determinada interpretação I se e somente se o resultado da aplicação da função interpretação I na fórmula H for verdadeiro, ou seja, I[H] = T.
É crucial notar que a verdade de uma fórmula é relativa a uma interpretação. A definição de "verdade" pode variar em lógicas não-clássicas (como a Lógica Intuicionista ou Lógicas Multivalentes).
--------------------------------------------------------------------------------
III. Tautologia, Contradição e Contingência
Essas são propriedades semânticas que classificam as fórmulas com base em seus valores de verdade em todas as possíveis interpretações.
1. Tautologia
Uma fórmula H é uma tautologia se, e somente se, para toda interpretação I, I[H] = T. Isso significa que a fórmula é sempre verdadeira, independentemente dos valores de verdade de suas proposições atômicas. Na tabela-verdade, a coluna da fórmula principal conterá apenas o valor V (ou T).
Exemplo Prático: A Lei do Terceiro Excluído: (P ∨ ¬P). | P | ¬P | P ∨ ¬P | | :-: | :--: | :-----: | | V | F | V | | F | V | V | Independentemente de P ser verdadeiro ou falso, (P ∨ ¬P) é sempre verdadeiro.
2. Contradição
Uma fórmula H é uma contradição semântica se, e somente se, para toda interpretação I, I[H] = F. A fórmula é sempre falsa, independentemente dos valores de verdade de suas proposições atômicas. Na tabela-verdade, a coluna da fórmula principal conterá apenas o valor F. Uma propriedade interessante é que, se H é contraditória, então ¬H é uma tautologia.
Exemplo Prático: A Lei da Não Contradição (em sua forma negativa): (P ∧ ¬P). | P | ¬P | P ∧ ¬P | | :-: | :--: | :-----: | | V | F | F | | F | V | F | Independentemente de P ser verdadeiro ou falso, (P ∧ ¬P) é sempre falso.
3. Contingência
Uma fórmula H é uma contingência se, e somente se, existem interpretações I e J, tais que I[H] = T e J[H] = F. Isso significa que a fórmula pode ser verdadeira em algumas situações e falsa em outras, dependendo da interpretação. Na tabela-verdade, a coluna da fórmula principal conterá tanto V quanto F.
Exemplo Prático: Uma implicação simples, como (P → Q). | P | Q | P → Q | | :-: | :-: | :-----: | | V | V | V | | V | F | F | | F | V | V | | F | F | V | Aqui, (P → Q) é verdadeira em algumas linhas e falsa em outras, caracterizando-a como uma contingência.
--------------------------------------------------------------------------------
Relações Importantes:
• Se uma fórmula é uma tautologia, ela é, por definição, satisfatível (existe pelo menos uma interpretação que a torna verdadeira). O inverso, porém, não é verdadeiro: uma fórmula satisfatível não é necessariamente uma tautologia.
• Se uma fórmula é uma contingência, ela é satisfatível.
• Uma tautologia não é uma contingência.
• Uma contradição não é satisfatível.
Esses conceitos são fundamentais para a avaliação de argumentos lógicos. Um argumento é considerado "bom" ou "correto" se suas premissas, quando verdadeiras, justificam a conclusão. A análise de um argumento, na Lógica Proposicional, é frequentemente reduzida a verificar se a implicação (premissas → conclusão) é uma tautologia