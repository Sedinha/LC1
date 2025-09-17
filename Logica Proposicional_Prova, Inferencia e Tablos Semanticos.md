1. Prova Lógica: O Coração da Dedução
O conceito de prova é fundamental não apenas na Matemática, mas em todas as ciências e até em nosso cotidiano. Na Lógica, uma prova não é uma mera "discussão" ou "contenda", mas sim uma justificação de uma conclusão. É uma análise crítica que nos permite distinguir argumentos e inferências corretas.
1.1. Definição e Natureza da Prova Lógica
Uma prova lógica (ou prova sintática) de uma fórmula H a partir de um conjunto de fórmulas β (hipóteses ou premissas) no sistema axiomático ℘a (Lógica Proposicional) ou ℘r (Lógica de Predicados) é uma sequência finita de fórmulas, digamos H1, H2, ..., Hn, onde:
1. A última fórmula da sequência (Hn) é a fórmula H que se deseja provar.
2. Para cada fórmula Hi na sequência, uma das seguintes condições é verdadeira:
    ◦ Hi é um axioma do sistema. Axiomas são fórmulas especiais que são consideradas "verdades básicas" ou "a priori" no sistema. No sistema ℘a, por exemplo, temos axiomas como (H ∨ H) → H (Ax1).
    ◦ Hi pertence ao conjunto de hipóteses β.
    ◦ Hi é deduzida de fórmulas anteriores na sequência (Hj e Hk, com j < i e k < i) utilizando uma regra de inferência. A principal regra de inferência é o Modus Ponens (MP).
É crucial entender que a prova sintática é um procedimento puramente sintático. Isso significa que ela não considera a interpretação ou o significado das fórmulas (se são verdadeiras ou falsas), mas sim a forma como são construídas e manipuladas de acordo com as regras estabelecidas. O objetivo é deduzir novas fórmulas a partir de outras, com base em sua estrutura, sem apelo ao conceito de verdade.
Notação:
• A dedução de H a partir de β é denotada por β ⊢ H. Este símbolo ⊢ representa a consequência lógica sintática ou dedução.
• Se β é um conjunto vazio de hipóteses, e ⊢ H, então H é um teorema do sistema.
Exemplo Prático (adaptado de): Seja o conjunto de premissas Δ = {p → q, r ∨ q, ¬r}. Queremos provar ¬p.
1. r ∨ q (Premissa - de Δ)
2. ¬r (Premissa - de Δ)
3. q (Silogismo Disjuntivo, 1, 2) – Se tivermos A ∨ B e ¬A, podemos concluir B.
4. p → q (Premissa - de Δ)
5. ¬p (Modus Tollens, 3, 4) – Se tivermos A → B e ¬B, podemos concluir ¬A.
Neste exemplo, cada passo é uma premissa ou é obtido de passos anteriores usando uma regra de inferência, demonstrando a prova de ¬p a partir de Δ.
1.2. Associação com Tablôs Semânticos
Enquanto a prova sintática lida com a derivação formal de fórmulas em um sistema axiomático, os tablôs semânticos oferecem um método semântico de dedução para verificar propriedades lógicas. Eles operam no "mundo semântico" ao investigar as interpretações de fórmulas.
Para demonstrar que uma fórmula H é uma tautologia (sempre verdadeira em todas as interpretações) usando tablôs semânticos, iniciamos o tablô com a negação de H (¬H). Se todos os ramos do tablô se fecharem (ou seja, cada ramo contém uma fórmula e sua negação, indicando uma contradição), então a suposição inicial de que ¬H é verdadeira levou a um absurdo. Pelo Teorema da Correção, isso implica que H é uma tautologia.
• Exemplo: Para provar que P ∨ ¬P é uma tautologia, construiríamos um tablô para ¬(P ∨ ¬P). Se ele fechar, P ∨ ¬P é uma tautologia.
• Para verificar a satisfatibilidade de um conjunto de fórmulas β = {A1, ..., An} ou se H é uma consequência lógica de β, iniciamos o tablô com β e a negação da conclusão (¬H). Se todos os ramos fecharem, a conclusão é consequência lógica das premissas. Se um ou mais ramos permanecerem abertos, um contraexemplo pode ser extraído para demonstrar que a fórmula não é uma tautologia ou que o argumento é inválido.
A equivalência entre esses dois mundos (sintático e semântico) é estabelecida pelos Teoremas da Correção e da Completude:
• Correção: Se uma fórmula tem uma prova sintática (⊢ H), então ela é uma tautologia (⊨ H). Isso garante que o sistema de prova não gera "falsidades".
• Completude: Se uma fórmula é uma tautologia (⊨ H), então existe uma prova sintática para ela (⊢ H). Isso garante que o sistema de prova é "poderoso" o suficiente para capturar todas as verdades lógicas.
--------------------------------------------------------------------------------
2. Regras de Inferência: As Ferramentas da Dedução
As regras de inferência são os mecanismos que nos permitem construir provas, deduzindo novas fórmulas a partir de outras já estabelecidas. Elas capturam as relações fundamentais entre os operadores lógicos e são, em sua maioria, bastante intuitivas.
Para cada conectivo lógico, idealmente, temos duas regras: uma de introdução (para mostrar como construir uma fórmula com aquele conectivo) e uma de eliminação (para mostrar como usar uma fórmula com aquele conectivo para derivar outra). Um conjunto de regras de inferência é considerado completo se todas as inferências válidas puderem ser provadas com elas.
2.1. Regras Fundamentais da Lógica Proposicional
Vamos considerar as regras conforme o sistema de Dedução Natural, que é mais natural para o raciocínio humano do que os sistemas axiomáticos.
• Implicação (→):
    ◦ Eliminação da Implicação (Modus Ponens - MP):
        ▪ Forma: Se tivermos H e H → G, podemos deduzir G.
        ▪ Exemplo: Se "Está chovendo" (P) e "Se está chovendo, então a rua está molhada" (P → Q), então deduzimos "A rua está molhada" (Q).
    ◦ Introdução da Implicação (→i):
        ▪ Forma: Se, assumindo H como hipótese, conseguimos provar G, então podemos concluir H → G e "descartar" a hipótese H.
        ▪ Exemplo: Se, ao assumir "Zé é inteligente" (P), você consegue mostrar que "Zé passa na prova" (Q), então você pode concluir "Se Zé é inteligente, então Zé passa na prova" (P → Q).
• Conjunção (∧):
    ◦ Introdução da Conjunção (∧i):
        ▪ Forma: Se tivermos H e G, podemos deduzir H ∧ G.
        ▪ Exemplo: Se "João tem 20 anos" (P) e "Maria tem 22 anos" (Q), então "João tem 20 anos E Maria tem 22 anos" (P ∧ Q).
    ◦ Eliminação da Conjunção (∧e):
        ▪ Forma: Se tivermos H ∧ G, podemos deduzir H. Alternativamente, podemos deduzir G.
        ▪ Exemplo: Se "O Brasil é um país E é grande" (P ∧ Q), podemos inferir "O Brasil é um país" (P).
• Disjunção (∨):
    ◦ Introdução da Disjunção (∨i):
        ▪ Forma: Se tivermos H, podemos deduzir H ∨ G (para qualquer G). Alternativamente, se tivermos G, podemos deduzir H ∨ G.
        ▪ Exemplo: Se "Vou ao teatro" (P), posso inferir "Vou ao teatro OU ao cinema" (P ∨ Q).
    ◦ Eliminação da Disjunção (∨e - Silogismo Disjuntivo):
        ▪ Forma: Se tivermos H ∨ G, e também ¬H, podemos deduzir G.
        ▪ Exemplo: Se "Maria está no Acre OU em Roraima" (P ∨ Q), e "Maria NÃO está no Acre" (¬P), podemos concluir "Maria está em Roraima" (Q).
• Negação (¬):
    ◦ Introdução da Negação (¬i - Prova por Contradição / Redução ao Absurdo):
        ▪ Forma: Se, assumindo H como hipótese, conseguimos provar uma contradição (⊥), então podemos concluir ¬H e "descartar" H.
        ▪ Exemplo: Se assumir que "A alma é um número inteiro" (P) leva à contradição "A alma é um número inteiro E não é um número inteiro" (P ∧ ¬P ou ⊥), então concluímos "A alma NÃO é um número inteiro" (¬P).
    ◦ Eliminação da Negação (¬e):
        ▪ Forma: Se tivermos ¬H e H, podemos deduzir uma contradição (⊥).
        ▪ Exemplo: Se "Não existe Deus" (¬P) e "Existe Deus" (P), isso leva a uma contradição.
• Outras Conectivas:
    ◦ A bi-implicação (↔) pode ser definida a partir de implicações e conjunção, como (H → G) ∧ (G → H). Suas regras de eliminação naturalmente seguem as da conjunção.
    ◦ A constante ⊥ (absurdo) tem a regra de Eliminação do Absurdo (⊥e), que afirma que de uma contradição, qualquer coisa pode ser deduzida.
2.2. Associação com Tablôs Semânticos
As regras de inferência nos tablôs semânticos são ferramentas para decompor fórmulas complexas em componentes mais simples (literais), procurando uma contradição em cada ramo. Elas são essencialmente regras de eliminação de conectivos, buscando desmembrar a fórmula original:
• Regras que não bifurcam (tipo alfa): Aplicadas quando uma premissa tem uma única forma de ser verdadeira (ou falsa). As conclusões são escritas em sequência no mesmo ramo.
    ◦ Exemplos: A ∧ B leva a A e B. ¬(A ∨ B) leva a ¬A e ¬B (Lei de De Morgan). ¬¬A leva a A. ¬(A → B) leva a A e ¬B.
• Regras que bifurcam (tipo beta): Aplicadas quando uma premissa pode ser verdadeira (ou falsa) de duas ou mais maneiras. Cada possibilidade inicia um novo ramo no tablô.
    ◦ Exemplos: A ∨ B leva a um ramo com A e outro ramo com B. A → B leva a um ramo com ¬A e outro ramo com B (equivalente a ¬A ∨ B). A ↔ B leva a um ramo com A ∧ B e outro ramo com ¬A ∧ ¬B.
Importante: A heurística de aplicação de regras em tablôs sugere aplicar preferencialmente as regras que não bifurcam a árvore primeiro (R1, R5, R7, R8 na notação padrão). Isso ajuda a manter o tablô mais compacto e legível.
--------------------------------------------------------------------------------
3. Regras Derivadas: Agilizando a Prova
Regras derivadas são atalhos. São regras que, embora não sejam primitivas do sistema (ou seja, poderiam ser provadas usando apenas as regras básicas), são tão comuns e úteis que são elevadas ao status de "regra" para simplificar e agilizar a construção de provas. Elas permitem condensar múltiplos passos de inferência em um único.
3.1. Exemplos Comuns de Regras Derivadas
• Prova por Condicional (→i):
    ◦ A versão generalizada da regra de introdução da implicação, fundamental para o Teorema da Dedução.
    ◦ Forma: Se, a partir de Γ e da hipótese φ, provamos ψ, então de Γ podemos provar φ → ψ.
    ◦ Essa regra é justificada pelo meta-teorema da dedução.
• Dupla Negação (Introdução ¬¬i e Eliminação ¬¬e):
    ◦ Introdução: Se temos H, podemos deduzir ¬¬H. (Se "Zé está feliz" (P), então "Não é verdade que Zé não está feliz" (¬¬P)).
    ◦ Eliminação: Se temos ¬¬H, podemos deduzir H. (Se "Não é verdade que Zé não está feliz" (¬¬P), então "Zé está feliz" (P)).
    ◦ A eliminação da dupla negação (¬¬e) é particularmente importante na Lógica Clássica.
• Modus Tollens (MT):
    ◦ Forma: Se temos H → G e ¬G, podemos deduzir ¬H.
    ◦ Exemplo: Se "Chove, então a rua molha" (P → Q), e "A rua NÃO está molhada" (¬Q), então "NÃO chove" (¬P).
• Silogismo Hipotético (SH) / Transitividade da Implicação:
    ◦ Forma: Se temos H → G e G → E, podemos deduzir H → E.
    ◦ Exemplo: Se "Se estudar, passa" (P → Q) e "Se passa, comemora" (Q → R), então "Se estudar, comemora" (P → R).
• Contraposição (CP):
    ◦ Forma: Se temos H → G, podemos deduzir ¬G → ¬H.
    ◦ Exemplo: Se "Se chove, a rua molha" (P → Q), então "Se a rua NÃO molha, NÃO chove" (¬Q → ¬P).
• Leis de De Morgan:
    ◦ São equivalências que permitem transformar negações de conjunções em disjunções e vice-versa. Embora apresentadas como leis de equivalência, na prática, elas informam regras de inferência para manipulação de negações.
    ◦ ¬(H ∧ G) equivale a ¬H ∨ ¬G.
    ◦ ¬(H ∨ G) equivale a ¬H ∧ ¬G.
• Comutatividade e Associatividade:
    ◦ Embora não sejam regras de inferência no sentido de "passo dedutivo", as propriedades comutativas (e.g., H ∧ G equivale a G ∧ H) e associativas (e.g., (H ∧ G) ∧ E equivale a H ∧ (G ∧ E)) dos conectivos ∧, ∨ e ↔ são frequentemente usadas para simplificar fórmulas e rearranjar termos em uma prova.
3.2. Associação com Tablôs Semânticos
No contexto dos tablôs semânticos, a noção de "regra derivada" não se aplica da mesma forma que na dedução natural. As regras dos tablôs (R1-R13) são geralmente consideradas primitivas para o método. No entanto, certas heurísticas na aplicação das regras funcionam de maneira análoga às regras derivadas, pois visam otimizar o processo de construção do tablô:
• Priorizar regras que não bifurcam: Isso ajuda a evitar a criação de muitos ramos, tornando o tablô mais fácil de gerenciar.
• Fechar ramos assim que uma contradição é encontrada: Não há necessidade de continuar desenvolvendo um ramo que já se mostrou contraditório.
--------------------------------------------------------------------------------
4. Passo a Passo para Resolução de Exercícios: Integrando os Métodos
Para agilizar a resolução de exercícios e solidificar o entendimento, é fundamental saber qual método aplicar e como.
4.1. Para Exercícios de Provas Sintáticas (Dedução Natural / Axiomático):
Se o objetivo é construir uma prova formal (sequência de passos) ou demonstrar Γ ⊢ φ:
1. Identifique as Premissas (Γ) e a Conclusão (φ).
2. Trabalhe de Baixo para Cima (da conclusão) ou de Cima para Baixo (das premissas):
    ◦ Se a conclusão é uma implicação (A → B), use a Introdução da Implicação (→i): "assuma A e tente provar B". Marque a hipótese assumida (e.g., [A]u) para descarte futuro.
    ◦ Se a conclusão é uma conjunção (A ∧ B), use a Introdução da Conjunção (∧i): "tente provar A e B separadamente".
    ◦ Se a conclusão é uma negação (¬A), use a Introdução da Negação (¬i): "assuma A e tente derivar uma contradição (⊥)". Marque [A]u.
    ◦ Se você tem uma implicação (A → B) e seu antecedente (A) como premissas, use Modus Ponens (→e) para derivar o consequente (B).
    ◦ Se você tem uma conjunção (A ∧ B) como premissa, use a Eliminação da Conjunção (∧e) para obter A ou B.
    ◦ Se você tem uma disjunção (A ∨ B) como premissa, e uma fórmula γ como objetivo, use a Eliminação da Disjunção (∨e): "prove γ assumindo A, e prove γ assumindo B".
3. Utilize Regras Derivadas para Simplificar: Sempre que possível, aplique Modus Tollens, Silogismo Hipotético, Contraposição ou Dupla Negação para encurtar a prova.
4. Feche Ramos com Axiomas: A prova de um sequente termina quando todas as folhas da árvore de derivação são axiomas (e.g., φ ⊢ φ).
5. Gerencie Hipóteses: Lembre-se de descartar (ou "descarregar") as hipóteses temporárias quando a regra de introdução correspondente é aplicada (e.g., o u em (→i)u).
4.2. Para Exercícios de Tablôs Semânticos (Validade, Tautologia, Satisfatibilidade):
Se o objetivo é verificar a validade de uma fórmula, se é uma tautologia, contradição, satisfatível, ou se um argumento é válido:
1. Formule a Questão para o Tablô:
    ◦ Tautologia/Validade de H: Comece o tablô com ¬H.
    ◦ Contradição de H: Comece o tablô com H.
    ◦ Satisfatibilidade de um conjunto {A1, ..., An}: Comece com A1, ..., An.
    ◦ Validade de um argumento Premissas → Conclusão: Comece com a negação do argumento completo ¬(Premissas → Conclusão).
2. Aplique as Regras de Decomposição: Decomponha as fórmulas usando as regras de inferência do tablô.
    ◦ Priorize as regras que não bifurcam a árvore (R1, R5, R7, R8). Isso minimiza a complexidade visual do tablô.
    ◦ No caso da Lógica de Predicados, as regras para quantificadores (R10-R13) exigem cuidado especial com a introdução de termos "novos" ou "quaisquer".
3. Feche os Ramos: Um ramo se fecha se ele contém uma fórmula A e sua negação ¬A (literais complementares). Quando um ramo se fecha, não há necessidade de continuar a expandi-lo.
4. Analise o Resultado Final:
    ◦ Todos os ramos fechados: A suposição inicial (negando a tautologia, por exemplo) levou a uma contradição. Portanto, a fórmula original é uma tautologia/válida, ou o argumento é válido.
    ◦ Um ou mais ramos abertos: A suposição inicial não levou a uma contradição. Isso significa que existe pelo menos uma interpretação que torna a fórmula falsa ou o argumento inválido.
5. Extraia o Contraexemplo (se houver ramos abertos):
    ◦ Para Lógica Proposicional: Para cada literal no ramo aberto, atribua T se o literal é uma proposição atômica (P) e F se for a negação de uma proposição atômica (¬P). Essa atribuição de valores de verdade será o contraexemplo.
    ◦ Para Lógica de Predicados: A partir dos literais em um ramo aberto, construa uma estrutura (domínio, interpretações para símbolos de predicados, funções e constantes) que torne as premissas verdadeiras e a conclusão falsa.