Matematica Discreta
Proposição (Sentenças Declarativas)
Proposições são sentenças utilizadas para declarar fatos, é uma sentença declarativa se é V ou F.
Representação simbólica
São utilizadas letras para representar variáveis proposicionais[variáveis declarativas] ou seja, variáveis capazes de representar proposições
As letras convencionais utilizadas para representar variáveis proposicionais, em geral, são: p, q, r, s, . . .
os valores-verdade ou valores lógicos de cada proposição (V ou F)
operadores lógicos (∧, ∨, ⊕, →, ↔, ¬) são utilizados para construção de proposições compostas
Conectivos (Operadores) Lógicos
“e”, “ou”, “não”, “se . . . então”
Permitem combinar proposições simples em proposições mais complexas.
Proposições que não podem ser decompostas em proposições menores, ligadas por conectivos lógicos é dita uma proposição simples ou atômica
Negação [¬]
A negação (¬) é um operador unário que inverte o valor-verdade de uma proposição.
• seja p uma proposição, a negação de p é denotado por ¬p
• a proposição ¬p é lida como “não p”

CONJUNÇÃO: [∧]

| p | q | p ∧ q |
|---|---|-------|
| V | V | V     |
| V | F | F     |
| F | V | F     |
| F | F | F     |
DISJUNÇÃO: [∨]
• seja p e q proposições, a disjunção de p e q, denotada por p ∨ q, é a proposição “p ou q”.
• a disjunção (p ∨ q) tem valor-verdade F quando ambos p e q forem F, caso contrário terá valor V
```
| p | q | p ∨ q |
|---|---|-------|
| V | V | V     |
| V | F | V     |
| F | V | V     |
| F | F | F     |
```
DISJUNÇÃO EXCLUSIVA: [⊕]
Seja p e q proposições, a disjunção exclusiva de p e q, denotada por p ⊕ q, é a proposição “p ou exclusivo q”
• a disjunção exclusiva (p ⊕ q) tem valor-verdade V quando apenas uma das proposições entre p e q forem V, mas não ambas, caso contrário terá valor F
```
| p | q | p ⊕ q |
|---|---|-------|
| V | V | F     |
| V | F | V     |
| F | V | V     |
| F | F | F     |
```
CONDICIONAL: [p → q] ([p ⊆ q])
Sejam p e q proposições.
• “Se p então q” (ou p implica em q) é representado por p → q
• p é chamado de hipótese e q é chamado de tese
Emprego correto do necessário e suficiente
Dada a preposição condicional p → q, p é condição suficiente para q e q é condição necessária para p.
Considere a seguinte correspondência:
• João é Mineiro
• João é Brasileiro
Se p:João é mineiro, então q:João é brasileiro:
• p:João ser mineiro é condição suficiente para que q:João seja brasileiro
• João não precisa ser mineiro para ser brasileiro, poderia ser paulista...
Ou seja, é suficiente que João seja mineiro para que ele possa ser brasileiro,mas não necessário.
• q:João ser brasileiro é condição necessária para que p:João seja mineiro
• João não pode ser mineiro sem ser brasileiro
ou seja, é necessário que João seja brasileiro para que ele possa ser mineiro
```
| p | q | p → q |
|---|---|-------|
| V | V | V     |
| V | F | F     |
| F | V | V     |
| F | F | V     |
```
OBS:
• “Se p então q” (ou p implica em q) é representado por p → q
• ![[250505_13h55m47s_screenshot.png]]
BICONDICIONAL: [p ↔ q]
Seja p e q proposições, a bicondição de p e q, denotada por p ↔ q, é a proposição “p se e somente se q.
```
| p | q | p ↔ q |
|---|---|-------|
| V | V | V     |
| V | F | F     |
| F | V | F     |
| F | F | V     |
```
Tautologia e Contradição
```
| p   | ¬p  | p ∨ ¬p | p ∧ ¬p |
|-----|-----|--------|--------|
| V   | F   | V      | F      |
| F   | V   | V      | F      |
```
Tautologia
Tautologia: ocorre quando uma proposição composta possui valores-verdade sempre V, independentemente dos valores-verdade de suas proposições atômicas
• a notação p ≡ q denota equivalência lógica
Contradição
ocorre quando uma proposição composta possui valores-verdade sempre F, independentemente dos valores-verdade de suas proposições atômicas
PRECEDÊNCIA DE OPERADORES LÓGICOS
operadores lógicos também possuem sua precedência,assim como operadores matemáticos, pondendo ser claramente destacadas por () e [].
A ordem de precedência são, respectivamente em ordem:
1. ¬
2. ∧
3. ∨, ⊕
4. →
5. ↔