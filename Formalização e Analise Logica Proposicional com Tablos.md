Documento de Resumo: Formalização na Lógica Proposicional
1. Introdução à Formalização
A formalização é o processo fundamental de traduzir sentenças de uma linguagem natural, como o português, para a linguagem formal da lógica. O principal objetivo dessa tradução é eliminar ambiguidades e focar na forma dos argumentos, em vez de seu conteúdo. Ao formalizar, podemos estudar as regras de inferência sem as distrações do significado contextual, o que é crucial tanto para o desenvolvimento de hardware quanto de software na computação.
Na Lógica Proposicional (LP), trabalhamos com proposições, que são sentenças declarativas que podem ser classificadas como verdadeiras ou falsas, mas nunca ambas.
• Proposições Atômicas: São as unidades mais simples da LP, representadas por letras (e.g., P, Q, R, S). Elas não podem ser divididas em outras proposições.
• Proposições Moleculares (Compostas): São formadas pela combinação de proposições atômicas através de conectivos ou operadores.
2. Conectivos Lógicos (Operadores Verofuncionais)
Os conectivos são chamados verofuncionais porque seu valor de verdade depende unicamente dos valores de verdade das proposições que conectam, seguindo o princípio da composicionalidade. Os cinco operadores verofuncionais principais são:
1. Negação (¬)
    ◦ Símbolo: ¬ (til).
    ◦ Função: Unário, inverte o valor de verdade de uma proposição.
    ◦ Linguagem Natural: Expressa por "não", "não é o caso que", "é falso que", ou prefixos como "in-" e "a-".
    ◦ Exemplo: Se P = "Zé é inteligente", então ¬P = "Zé não é inteligente".
    ◦ Importância dos Parênteses: Ao negar proposições compostas, parênteses são cruciais para evitar ambiguidades (e.g., ¬(P → Q) é diferente de ¬P → Q).
2. Disjunção (∨)
    ◦ Símbolo: ∨.
    ◦ Função: Binário, é verdadeira se pelo menos uma das proposições é verdadeira.
    ◦ Linguagem Natural: Expressa por "ou". Na lógica clássica, o "ou" é inclusivo (aceita que ambas as partes sejam verdadeiras).
3. Conjunção (∧)
    ◦ Símbolo: ∧.
    ◦ Função: Binário, é verdadeira se e somente se ambas as proposições são verdadeiras.
    ◦ Linguagem Natural: Expressa por "e". Palavras como "mas", "porém", "no entanto", "entretanto" (que expressam adversidade) são formalizadas como "e", pois o aspecto adversativo não é relevante para a lógica clássica.
4. Implicação (Condicional) (→)
    ◦ Símbolo: →.
    ◦ Função: Binário (antecedente → consequente). É falsa apenas quando o antecedente é verdadeiro e o consequente é falso. Em todos os outros casos, é verdadeira (inclusive quando o antecedente é falso).
    ◦ Linguagem Natural: Expressa por "se...então...", "se", "é condição suficiente para que", "é condição necessária para que", "implica".
    ◦ Importante: Não assume relação causal ou temporal. Para evitar interpretações errôneas, é preferível pensar em P → Q como "não é o caso que P é verdadeiro e Q é falso".
5. Equivalência (Bicondicional) (↔)
    ◦ Símbolo: ↔.
    ◦ Função: Binário, é verdadeira se e somente se as duas proposições têm o mesmo valor de verdade.
    ◦ Linguagem Natural: Expressa por "se, e somente se" ou "sse", "bi-implicação".
Literais: Uma proposição atômica ou a negação de uma proposição atômica (e.g., P, ¬Q).
Passo a Passo para Formalização de Sentenças:
1. Leia a sentença cuidadosamente e identifique as palavras que denotam conectivos lógicos ("e", "ou", "se...então...", "não", "a menos que", "somente se", etc.).
2. Divida a sentença em suas proposições atômicas, as declarações mais simples que podem ser consideradas verdadeiras ou falsas.
3. Atribua uma variável proposicional (uma letra maiúscula como P, Q, R) a cada proposição atômica única. Evite usar 'F', 'V' ou 'T' como variáveis proposicionais, pois são usados para valores de verdade.
4. Reconstrua a sentença usando as variáveis proposicionais e os conectivos lógicos correspondentes. Utilize parênteses para garantir a clareza e evitar ambiguidades, definindo a ordem de precedência dos operadores. (A ordem de precedência padrão é: ¬ > (∀, ∃) > (→, ↔) > (∨, ∧)).
5. Desconsidere tempos verbais na maioria dos casos da lógica clássica, a menos que sejam cruciais para o significado.
3. Condições Necessárias e/ou Suficientes
A formalização de sentenças que expressam condições requer atenção especial devido à sua natureza contraintuitiva na linguagem natural.
• Condição Necessária:
    ◦ Sentença: "P é condição necessária para Q."
    ◦ Significado: Se Q acontece/é verdadeiro, então P deve ter acontecido/ser verdadeiro. Não é possível ter Q sem P.
    ◦ Formalização: Q → P.
    ◦ Exemplo: "Estudar é uma condição necessária para passar de ano."
        ▪ P = "Estudar"
        ▪ Q = "Passar de ano"
        ▪ Formalização: Q → P (Se você passou de ano, então você estudou).
        ▪ Erro comum intuitivo: P → Q (Se você estudou, então você passou de ano – isso pode não ser verdade, pode-se estudar e não passar).
• Condição Suficiente:
    ◦ Sentença: "P é condição suficiente para Q."
    ◦ Significado: Se P acontece/é verdadeiro, então Q certamente acontece/é verdadeiro. P é suficiente para garantir Q.
    ◦ Formalização: P → Q.
    ◦ Exemplo: "Argumentar é condição suficiente para justificar."
        ▪ P = "Argumentar"
        ▪ Q = "Justificar"
        ▪ Formalização: P → Q (Se você argumenta, então você justifica).
• "A menos que":
    ◦ Sentença: "P, a menos que Q." ou "P salvo se Q."
    ◦ Significado: Se Q não acontece/não é verdadeiro, então P acontece/é verdadeiro.
    ◦ Formalização: ¬Q → P.
    ◦ Exemplo: "Fulano não será aprovado a menos que estude."
        ▪ P = "Fulano não será aprovado"
        ▪ Q = "Fulano estude"
        ▪ Formalização: ¬Q → P (Se Fulano não estudar, então Fulano não será aprovado).
        ▪ Note que esta é a contrapositiva de ¬P → Q (Se Fulano for aprovado, então Fulano estudou), ou seja, Q → P (Se estudar é condição necessária para aprovação).
4. Formalização de Argumentos
Um argumento em lógica é uma coleção de sentenças (premissas) que são apresentadas como suporte para outra sentença (a conclusão). O propósito da lógica é avaliar se a conclusão é justificada pelas premissas.
• Estrutura Lógica Padrão: Em lógica, um argumento é frequentemente representado na forma Premissas → Conclusão. Mais especificamente, como uma conjunção das premissas implicando a conclusão: (P1 ∧ P2 ∧ ... ∧ Pn) → C. Alternativamente, em contextos de prova, pode-se listar as premissas e, em seguida, a conclusão, separadas por um símbolo como ∴.
Identificando Premissas e Conclusão: A conclusão de um argumento em linguagem natural nem sempre aparece no final. Certas palavras e frases funcionam como indicadores:
• Indicadores de Conclusão: "logo", "daí decorre que", "em consequência disso", "assim", "se segue que", "portanto", "isso prova que", "isso nos mostra que".
• Indicadores de Premissa: "desde que", "uma vez que", "pois", "porque", "já que".
Passo a Passo para Formalização de Argumentos:
1. Leia o argumento completo e identifique a conclusão, procurando por palavras indicadoras.
2. Identifique as premissas, que são todas as outras declarações que apoiam a conclusão.
3. Formalize cada premissa e a conclusão individualmente, usando o método de formalização de sentenças descrito na seção 2. Atribua variáveis proposicionais distintas para cada proposição atômica única.
4. Estruture o argumento na forma lógica padrão. Se P1, P2, ..., Pn são as premissas e C é a conclusão, a formalização é (P1 ∧ P2 ∧ ... ∧ Pn) → C. A ordem das premissas geralmente não altera a validade lógica.
5. Atenção a Premissas Omitidas: Em linguagem natural, algumas premissas podem ser implícitas ou omitidas. É importante reconstruir o argumento completo, explicitando todas as premissas para uma análise lógica rigorosa.
5. Associação com Tablôs Semânticos para Análise de Argumentos
O método dos tablôs semânticos é uma ferramenta poderosa para determinar a validade de argumentos e a satisfatibilidade de fórmulas na Lógica Proposicional e de Predicados.
Verificação da Validade de um Argumento via Tablôs Semânticos:
Um argumento é válido se, e somente se, em todas as situações em que as premissas são verdadeiras, a conclusão também é verdadeira. Em termos de tablôs semânticos, um argumento (P1 ∧ P2 ∧ ... ∧ Pn) → C é uma tautologia (válido) se o tableau de sua negação ¬((P1 ∧ P2 ∧ ... ∧ Pn) → C) for fechado.
Passo a Passo para Analisar a Validade de um Argumento com Tablôs Semânticos:
1. Negue a Conclusão: Para provar que o argumento (P1 ∧ P2 ∧ ... ∧ Pn) → C é válido, iniciamos o tableau com as premissas e a negação da conclusão. Isso é equivalente a iniciar o tableau com ¬((P1 ∧ P2 ∧ ... ∧ Pn) → C), que, pela regra da negação da implicação (R8), se decompõe em (P1 ∧ P2 ∧ ... ∧ Pn) e ¬C.
2. Liste as Fórmulas Iniciais: Escreva as premissas do argumento e a negação da conclusão (todas como verdadeiras) na raiz do tableau, uma abaixo da outra.
3. Aplique as Regras de Decomposição: Prossiga aplicando as regras de inferência dos tablôs semânticos às fórmulas, buscando decompô-las em fórmulas mais simples até chegar a literais.
    ◦ Regras que não bifurcam:
        ▪ A ∧ B → A e B.
        ▪ ¬¬A → A.
        ▪ ¬(A ∨ B) → ¬A e ¬B.
        ▪ ¬(A → B) → A e ¬B.
        ▪ Heurística: Priorize sempre a aplicação de regras que não bifurcam o tableau (R1, R5, R7, R8). Isso ajuda a manter o tableau menor e mais organizado.
    ◦ Regras que bifurcam:
        ▪ A ∨ B → Ramo 1: A, Ramo 2: B.
        ▪ A → B → Ramo 1: ¬A, Ramo 2: B. (Lembre-se da equivalência A → B ≡ ¬A ∨ B).
        ▪ A ↔ B → Ramo 1: A ∧ B, Ramo 2: ¬A ∧ ¬B.
        ▪ ¬(A ∧ B) → Ramo 1: ¬A, Ramo 2: ¬B. (Lembre-se da Lei de De Morgan: ¬(A ∧ B) ≡ ¬A ∨ ¬B).
        ▪ ¬(A ↔ B) → Ramo 1: A ∧ ¬B, Ramo 2: ¬A ∧ B.
    ◦ Marcação: É útil marcar as fórmulas já utilizadas (e.g., com uma bolinha) para garantir que todas as regras aplicáveis sejam exauridas.
4. Análise dos Ramos:
    ◦ Um ramo se fecha quando contém um par de literais complementares (uma fórmula e sua negação, e.g., P e ¬P). Indica uma contradição.
    ◦ Um ramo permanece aberto se não for possível encontrar literais complementares nele, mesmo após a aplicação exaustiva de todas as regras possíveis.
5. Conclusão:
    ◦ Se todos os ramos se fecham, o tableau está fechado. Isso significa que a suposição inicial (premissas verdadeiras e conclusão falsa) leva a uma contradição. Portanto, o argumento é válido (a fórmula negada era uma tautologia).
    ◦ Se pelo menos um ramo permanece aberto, o tableau está aberto. Isso significa que a suposição inicial (premissas verdadeiras e conclusão falsa) não leva a uma contradição. Portanto, o argumento é inválido.
Extração de Contraexemplo (para Lógica Proposicional):
Se um argumento é inválido (tableau aberto), um ramo aberto fornece um contraexemplo. Um contraexemplo é uma interpretação (atribuição de valores de verdade às proposições atômicas) que torna todas as premissas verdadeiras e a conclusão falsa.
Passo a Passo para Extrair um Contraexemplo de um Ramo Aberto:
1. Identifique os Literais do Ramo Aberto: Liste todas as proposições atômicas (e suas negações) que aparecem como literais no ramo aberto.
2. Atribua Valores de Verdade:
    ◦ Para cada proposição atômica P que aparece como literal positivo (P) no ramo, atribua I[P] = Verdadeiro.
    ◦ Para cada proposição atômica Q cuja negação (¬Q) aparece como literal no ramo, atribua I[Q] = Falso.
    ◦ Para proposições atômicas que não aparecem no ramo aberto (nem positivamente nem negativamente), seus valores podem ser atribuídos arbitrariamente (Verdadeiro ou Falso), pois não afetam a inconsistência do ramo.
3. Verifique: Essa interpretação será um contraexemplo, pois tornará as premissas verdadeiras e a conclusão falsa, demonstrando a invalidade do argumento.
• Nota para Lógica de Predicados: A extração de contraexemplos em Lógica de Predicados é mais complexa, exigindo a definição de um universo de discurso e funções de interpretação para predicados, funções e constantes, e não apenas atribuição de valores de verdade para literais.