--------------------------------------------------------------------------------

1. Consequência Sintática e Semântica

Neste domínio da Lógica, é crucial entender como a verdade de uma proposição pode ser "herdada" de outras, tanto por sua forma (sintaxe) quanto por seu significado (semântica).

1.1. Consequência Lógica Sintática (β ⊢ α)

A consequência lógica sintática, denotada por β ⊢ α, estabelece que a fórmula α pode ser provada a partir de um conjunto de fórmulas β (denominadas hipóteses ou premissas). Uma prova, neste contexto, é uma sequência de fórmulas onde cada passo é um axioma, uma hipótese de β, ou é derivado de fórmulas anteriores na sequência por meio de regras de inferência. O conceito de verdade não é diretamente manipulado aqui; trata-se de um procedimento puramente formal e mecânico.

1.2. Consequência Lógica Semântica (β ⊨ α)

A consequência lógica semântica, denotada por β ⊨ α, significa que toda e qualquer interpretação (I) que torna todas as fórmulas do conjunto β verdadeiras, também torna a fórmula α verdadeira. Em outras palavras, não existe uma situação (interpretação) em que todas as premissas de β são verdadeiras e α é falsa. Este conceito lida diretamente com o significado ou interpretação das fórmulas.

1.3. Diferenças e Relações

A principal diferença reside na natureza dos conceitos: sintático refere-se à forma e às regras de manipulação de símbolos, enquanto semântico refere-se ao significado e aos valores de verdade.

Na Lógica Proposicional, o que é fascinante é a equivalência entre esses dois conceitos, garantida por dois teoremas fundamentais:

• Teorema da Correção: Se β ⊢ α, então β ⊨ α. Isso significa que um sistema de prova "correto" (como o ℘a ou os tablôs semânticos) não deduz nada que seja semanticamente falso a partir de premissas verdadeiras.

• Teorema da Completude: Se β ⊨ α, então β ⊢ α. Isso garante que, se algo é semanticamente uma consequência (sempre verdadeiro sob certas condições), nosso sistema de prova é "completo" o suficiente para demonstrá-lo sintaticamente.

Essa bi-implicação (β ⊢ α se, e somente se, β ⊨ α) na Lógica Proposicional significa que podemos usar tanto métodos sintáticos (provas) quanto semânticos (tabelas-verdade, tablôs semânticos) para verificar a consequência lógica.

1.4. Associação com Tablôs Semânticos para Consequência Semântica

Os tablôs semânticos são uma ferramenta semântica poderosa para verificar a consequência lógica. Para demonstrar que β ⊨ α, onde β = {A1, A2, ..., An}, seguimos os passos:

1. Formular a implicação: Construa a fórmula H = (A1 ∧ A2 ∧ ... ∧ An) → α. Queremos verificar se H é uma tautologia.

2. Negar a fórmula: Formule a negação de H, ou seja, ¬H = ¬((A1 ∧ A2 ∧ ... ∧ An) → α).

3. Construir o tablô: Inicie um tablô semântico com ¬H e aplique as regras de inferência (R1 a R9).

4. Verificar fechamento:

    ◦ Se todos os ramos do tablô se fecharem (ou seja, cada ramo contém uma fórmula A e sua negação ¬A), então ¬H é uma contradição. Isso implica que H é uma tautologia. Logo, β ⊨ α é verdadeiro.

    ◦ Se pelo menos um ramo do tablô permanecer aberto, então ¬H não é uma contradição. Isso significa que H não é uma tautologia. Consequentemente, β ⊨ α é falso.



--------------------------------------------------------------------------------

2. Validade Sintática e Semântica de Argumentos e Fórmulas

Os conceitos de validade nos permitem avaliar a solidez de argumentos e a verdade intrínseca de fórmulas.

2.1. Validade de Argumentos

Um argumento é um conjunto de afirmações (premissas) que são usadas para justificar uma conclusão.

• Validade Sintática de Argumentos: Um argumento é sintaticamente válido se sua conclusão é uma consequência lógica sintática de suas premissas. Isso significa que existe uma prova da conclusão a partir das premissas utilizando as regras de um sistema formal (como o de Dedução Natural).

• Validade Semântica de Argumentos: Um argumento é semanticamente válido se sua conclusão é uma consequência lógica semântica de suas premissas. Isso quer dizer que não há nenhuma interpretação possível em que todas as premissas são verdadeiras e a conclusão é falsa.

2.2. Validade de Fórmulas

Uma fórmula, por si só, pode ter uma propriedade de validade.

• Uma fórmula é logicamente válida (ou uma tautologia) se ela é verdadeira em todas as interpretações possíveis.

2.3. Relações e Esclarecimentos

Na Lógica Proposicional, devido aos teoremas da Correção e Completude, a validade sintática e semântica de um argumento são equivalentes. Portanto, provar um implica o outro.

A validade de um argumento está intrinsecamente ligada à tautologia da fórmula condicional que o representa. Um argumento com premissas A1, ..., An e conclusão H é válido se, e somente se, a fórmula (A1 ∧ ... ∧ An) → H é uma tautologia.

2.4. Associação com Tablôs Semânticos para Validade

Para verificar a validade de um argumento usando tablôs semânticos:

1. Formalize o argumento: Represente as premissas como A1, ..., An e a conclusão como H.

2. Construa a fórmula condicional: Crie a fórmula G = (A1 ∧ ... ∧ An) → H.

3. Verifique se G é uma tautologia:

    ◦ Construa um tablô semântico para ¬G.

    ◦ Se o tablô para ¬G for fechado (todos os ramos se fecham), então G é uma tautologia. Isso significa que o argumento é válido.

    ◦ Se o tablô para ¬G tiver pelo menos um ramo aberto, então G não é uma tautologia, e o argumento é inválido.



--------------------------------------------------------------------------------

3. Relação entre Verdade e Validade

É fundamental distinguir entre "verdade" e "validade", conceitos que frequentemente são confundidos no uso cotidiano, mas que têm significados precisos e distintos em Lógica.

3.1. Verdade

• Definição: A verdade (ou falsidade) é uma propriedade de uma proposição ou fórmula sob uma dada interpretação. Uma proposição atômica, como "João é feliz", pode ser verdadeira ou falsa dependendo do estado do mundo ou da interpretação que lhe é atribuída. Fórmulas complexas têm seu valor de verdade determinado pelas interpretações de suas partes e pela semântica dos conectivos.

• Objeto: Em alguns contextos, "verdadeiro" (V) e "falso" (F) são vistos como os valores que uma função de interpretação atribui às fórmulas.

3.2. Validade

• Definição: A validade é uma propriedade de argumentos ou, em um sentido específico, de fórmulas (quando são tautologias, diz-se que são logicamente válidas). A validade de um argumento diz respeito à sua forma lógica, e não ao conteúdo de suas premissas ou conclusão. Um argumento é válido se a conclusão necessariamente se segue das premissas.

• Independência do Conteúdo: A validade é uma propriedade formal. Por exemplo, o argumento "Se está chovendo, então a rua está molhada. Está chovendo. Logo, a rua está molhada" é válido. O argumento "Se 2 + 2 = 5, então a lua é feita de queijo. 2 + 2 = 5. Logo, a lua é feita de queijo" também é válido, apesar de suas premissas serem falsas e a conclusão ser potencialmente falsa. A forma é a mesma, e essa forma é válida.

3.3. Diferenças Chave e Esclarecimentos

• Proposições são verdadeiras ou falsas; Argumentos são válidos ou inválidos. É um erro dizer que um argumento é "verdadeiro", assim como é um erro dizer que uma proposição é "válida" (a menos que se refira a uma tautologia como "logicamente válida").

• Argumento "Correto" vs. "Bom":

    ◦ Um argumento é correto se suas premissas justificam a conclusão (ou seja, o argumento é semanticamente válido).

    ◦ Um argumento é bom se, além de ser correto, suas premissas são de fato verdadeiras. Um argumento pode ser válido (correto) mas não ser "bom" se suas premissas são falsas.

• Causalidade vs. Implicação Lógica: Na linguagem natural, a implicação "se...então" muitas vezes sugere uma relação de causa e efeito. Na Lógica, o conectivo → (implicação material) não expressa causalidade. A fórmula P → Q é verdadeira se P é falso (independentemente de Q), ou se P e Q são ambos verdadeiros. Isso pode parecer "estranho" ao senso comum, mas é crucial para a consistência matemática.



--------------------------------------------------------------------------------

4. Formalização e Prova

A Lógica Proposicional nos oferece uma linguagem precisa para representar e analisar o raciocínio, eliminando ambiguidades da linguagem natural.

4.1. Formalização

Formalização é o processo de traduzir sentenças da linguagem natural para o formato rigoroso da Lógica Proposicional. Este processo envolve:

1. Identificar Proposições Atômicas: São as sentenças declarativas mais simples, que não podem ser decompostas em partes menores ligadas por conectivos lógicos, e que podem ser classificadas como verdadeiras ou falsas.

    ◦ Exemplo: "Está chovendo" é uma proposição atômica. "José comeu o bolo" é uma proposição atômica; "O bolo foi comido por José" representa a mesma proposição, pois a Lógica se preocupa com o conteúdo e significado, não com a sequência exata das palavras.

2. Representar com Variáveis Proposicionais: Atribua um símbolo proposicional (geralmente letras maiúsculas como P, Q, R, ou minúsculas como p, q, r para variáveis proposicionais) a cada proposição atômica distinta.

    ◦ Exemplo: P = "Está chovendo", Q = "A rua está molhada".

3. Utilizar Conectivos Lógicos: Conectivos são símbolos que combinam proposições simples em proposições mais complexas.

    ◦ ¬ (não): Negação unária. ¬P é lido como "não P".

    ◦ ∧ (e): Conjunção. P ∧ Q é lido como "P e Q".

    ◦ ∨ (ou): Disjunção. P ∨ Q é lido como "P ou Q". Na Lógica Clássica, é uma disjunção inclusiva (pode ser um ou outro, ou ambos).

    ◦ → (se...então): Implicação. P → Q é lido como "Se P, então Q". P é o antecedente, Q é o consequente.

    ◦ ↔ (se, e somente se): Bi-implicação. P ↔ Q é lido como "P se, e somente se, Q".

    ◦ Ordem de Precedência dos Conectivos: Para evitar ambiguidades e omitir parênteses em fórmulas complexas, segue-se uma ordem de precedência:

        1. ¬ (maior precedência)

        2. ∧

        3. ∨, ⊕ (disjunção exclusiva, se usada)

        4. →

        5. ↔ (menor precedência) Exemplo: P → Q ↔ R é lido como (P → Q) ↔ R.

4. Conectar e Estruturar: Use parênteses para agrupar as proposições e conectivos, seguindo a estrutura lógica da sentença original, respeitando a ordem de precedência.

    ◦ Exemplo Prático de Formalização:

        ▪ Sentença: "Se eu sou feliz, então você é feliz."

        ▪ Proposições Atômicas: P = "eu sou feliz", Q = "você é feliz".

        ▪ Fórmula: P → Q.

        ▪ Argumento: "Se está chovendo, então a rua está molhada. Está chovendo. Portanto, a rua está molhada."

        ▪ Formalização: P = "está chovendo", Q = "a rua está molhada". As premissas são P → Q e P. A conclusão é Q. Este argumento tem a forma: (P → Q) ∧ P → Q.

4.2. Prova (Dedução Sintática)

Uma prova sintática, ou derivação, é um procedimento formal para estabelecer que uma fórmula é uma consequência lógica sintática de um conjunto de premissas. Ela é uma sequência de fórmulas, onde cada linha é justificada por um axioma, uma premissa (hipótese), ou pela aplicação de uma regra de inferência a linhas anteriores.

Sistema de Dedução Natural (Moura): Este sistema utiliza regras divididas em introdução (para construir fórmulas com um conectivo) e eliminação (para usar fórmulas com um conectivo).

• Axioma (Ax): φ ⊢ φ. Uma fórmula é uma consequência de si mesma.

• Regra de Eliminação da Implicação (→e) / Modus Ponens (MP):

    ◦ Se temos Γ1 ⊢ φ → ψ e Γ2 ⊢ φ, podemos concluir Γ1 ∪ Γ2 ⊢ ψ.

    ◦ Interpretação: Se temos uma implicação e seu antecedente, podemos concluir o consequente.

• Regra de Introdução da Implicação (→i):

    ◦ Se, ao assumir φ como hipótese temporária, conseguimos provar ψ (Γ, φ ⊢ ψ), então podemos concluir a implicação Γ ⊢ φ → ψ e "descartar" a hipótese φ.

    ◦ Interpretação: Para provar "se φ então ψ", assumimos φ e tentamos provar ψ.

Outras regras (LPM - Lógica Proposicional Minimal):

• Negação: Introdução (¬i) e Eliminação (¬e).

• Conjunção: Introdução (∧i) e Eliminação (∧e1, ∧e2).

• Disjunção: Introdução (∨i1, ∨i2) e Eliminação (∨e).

Exemplo de Construção de Prova Sintática (em árvore, notação padrão com descarte de hipóteses): Prove o sequente φ → ψ, ¬ψ ⊢ ¬φ (Lei do Contrarrecíproco ou Modus Tollens):

[φ]u φ → ψ ¬ψ [φ]u

----- (Ax) -------- (Ax) -------- (Ax)

φ ψ ¬ψ ⊥

----------------- (→e) ----------- (¬e)

⊥

------ (¬i) u

¬φ

Passo a passo:

1. Começamos de baixo para cima. Para provar ¬φ (uma negação), usamos a regra (¬i), assumindo φ como hipótese temporária ([φ]u) e buscando uma contradição ⊥.

2. Agora precisamos provar ⊥ a partir de φ → ψ, ¬ψ e [φ]u.

3. Temos φ → ψ (premissa) e [φ]u (hipótese). Pela regra (→e), podemos deduzir ψ.

4. Temos ψ (acabamos de deduzir) e ¬ψ (premissa). Pela regra (¬e), podemos deduzir ⊥.

5. Atingimos a contradição ⊥. A hipótese [φ]u é descartada pela aplicação de (¬i) e marcamos com o índice u.

4.3. Associação com Tablôs Semânticos para Prova

Embora a prova sintática seja sobre a manipulação de símbolos, os tablôs semânticos oferecem um método de prova que pode ser mecanizado. Para "provar" uma fórmula H (ou um argumento) utilizando tablôs, estamos, na verdade, provando que H é uma tautologia (válida).

• Método: Para provar H (que se assume ser uma tautologia), construímos um tablô semântico a partir de ¬H. Se o tablô fecha, então H é uma tautologia, e consideramos que foi "provada".



--------------------------------------------------------------------------------

5. Invalidade de Argumentos

A invalidade é o oposto da validade e é crucial para identificar falhas no raciocínio.

5.1. Definição Sintática de Invalidade

• Um argumento é sintaticamente inválido se não existe uma prova de sua conclusão a partir de suas premissas.

• Dificuldade: É muito difícil demonstrar a não existência de uma prova. Geralmente, demonstramos a invalidade semanticamente.

5.2. Definição Semântica de Invalidade

• Um argumento é semanticamente inválido se existe pelo menos uma interpretação (I) que torna todas as suas premissas verdadeiras e sua conclusão falsa. Essa interpretação é chamada de contraexemplo.

• Vantagem: Graças aos teoremas da Correção e Completude na Lógica Proposicional, se um argumento é semanticamente inválido, ele também é sintaticamente inválido. Assim, encontrar um contraexemplo é suficiente.

5.3. Associação com Tablôs Semânticos para Invalidade e Contraexemplo

Os tablôs semânticos são excelentes para demonstrar a invalidade e, mais importante, para encontrar um contraexemplo.

Passo a Passo para Demonstrar Invalidade e Encontrar Contraexemplo com Tablôs Semânticos:

1. Formalize o Argumento: Represente as premissas (A1, ..., An) e a conclusão (H).

2. Construa a Fórmula Condicional: A fórmula correspondente ao argumento é G = (A1 ∧ ... ∧ An) → H.

3. Negue a Fórmula para Validade: Para testar a validade, inicie o tablô com ¬G = ¬((A1 ∧ ... ∧ An) → H).

4. Desenvolva o Tablô: Aplique as regras de inferência do tablô semântico. Uma heurística útil é aplicar primeiro as regras que não bifurcam a árvore (R1, R5, R7, R8) para manter o tablô mais compacto.

5. Verifique os Ramos:

    ◦ Se todos os ramos se fecharem, o argumento é válido (como explicado na seção 2.4).

    ◦ Se pelo menos um ramo permanecer aberto (ou seja, não é possível encontrar uma fórmula A e sua negação ¬A no mesmo ramo), então o argumento é inválido.

6. Extrair o Contraexemplo (se inválido):

    ◦ Identifique um Ramo Aberto: Escolha qualquer ramo que não se fechou.

    ◦ Liste os Literais: Colete todos os literais (fórmulas atômicas ou suas negações) que aparecem nesse ramo aberto.

    ◦ Atribua Valores de Verdade:

        ▪ Para cada proposição atômica P que aparece como literal não negado no ramo, atribua I[P] = V (Verdadeiro).

        ▪ Para cada proposição atômica P cuja negação ¬P aparece como literal no ramo, atribua I[P] = F (Falso).

    ◦ Verifique: Esta atribuição de valores de verdade (I) é o contraexemplo. Sob essa interpretação, todas as premissas do argumento serão verdadeiras e a conclusão será falsa, demonstrando a invalidade do argumento.

    ◦ Exemplo Prático de Tablô e Contraexemplo: Considere o argumento: (P → Q), (Q → R) ∧ (R → S), ¬S ⊢ ¬P. Para testar a validade, construímos a fórmula: G = ((P → Q) ∧ ((Q → R) ∧ (R → S)) ∧ ¬S) → ¬P. Em seguida, iniciamos o tablô com ¬G: ¬G = ¬(((P → Q) ∧ ((Q → R) ∧ (R → S)) ∧ ¬S) → ¬P) Aplicando a regra de negação da implicação (R8 ou ¬(A→B) que resulta em A e ¬B), teremos duas subfórmulas:

        1. ((P → Q) ∧ ((Q → R) ∧ (R → S)) ∧ ¬S) (Verdadeira)

        2. ¬(¬P) (Verdadeira, que simplifica para P por R5)

