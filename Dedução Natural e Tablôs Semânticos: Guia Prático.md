1. Dedução Natural (Método Direto)
O método direto de prova na Dedução Natural visa demonstrar que uma determinada conclusão se segue de um conjunto de premissas, aplicando-se regras de inferência diretamente às premissas já estabelecidas. Este é um processo fundamental para a validação de argumentos.
Conceitos Essenciais:
• Argumento: Uma afirmação ou conjunto de afirmações (premissas) usadas para justificar uma conclusão. Na Lógica, o foco é a relação objetiva entre premissas e conclusão, não o poder persuasivo.
• Premissas: Fórmulas ou afirmações iniciais que são aceitas como verdadeiras para o propósito da prova.
• Conclusão: A fórmula que se deseja derivar das premissas.
• Regras de Inferência: São esquemas de regras que permitem derivar novas fórmulas a partir de fórmulas existentes. Algumas são primitivas (aceitas sem demonstração, como o Modus Ponens), e outras são derivadas (podem ser provadas a partir das primitivas). As regras são divididas em regras de introdução (para construir um conectivo na conclusão) e eliminação (para "desmontar" um conectivo em uma premissa).
Regra Fundamental: Modus Ponens (→e) É uma das regras mais básicas e intuitivas. Se temos uma premissa na forma de uma implicação "H → G" e também a premissa "H" (o antecedente), podemos inferir "G" (o consequente).
• Notação: Premissa 1: H → G Premissa 2: H Conclusão: G
Exemplos Práticos de Regras (Método Direto):
Vamos considerar o alfabeto da Lógica Proposicional, que inclui símbolos proposicionais (P, Q, R, S, P1, Q1, R1, S1, P2, Q2, ...) e conectivos proposicionais (¬, ∨, ∧, →, ↔).
1. Introdução da Conjunção (∧i): Se você provou φ1 e provou φ2, então pode concluir a conjunção "φ1 ∧ φ2".
    ◦ Exemplo: Para provar P ∧ Q, se já temos P e já temos Q.
        1. P (Premissa)
        2. Q (Premissa)
        3. P ∧ Q (1, 2, Introdução da Conjunção)
2. Eliminação da Conjunção (∧e): Se você tem uma conjunção "φ1 ∧ φ2", pode concluir qualquer uma das suas partes ("φ1" ou "φ2").
    ◦ Exemplo: Para usar P ∧ Q.
        1. P ∧ Q (Premissa)
        2. P (1, Eliminação da Conjunção)
        3. Q (1, Eliminação da Conjunção)
3. Introdução da Disjunção (∨i): Se você provou φ1 (ou φ2), pode concluir a disjunção "φ1 ∨ φ2" (ou "φ2 ∨ φ1").
    ◦ Exemplo: Para provar P ∨ Q.
        1. P (Premissa)
        2. P ∨ Q (1, Introdução da Disjunção)
Passo a Passo para Resolução de Exercícios (Método Direto):
1. Identifique Premissas e Conclusão: Escreva claramente as premissas dadas e a conclusão que você quer atingir.
2. Analise a Conclusão: Qual é a estrutura da conclusão? Isso pode sugerir qual regra de introdução usar por último. Por exemplo, se a conclusão é "A ∧ B", você precisará provar A e provar B separadamente.
3. Analise as Premissas: Use regras de eliminação para "desmontar" as premissas e obter fórmulas mais simples.
4. Aplique Regras de Inferência: Comece a aplicar as regras (primitivas e derivadas) às suas premissas para derivar novas fórmulas.
    ◦ Dica: Marque as premissas ou linhas que você já usou (como com uma "bolinha" vista nos vídeos) para não se perder e identificar premissas desnecessárias.
5. Crie Novas Linhas: Cada nova fórmula derivada é uma nova linha em sua prova. Justifique cada linha com a regra usada e os números das linhas das quais ela foi derivada.
6. Continue até a Conclusão: Prossiga o processo até que a conclusão desejada seja alcançada.
Exemplo Ilustrativo do Método Direto (adaptado de fontes): Provar: {P → Q, Q} ⊢ P ∨ Q
1. P → Q (Premissa 1)
2. Q (Premissa 2)
3. P ∨ Q (2, Introdução da Disjunção – se Q é verdadeiro, então "P ou Q" também é.)
Nota: Este é um exemplo simples. Casos mais complexos podem envolver várias aplicações de regras e combinações.
--------------------------------------------------------------------------------
2. Dedução Natural (Provas Hipotéticas/Condicionais)
As provas hipotéticas, também um método direto, permitem fazer suposições temporárias para alcançar uma conclusão específica. Elas são cruciais quando a conclusão é uma implicação (A → B).
Conceitos Essenciais:
• Hipótese Temporária: Uma premissa assumida para o propósito de uma parte específica da prova. Essas hipóteses são marcadas (por exemplo, com colchetes ou uma barra vertical) para indicar seu escopo e que elas serão descartadas posteriormente.
• Regra de Prova Condicional / Introdução da Implicação (→i): Se, assumindo uma fórmula "A" como hipótese, você consegue derivar uma fórmula "B", então você pode concluir que "A implica B" ("A → B") e descartar a hipótese "A".
Passo a Passo para Resolução de Exercícios (Provas Hipotéticas):
1. Identifique a Conclusão como Implicação: Se a conclusão que você quer provar é da forma "A → B", este método é geralmente o mais adequado.
2. Assuma o Antecedente como Hipótese: Crie uma nova linha, assumindo "A" como uma hipótese temporária. Marque-a com uma notação apropriada (ex: [A]h ou | A).
3. Deduza o Consequente: Usando "A" (sua nova hipótese) e as premissas originais, aplique as regras de inferência para derivar "B".
4. Descarregue a Hipótese: Assim que você derivar "B", você pode aplicar a regra de introdução da implicação (→i). Isso permite concluir "A → B" e "descarregar" (ou descartar) a hipótese "A". A justificativa indicará as linhas onde a hipótese foi assumida e onde a conclusão "B" foi derivada, e o nome da regra (→i) seguido do identificador da hipótese descarregada.
5. Reiteração (Opcional, mas útil): A regra da reiteração permite repetir uma fórmula já provada (ou uma hipótese ativa) em um ponto posterior da prova, dentro do seu escopo, para usá-la em novas inferências.
Exemplo Ilustrativo de Prova Hipotética (adaptado de fontes): Provar: {P → Q, Q → R} ⊢ P → R (Silogismo Hipotético)
1. P → Q (Premissa 1)
2. Q → R (Premissa 2)
3. [P]h (Hipótese para →i)
4. Q (1, 3, Modus Ponens)
5. R (2, 4, Modus Ponens)
6. P → R (3-5, Introdução da Implicação, descarrega a hipótese P)
Regras Derivadas Comuns em Provas Hipotéticas:
• Modus Tollens (MT): Se "H → G" e "¬G" são verdadeiros, então "¬H" é verdadeiro.
    ◦ Exemplo:
        1. H → G (Premissa)
        2. ¬G (Premissa)
        3. [H]h (Hipótese para →i)
        4. G (1, 3, Modus Ponens)
        5. ⊥ (2, 4, Contradição - G e ¬G)
        6. ¬H (3-5, Introdução da Negação, descarrega H - Nota: Este é um método direto, mas a regra de introdução da negação tem um descarte de hipótese similar ao (→i), buscando uma contradição ⊥ para provar ¬H.)
• Contrapositiva (CP): "H → G" é equivalente a "¬G → ¬H". Pode ser demonstrado usando prova hipotética e Modus Tollens.
--------------------------------------------------------------------------------
3. Dedução Natural (Prova por Contradição / Redução ao Absurdo)
Este é um método indireto de prova, extremamente poderoso e frequentemente mais simples para certas classes de problemas do que o método direto. A ideia central é provar uma afirmação "A" mostrando que sua negação "¬A" leva a uma contradição (algo logicamente impossível).
Conceitos Essenciais:
• Negação da Conclusão: O primeiro passo é assumir a negação da fórmula que se deseja provar.
• Contradição (⊥): Uma fórmula que é sempre falsa (ex: "B ∧ ¬B"). Encontrar uma contradição significa que a suposição inicial deve ser falsa.
• Redução ao Absurdo (RAA / ¬i): Se, assumindo uma hipótese "H" você consegue derivar uma contradição "⊥", então você pode concluir "¬H" e descarregar a hipótese "H". Se o objetivo é provar "A" e você assume "¬A" e deriva uma contradição, então "¬¬A" é provado. Pela dupla negação, conclui-se "A".
Passo a Passo para Resolução de Exercícios (Prova por Contradição):
1. Identifique a Conclusão: Seja "A" a fórmula que você quer provar.
2. Assuma a Negação como Hipótese: Crie uma nova linha, assumindo "¬A" como uma hipótese temporária. Marque-a.
3. Derive uma Contradição: Usando "¬A" (sua nova hipótese) e as premissas originais, aplique as regras de inferência (introdução e eliminação, incluindo provas hipotéticas, se necessário) para derivar uma contradição. Uma contradição pode ser, por exemplo, "B ∧ ¬B" para alguma fórmula B, ou o símbolo especial de falsidade (⊥).
4. Descarregue a Hipótese e Conclua: Uma vez que a contradição é derivada, você aplica a regra da Redução ao Absurdo (ou introdução da negação para provar ¬¬A). Isso permite concluir "A" (se a hipótese foi ¬A) e descarregar "¬A".
Exemplo Ilustrativo de Prova por Contradição (adaptado de fontes): Provar: {P → Q, Q → R} ⊢ P → R (o mesmo silogismo hipotético, agora por contradição)
1. P → Q (Premissa 1)
2. Q → R (Premissa 2)
3. [¬(P → R)]h (Hipótese para Redução ao Absurdo)
4. [P]h' (Hipótese para Introdução da Implicação)
5. Q (1, 4, Modus Ponens)
6. R (2, 5, Modus Ponens)
7. P → R (4-6, Introdução da Implicação, descarrega P)
8. ⊥ (3, 7, Contradição - (P → R) e ¬(P → R))
9. P → R (3-8, Redução ao Absurdo, descarrega ¬(P → R))
--------------------------------------------------------------------------------
4. Associação com Tablôs Semânticos
Apesar de a Dedução Natural ser um método sintático (focado em regras de derivação) e os Tablôs Semânticos serem um método semântico (focado na atribuição de valores de verdade para encontrar uma interpretação), ambos são ferramentas poderosas para a dedução lógica e estão intrinsecamente relacionados pelos teoremas da Correção e da Completude.
• Correção da Lógica Proposicional: Se uma fórmula é provável por Dedução Natural (Γ ⊢ φ), então ela é uma consequência lógica (Γ |= φ), ou seja, é verdadeira em todas as interpretações onde as premissas são verdadeiras.
• Completude da Lógica Proposicional: Se uma fórmula é uma consequência lógica (Γ |= φ), então ela é provável por Dedução Natural (Γ ⊢ φ).
Esses teoremas nos asseguram que os dois métodos são equivalentes em poder, ou seja, tudo que pode ser provado por um, pode ser provado pelo outro.
A Ligação entre Prova por Contradição e Tablôs Semânticos:
O método da Redução ao Absurdo na Dedução Natural tem um paralelo direto com a construção de Tablôs Semânticos:
1. Objetivo: Provar que uma fórmula "H" é uma tautologia (sempre verdadeira) ou que um argumento é válido.
2. Início: Em ambos os métodos, o primeiro passo é negar o que se quer provar.
    ◦ Dedução Natural (Contradição): Você assume "¬H" como uma hipótese.
    ◦ Tablôs Semânticos: Você inicia o tablô com "¬H".
3. Busca por Contradição:
    ◦ Dedução Natural: Aplica-se regras de inferência até derivar uma contradição explícita (como "B ∧ ¬B" ou ⊥).
    ◦ Tablôs Semânticos: Aplica-se regras de dedução do tablô (que ramificam ou não) até que todos os ramos se "fechem" (ou seja, cada ramo contenha uma fórmula "A" e sua negação "¬A").
4. Conclusão:
    ◦ Dedução Natural: Se uma contradição é alcançada a partir de "¬H", então "¬H" é falsa, o que significa que "H" deve ser verdadeira (tautologia).
    ◦ Tablôs Semânticos: Se todos os ramos do tablô iniciado com "¬H" se fecham, isso prova que "¬H" é uma contradição e, portanto, "H" é uma tautologia.
Vantagens dos Tablôs Semânticos (para agilizar a resolução de exercícios e análise):
• Busca Sistemática por Contraexemplo: Se um tablô iniciado com "¬H" não fecha (ou seja, tem pelo menos um ramo aberto), esse ramo aberto oferece um contraexemplo. Isso significa que ele indica uma interpretação (atribuição de valores de verdade para as proposições atômicas) na qual "¬H" é verdadeira, e consequentemente "H" é falsa. Isso é extremamente útil para provar que uma fórmula não é uma tautologia ou que um argumento não é válido.
    ◦ Passo a passo para obter um contraexemplo de um tablô aberto:
        1. Escolha um ramo que permaneça aberto (não fechado).
        2. Liste todos os literais (fórmulas atômicas ou suas negações) presentes nesse ramo.
        3. Atribua valores de verdade: Se um literal é "P", P é Verdadeiro. Se é "¬P", P é Falso.
        4. Essa atribuição é a interpretação que torna a fórmula original (ou o argumento) falsa, sendo, portanto, o contraexemplo.
• Procedimento Algorítmico: Os tablôs semânticos podem ser vistos como um algoritmo para verificar a validade de fórmulas na Lógica Proposicional. A sua implementação em computadores é facilitada, diferentemente dos sistemas axiomáticos mais abstratos.
• Heurística para Eficiência: Para manter os tablôs menores e mais fáceis de analisar, uma heurística é aplicar primeiro as regras que não bifurcam (R1, R5, R7 e R8).
Exemplo de Ligação Prática:
Se você usa a Dedução Natural para provar que uma fórmula é uma tautologia, e seu processo é demorado ou você se perde, a construção do Tablô Semântico para a negação daquela fórmula pode confirmar sua intuição.
• Se o Tablô fechar: Sua fórmula é de fato uma tautologia. Você sabe que a prova por Dedução Natural é possível, mesmo que você não a tenha encontrado ainda.
• Se o Tablô ficar aberto: Sua fórmula não é uma tautologia. O ramo aberto fornecerá um contraexemplo, que lhe dará a interpretação exata em que a fórmula é falsa. Isso é crucial para evitar gastar tempo tentando provar algo que é, na verdade, inválido.
--------------------------------------------------------------------------------
Guia de Resolução de Exercícios Integrado: Dedução Natural e Tablôs Semânticos
Para maximizar a eficiência na resolução de exercícios, sugerimos a seguinte abordagem:
1. Entendimento do Problema:
    ◦ Identifique claramente as proposições atômicas envolvidas.
    ◦ Formalize o argumento ou a fórmula na linguagem da Lógica Proposicional.
    ◦ Exemplo: "Se o Curingão caiu para a segundona e sua torcida chorou, então ficamos com pena deles. Portanto: Dado que a torcida chorou se o Curingão caiu para a segundona, podemos concluir que ficamos com pena deles se o Curingão caiu para a segundona.".
        ▪ Proposições Atômicas:
            • P = "O Curingão caiu para a segundona"
            • Q = "Sua torcida chorou"
            • R = "Ficamos com pena deles"
        ▪ Formalização: ((P ∧ Q) → R) ⊢ (Q → P) → (P → R)
2. Verificação Preliminar com Tablôs Semânticos (Recomendado para eficiência):
    ◦ Negue o argumento: A forma geral de um argumento é "Premissas → Conclusão". Para verificar a validade de um argumento, negue toda a implicação: ¬(Premissas → Conclusão). Se for provar uma tautologia H, inicie com ¬H.
        ▪ Exemplo: ¬[((P ∧ Q) → R) → ((Q → P) → (P → R))]
    ◦ Construa o Tablô: Aplique as regras dos tablôs semânticos (R1 a R9 para Lógica Proposicional) de forma sistemática.
        ▪ Heurística: Priorize as regras que não bifurcam a árvore (R1: conjunção, R5: dupla negação, R7: negação da disjunção, R8: negação da implicação) para manter o tablô mais conciso.
    ◦ Analise o Resultado do Tablô:
        ▪ Se todos os ramos fecharem: A negação do argumento (ou da fórmula) é uma contradição. Isso significa que o argumento original é válido (ou a fórmula é uma tautologia). Você tem a garantia de que uma prova por Dedução Natural existe.
        ▪ Se pelo menos um ramo permanecer aberto: A negação do argumento (ou da fórmula) é satisfatível. Isso significa que o argumento original é inválido (ou a fórmula não é uma tautologia). O ramo aberto fornece um contraexemplo. As atribuições de verdade dos literais nesse ramo formam uma interpretação que torna o argumento (ou a fórmula) falso. Isso evita que você gaste tempo tentando provar algo impossível.
3. Construção da Prova por Dedução Natural (se o tablô fechou):
    ◦ Método Direto:
        ▪ Liste as premissas.
        ▪ Aplique sequencialmente as regras de introdução e eliminação para derivar a conclusão.
        ▪ Marque as linhas usadas para organização.
    ◦ Provas Hipotéticas (se a conclusão é uma implicação A → B):
        ▪ Liste as premissas.
        ▪ Crie uma nova subprova assumindo [A]h como hipótese.
        ▪ Dentro dessa subprova, derive B.
        ▪ Feche a subprova e conclua A → B usando a regra (→i)h.
    ◦ Prova por Contradição (se A for a conclusão desejada):
        ▪ Liste as premissas.
        ▪ Crie uma nova subprova assumindo [¬A]h como hipótese.
        ▪ Dentro dessa subprova, derive uma contradição (B ∧ ¬B ou ⊥).
        ▪ Feche a subprova e conclua A usando a regra da Redução ao Absurdo (ou ¬i seguido de dupla negação).
4. Revisão:
    ◦ Verifique se cada passo da prova é justificado por uma regra válida e por premissas/linhas anteriores dentro do escopo correto.
    ◦ Confirme se a conclusão final corresponde exatamente ao que foi pedido.
