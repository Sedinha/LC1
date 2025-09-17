Guia de Estudo: Lógica Proposicional e Lógica de Predicados
Este guia de estudo foi elaborado para revisar sua compreensão dos fundamentos da Lógica, abrangendo Lógica Proposicional e Lógica de Predicados, com ênfase nas necessidades da Ciência da Computação e áreas afins.

I. Lógica Proposicional (LP)
A. Fundamentos e Conceitos Básicos
Definição e Natureza da Lógica:
O que é Lógica e qual seu objetivo principal neste contexto?
Qual a abordagem deste material em relação aos problemas filosóficos e de argumentação lógica?
Para quais áreas a Lógica Clássica é considerada fundamental neste livro?
Linguagem da Lógica Proposicional:
Compreensão de Proposição: O que é e quais características possui? Exemplos de sentenças que são e não são proposições.
Distinção entre linguagem-objeto e metalinguagem.
Componentes do Alfabeto da Lógica Proposicional (definição 1.1):
Símbolos de pontuação.
Símbolos proposicionais (sua natureza e representação).
Conectivos proposicionais (símbolos e denominações: ¬, ∨, ∧, →, ↔).
Símbolos de verdade (true, false): são parte do alfabeto padrão? Qual sua função e interpretação?
Fórmulas: Definição indutiva das fórmulas bem formadas (definição 1.2).
Precedência de conectivos e omissão de parênteses.
Características Sintáticas das Fórmulas:
Variáveis da metalinguagem (P̆, A, H, G): o que representam?
Esquemas de fórmulas: o que são e como se relacionam com as fórmulas?
Comprimento de uma fórmula (definição 1.4).
Subfórmula (definição 1.5).
Notação Polonesa (prefixa): como as fórmulas são construídas e como convertê-las para a notação usual.
Semântica da Lógica Proposicional:
Introdução à semântica: como interpretar fórmulas.
Função binária (definição 2.3).
Princípio de Bivalência: o que implica para a Lógica Clássica?
Função Interpretação (definição 2.5): domínio, contradomínio.
Regras semânticas para interpretação de fórmulas (definição 2.6) e tabelas-verdade.
Análise da semântica de cada conectivo (¬, ∨, ∧, →, ↔) em comparação com a linguagem natural:
Negação: diferenças com "não", "infeliz".
Disjunção (inclusiva): "ou" na LP vs. "ou" na linguagem natural.
Conjunção: "e", "mas", "todavia" e perda de nuances temporais/causais.
Implicação material (→): o que significa "P implica Q" na LP? Relação com causa e tempo. Prova de Russell.
Bi-implicação (↔): "se, e somente se".
Princípio da Composicionalidade e Funções de Verdade: importância para a Lógica Clássica.
Representação de sentenças e argumentos lógicos em LP:
Passos para tradução (identificar proposições atômicas, atribuir símbolos, usar conectivos, estruturar).
Expressões que indicam premissas e conclusões em argumentos.
A importância de argumentos completos.
B. Propriedades Semânticas da Lógica Proposicional
Conceitos Fundamentais:
Tautologia (definição 3.1): o que é? Exemplo: (P ∨ ¬P) e o princípio do terceiro-excluído.
Satisfatibilidade (definição 3.2): o que é? Relação com tautologia.
Contradição Semântica (definição 3.3): o que é?
Contingência (definição 3.4): o que é?
Implicação Semântica (definição 3.9): entre fórmulas e entre conjuntos de fórmulas (consequência lógica semântica).
Equivalência Semântica (definição 3.6): relação com a bi-implicação.
Relações Semânticas entre Conectivos:
Conjuntos de conectivos completos (definição 3.11): o que significa e exemplos ({¬,∨}, {¬,∧}, {nand}, {nor}).
Simplificação do alfabeto da Lógica Proposicional (definição 3.14).
Transformação de fórmulas para conjuntos completos de conectivos.
Regra da Substituição (proposição 3.15).
Formas Normais:
Literal (definição 3.16).
Forma Normal Conjuntiva (FNC) e Forma Normal Disjuntiva (FND) (definição 3.17).
Algoritmo para obtenção de FND e FNC.
Conceito de dualidade entre algoritmos.
Classificação dos Argumentos Lógicos:
Argumento "Correto" vs. "Bom".
Classificação baseada em tautologia, satisfatibilidade e implicação.
Uso de diagramas de Venn para análise de argumentos.
C. Métodos Semânticos de Dedução na Lógica Proposicional
Método da Tabela-Verdade:
Custo computacional para verificar satisfatibilidade: análise do pior caso, notação exponencial, relação com o problema P=NP.
Limitações para fórmulas com muitos símbolos proposicionais.
Método da Negação (Redução ao Absurdo):
Fundamentos: supor o oposto e buscar uma contradição.
Aplicações para provar tautologias e contradições.
Várias possibilidades no desenvolvimento da prova: quando é mais simples (conectivos →, ∨ falsos; ∧ verdadeiro) e quando não (conectivo ↔ falso).
Custo computacional (no pior caso): ainda exponencial. Vantagens em casos específicos.
Tableaux Semânticos na Lógica Proposicional:
Sistemas de dedução: tableaux como alternativa aos sistemas axiomáticos para implementação computacional.
Elementos básicos: alfabeto, fórmulas, regras de dedução (R1-R9).
Significado das regras de inferência (R1-R9): como representam a lógica e a dedução.
Construção de tableaux: aplicação de regras, ramos abertos/fechados.
Heurística para aplicação de regras (preferir regras que não bifurcam).
Tableau fechado (definição 4.7) e tableau aberto (definição 4.8).
Teorema da Correção (4.1) e Teorema da Completude (4.2): o que significam para os tableaux semânticos.
Consequência lógica de conjunto de hipóteses por tableaux.
Relação entre tableaux semânticos, prova por contradição e tabelas-verdade.
D. Método Sintático de Dedução na Lógica Proposicional (Sistema ℘a)
Sistema Formal ℘a:
Denotações para conectivos (∧, →, ↔) em termos de ¬ e ∨.
Axiomas do sistema ℘a (Ax1, Ax2, Ax3) (definição 5.2): são tautologias?
Natureza dos axiomas (esquemas de fórmulas, infinitamente axiomatizável, decidível, enumerável).
Regra de inferência: Modus Ponens (definição 5.3).
Prova e Consequência Lógica Sintática:
Prova sintática (definição 5.4): sequência de fórmulas.
Consequência lógica sintática (definição 5.5): existe uma prova.
Notação (β ⊢ H) vs (β ⊨ H): diferença entre consequência sintática e semântica.
Limitações do método de prova sintático (indecidibilidade, loops).
Propriedades do Sistema ℘a:
Lema 5.1 (Axioma de Introdução).
Proposição 5.2 (princípio do terceiro excluído sintático).
Regra da substituição (proposição 5.3).
Teorema da Dedução (5.1): forma sintática.
Teorema da Correção (5.2): todo teorema é uma tautologia.
Teorema da Completude (5.3): toda tautologia é um teorema.
Equivalência entre consequência lógica semântica e sintática em ℘a.
Equivalência entre tautologia e teorema em ℘a.
Consistência:
Consistência de um sistema axiomático (definição 5.7): o que significa um sistema não ser consistente (trivialização).
Teorema da Consistência (5.4) do sistema ℘a.
Consistência de um conjunto de fórmulas (definição 5.9).
Teorema da Consistência e Satisfatibilidade (5.5).
II. Lógica de Predicados (LPO)
A. Linguagem da Lógica de Predicados
Motivação e Extensão da LP:
Limitações de expressividade da LP (silogismos categóricos, quantificações).
Como a Lógica de Predicados estende a LP (quantificadores, símbolos funcionais, predicados, variáveis).
Lógicas Complementares vs. Lógicas Alternativas.
Componentes do Alfabeto da Lógica de Predicados (definição 6.1):
Símbolos de pontuação e conectivos.
Símbolos para variáveis (x, y, z, ...).
Símbolos para funções (f, g, h, ...) e sua aridade. Constantes como funções zero-árias.
Símbolos para predicados (p, q, r, ...) e sua aridade. Símbolos proposicionais como predicados zero-ários.
Símbolos para quantificadores (∀, ∃).
Natureza dos conjuntos de símbolos (infinitos e enumeráveis).
Termos, Átomos e Fórmulas:
Termo (definição 6.2): definição indutiva e exemplos (variáveis, constantes, aplicação de funções). Notação prefixa vs. infixa.
Átomo (definição 6.3): definição indutiva e exemplos (símbolos proposicionais, aplicação de predicados a termos).
Fórmula (definição 6.4): definição indutiva a partir de átomos e conectivos lógicos/quantificadores.
Correspondência entre quantificadores (definição 6.6): ∀ e ∃ podem ser definidos um a partir do outro.
Precedência de conectivos e quantificadores.
Características Sintáticas das Fórmulas:
Subtermo, Subfórmula, Subexpressão (definição 6.8).
Comprimento de uma fórmula (definição 6.9).
Escopo de um quantificador (definição 6.10).
Ocorrência livre e ligada de uma variável (definição 6.11).
Variável livre e ligada em uma fórmula (definição 6.12).
Símbolos livres de uma fórmula (definição 6.13).
Fórmula fechada (sentença) (definição 6.14).
Fecho universal e existencial de uma fórmula (definição 6.15).
Formas Normais e Programação em Lógica:
Literal na Lógica de Predicados (definição 6.16).
Forma Normal Conjuntiva (FNC) e Forma Normal Disjuntiva (FND) (definição 6.17).
Cláusula de programa (definição 6.18) e sua denotação em Prolog.
Cláusula unitária (fato) (definição 6.19).
Programa lógico (definição 6.20).
B. Semântica da Lógica de Predicados
Introdução à Semântica:
Necessidade de interpretações mais elaboradas (domínio, variáveis, funções, predicados, quantificadores).
Abordagens de interpretação (Tarski, Manna/Mendelson).
Interpretação Informal de Predicados e Funções:
Domínio do Discurso (Universo U): papel fundamental.
Interpretação de predicados e funções: o que representam (Exemplos 7.1, 7.2, 7.3).
Função Semântica para símbolos de função (I[f]: Uⁿ → U) e predicado (I[p]: Uⁿ → {T,F}).
Interpretação de Átomos e Termos (definição 7.1):
Interpretação de variáveis, constantes, símbolos de função, termos, símbolos de predicado e átomos.
Interpretação I é uma função total.
Interpretação de Fórmulas com Estrutura Inicial Simples (definição 7.2) e Quantificadores:
Regras semânticas para conectivos (análogas à LP).
Interpretação estendida (<x←d>I) (definição 7.4): o que faz e por que é necessária.
Regras semânticas para quantificadores (definição 7.5) (∀x)H e (∃x)H.
Diferença entre o quantificador na linguagem e na metalinguagem.
A necessidade de interpretar símbolos livres (variáveis livres em particular).
Diferença de significado entre (∀x)(∃y)p(x,y) e (∃y)(∀x)p(x,y).
A Aritmética na Lógica de Predicados:
Representação dos números naturais: modelo padrão, constante 0, função sucessor S.
Notação de numerais (1, 2, ...).
Representação de operações básicas (adição +̂, multiplicação ×̂).
Representação de propriedades aritméticas (igualdade =̂).
Aritmética de Robinson (Aritmética básica): alfabeto estendido, princípios fundamentais (Bx1-Bx7).
Definições recursivas de funções e predicados (ex: fatorial, exponencial).
Linguagem da Aritmética básica (La) (definição 7.8): símbolos lógicos e não lógicos.
Interpretação da Aritmética básica: modelos padrão vs. interpretações não usuais (modelos da Aritmética).
Expressividade da Aritmética básica (definição 7.9): Teorema 7.1.
Representação de Argumentos Lógicos:
Tradução de argumentos da linguagem natural para Lógica de Predicados.
Exemplos de silogismos categóricos e sua formalização.
C. Propriedades Semânticas da Lógica de Predicados
Conceitos Fundamentais:
Satisfatibilidade na Lógica de Predicados.
Validade (definição 8.7): o que é?
Fórmula tautologicamente válida (definição 8.6): relação com tautologia da LP.
Relação entre validade, tautologia e fórmulas tautologicamente válidas.
Princípio de Identidade.
Implicação Semântica e Equivalência Semântica na Lógica de Predicados.
Generalização de uma fórmula (proposição 8.2).
Classificação dos Argumentos Lógicos (LPO):
Uso de Diagramas de Venn para análise de validade.
Exemplos de argumentos válidos, inválidos, corretos, bons, fortes e fracos.
D. Métodos Semânticos de Dedução na Lógica de Predicados
Método dos Tableaux Semânticos (LPO):Regras para quantificadores (R10-R13).
Significado das regras R10-R13 e a manipulação de negação e quantificadores.
O termo "novo" na regra R12 (∃x)A → A(t) e a importância de sua novidade.
O termo "qualquer" na regra R13 (∀x)A → A(t).
Construção de tableaux em LPO: exemplos.
Impacto da ordem de aplicação das regras na Lógica de Predicados.
Ramos infinitos nos tableaux em LPO.
Indecidibilidade na Lógica de Predicados (Teorema 9.3): o que significa e suas consequências para os métodos de decisão (prova do sim e do não).
E. Método Sintático de Dedução na Lógica de Predicados (Sistema ℘r)
Elementos Básicos do Sistema Formal ℘r (definição 10.1):
Alfabeto, fórmulas, axiomas, regras de dedução.
Notação H{x←t} para substituição.
Substituição Segura (definição 10.2): importância de variáveis em t ocorrerem livremente em H{x←t}.
Axiomas do Sistema ℘r (definição 10.3):
Ax1, Ax2, Ax3 (análogos a ℘a).
Ax4 ((∀x)H → H{x←t}): significado e restrição da substituição segura.
Ax5 ((∀x)(H ∨G) → (H ∨ (∀x)G)): significado e restrição da não ocorrência livre de x em H.
Validade dos axiomas de ℘r.
Lema 10.1 (Substitutividade): fundamental para a validade de Ax4.
Regras de Dedução:
Modus Ponens (definição 10.4).
Generalização (GE) (definição 10.4): H → (∀x)H se x não ocorre livre em hipóteses.
Denotações para conectivos e quantificadores.
Consequência Lógica Sintática em ℘r:
Prova sintática (definição 10.5).
Corolário 10.1 (Teorema da Dedução): restrição para fórmulas fechadas.
Teoremas de Correção e Completude (LPO):
Teorema da Correção (10.2): se é teorema, então é válido.
Teorema da Completude (10.3): se é válido, então é teorema.
Consequências dos teoremas: equivalência entre validade e teorema, entre consequência semântica e sintática.
Importância da distinção entre sistema ℘a e ℘r.
Sistemas Formais Aritméticos:
Sistema Formal Q (Aritmética de Robinson): axiomas Bx1-Bx7.
Incompletude do sistema Q para negação.
Sistema Formal PA (Aritmética de Peano): axiomas de Q + axioma Bx8 (princípio de indução finita).
Expressividade e Captura:
Capturando uma propriedade (definição 10.13).
Capturando uma função (definição 10.14).
Números representáveis por um sistema formal (definição 10.15).
Teoremas de Incompletude de Gödel (10.5, 10.6).
Teorema de Tarski (10.8): impossibilidade de definir "verdade" no próprio sistema.
III. Provas e Dedução Natural
Consequência Lógica Sintática (β ⊢ α):
Definição de prova como sequência de fórmulas.
Natureza formal e mecânica.
Proposição:
Definição e exemplos.
Atômicas vs. Compostas.
Argumentos:
Validar argumentos.
Argumento "Correto" vs. "Bom".
Formalização de argumentos: identificar premissas, conclusão, variáveis proposicionais, conectivos.
Dedução Natural (Sistema de Moura):
Regras de introdução e eliminação.
Axioma (Ax): φ ⊢ φ.
Regra de Eliminação da Implicação (→e) / Modus Ponens (MP).
Regra de Introdução da Implicação (→i): descarte de hipóteses.
Outras regras (¬i, ¬e, ∧i, ∧e, ∨i, ∨e).
Construção de provas sintáticas em árvore: exemplos (Modus Tollens, Contrapositiva).
Regras derivadas (¬¬i, MT, CP, (→i)∅).
Papel da criatividade na construção de provas.
Lógica Proposicional Intuicionista (LPI) vs. Lógica Proposicional Clássica (LPC).
Regra de Prova por Contradição (PBC) (¬e), Lei do Terceiro Excluído (LEM), Lei de Peirce (LP): equivalência e relação com LPC.
Problemas de honestos e desonestos como aplicação da semântica.
Gramática da LP com ⊥, ¬, ∧, ∨, →.
Quiz de Lógica
Instruções: Responda às dez questões a seguir com 2-3 frases cada.

Qual é a principal diferença entre a abordagem da Lógica Clássica apresentada no material e uma abordagem filosófica ou focada em argumentação lógica?
Explique o conceito de "proposição" na Lógica Proposicional e forneça um exemplo de sentença da linguagem natural que não seria considerada uma proposição.
Descreva a função principal dos conectivos proposicionais na construção de fórmulas lógicas e mencione a ordem de precedência entre eles.
O que distingue a interpretação do conectivo de disjunção (∨) na Lógica Clássica da palavra "ou" na linguagem natural, especialmente no que diz respeito à inclusividade?
No contexto da Lógica Proposicional, qual é a diferença crucial entre um argumento "correto" e um argumento "bom"?
Explique por que o método da tabela-verdade se torna computacionalmente inviável para fórmulas com um grande número de símbolos proposicionais.
Qual é o significado do Teorema da Correção no sistema de Tableaux Semânticos da Lógica Proposicional?
Na Lógica de Predicados, o que é uma "substituição segura" de um termo por uma variável em uma fórmula H{x←t}, e por que essa condição é importante para o axioma Ax4?
Diferencie uma "variável livre" de uma "variável ligada" em uma fórmula da Lógica de Predicados.
Explique o que é a Indecidibilidade na Lógica de Predicados (Teorema 9.3) e qual sua implicação para os métodos de decisão.
Chave de Respostas do Quiz
A Lógica Clássica, conforme apresentada, foca nos fundamentos da Lógica Matemática necessários à Ciência da Computação, simplificando problemas filosóficos e enfatizando elementos iniciais de argumentação. Abordagens filosóficas ou de argumentação lógica, por outro lado, se aprofundam nas controvérsias e nuances da linguagem natural e do raciocínio humano.
Uma proposição na Lógica Proposicional é uma afirmação ou sentença declarativa que pode ser qualificada como verdadeira ou falsa, mas nunca ambas simultaneamente. Um exemplo de sentença que não seria uma proposição é "Feche a porta!", pois é uma ordem e não pode ser julgada como verdadeira ou falsa.
Os conectivos proposicionais combinam proposições simples para formar proposições mais complexas, estabelecendo relações lógicas entre elas. A ordem de precedência, da maior para a menor, é: negação (¬), conjunção (∧), disjunção (∨, ⊕), implicação (→) e bi-implicação (↔).
A disjunção (∨) na Lógica Clássica é inclusiva, significando que "P ou Q" é verdadeiro se P for verdadeiro, Q for verdadeiro, ou ambos forem verdadeiros. Na linguagem natural, a palavra "ou" pode ter um sentido exclusivo, implicando que apenas uma das alternativas pode ser verdadeira, mas não ambas.
Um argumento é "correto" se suas premissas justificam a conclusão, ou seja, se a implicação (premissas → conclusão) é semanticamente válida (uma tautologia). Um argumento é "bom" se, além de ser correto, suas premissas são de fato verdadeiras no mundo real.
O método da tabela-verdade tem um custo computacional exponencial em relação ao número de símbolos proposicionais na fórmula. Para uma fórmula com 'n' símbolos, há 2^n linhas para analisar, tornando o processo impraticável para valores de 'n' maiores.
O Teorema da Correção (Teorema 4.1) afirma que se existe uma prova de uma fórmula H no sistema de Tableaux Semânticos (ou seja, um tableau fechado iniciado com ¬H), então H é uma tautologia. Isso garante que o sistema de dedução não prova nada que seja semanticamente inválido.
Uma substituição {x←t} é segura para uma fórmula H quando toda variável que ocorre no termo t ocorre livremente na fórmula H{x←t} (H com x substituído por t). Essa condição é crucial para o axioma Ax4 da Lógica de Predicados (∀x)H → H{x←t}, pois impede que uma variável no termo t seja "capturada" por um quantificador em H, alterando o significado pretendido.
Em uma fórmula da Lógica de Predicados, uma ocorrência de uma variável é "ligada" se está dentro do escopo de um quantificador que a quantifica (e.g., x em (∀x)P(x)). Uma ocorrência é "livre" se não estiver sob o escopo de um quantificador que a quantifica. Uma variável é considerada "livre" em uma fórmula se tiver pelo menos uma ocorrência livre, e "ligada" se tiver pelo menos uma ocorrência ligada.
O Teorema da Indecidibilidade (Teorema 9.3) na Lógica de Predicados afirma que não existe um algoritmo que possa, para qualquer fórmula, decidir em um número finito de passos se ela é satisfatível ou não (sem entrar em loop). Isso significa que, ao contrário da Lógica Proposicional, não há um procedimento algorítmico universal que garanta uma resposta "sim" ou "não" para a satisfatibilidade ou validade de qualquer fórmula na LPO.
Questões Dissertativas
Compare e contraste os conceitos de "tautologia" na Lógica Proposicional e "validade" na Lógica de Predicados. Explique por que uma fórmula válida na Lógica de Predicados nem sempre é tautologicamente válida, fornecendo um exemplo conceitual.
Discuta a relação entre os métodos semânticos de dedução na Lógica Proposicional (tabela-verdade, redução ao absurdo, tableaux semânticos). Embora sejam "equivalentes do ponto de vista conceitual", explique por que ainda é valioso ter "diferentes visões do mesmo problema", especialmente do ponto de vista computacional.
Explique o papel das variáveis da metalinguagem e dos esquemas de fórmulas na apresentação dos sistemas formais (℘a e ℘r). Como esses conceitos ajudam a generalizar definições e demonstrações, e qual a importância da "substituição segura" nesse contexto na Lógica de Predicados?
Analise os axiomas da Aritmética de Robinson (Bx1-Bx7) no Capítulo 7. Discuta como esses axiomas fundamentam propriedades básicas dos números naturais e as operações de adição e multiplicação, e por que eles são considerados "válidos no contexto dos modelos padrão".
Considerando os Teoremas da Incompletude de Gödel e o Teorema de Tarski, discuta as limitações fundamentais dos sistemas formais em relação à captura de propriedades e à definição da verdade na Aritmética. Qual a implicação desses resultados para a capacidade de prova em sistemas como PA?
Glossário de Termos-Chave
Lógica Proposicional (LP): Um sistema lógico no qual as unidades mais básicas são proposições atômicas, e sua verdade ou falsidade não depende de sua estrutura interna, mas apenas de como são combinadas por conectivos.
Proposição: Uma sentença declarativa que é ou verdadeira (T) ou falsa (F), mas não ambas.
Conectivo Proposicional: Símbolo usado para conectar ou modificar proposições, formando fórmulas mais complexas (e.g., ¬, ∧, ∨, →, ↔).
Fórmula (LP): Uma sequência de símbolos do alfabeto da LP que segue as regras gramaticais para ser bem formada.
Metalinguagem: A linguagem usada para falar sobre a linguagem-objeto. No texto, o português é a metalinguagem para descrever a Lógica Proposicional e de Predicados.
Variável da Metalinguagem: Símbolo usado na metalinguagem para representar elementos da linguagem-objeto (e.g., P̆ para símbolos proposicionais, H para fórmulas).
Esquema de Fórmula: Uma expressão que contém variáveis da metalinguagem e representa um conjunto de fórmulas da linguagem-objeto que seguem um padrão estrutural.
Tabela-Verdade: Uma tabela que mostra o valor de verdade de uma fórmula composta para todas as combinações possíveis de valores de verdade de suas proposições atômicas.
Interpretação (LP): Uma função que atribui um valor de verdade (T ou F) a cada símbolo proposicional em uma fórmula.
Tautologia: Uma fórmula da LP que é sempre verdadeira, independentemente da interpretação de seus símbolos proposicionais.
Satisfatibilidade (LP): Uma fórmula da LP é satisfatível se existe pelo menos uma interpretação que a torna verdadeira.
Contradição Semântica (LP): Uma fórmula da LP que é sempre falsa, independentemente da interpretação de seus símbolos proposicionais.
Contingência (LP): Uma fórmula da LP que pode ser verdadeira ou falsa, dependendo da interpretação de seus símbolos proposicionais.
Implicação Semântica (LP): Um conjunto de fórmulas β implica semanticamente uma fórmula H (β ⊨ H) se toda interpretação que torna todas as fórmulas em β verdadeiras também torna H verdadeira.
Equivalência Semântica (LP): Duas fórmulas H e G são semanticamente equivalentes (H ⊨ G e G ⊨ H) se têm o mesmo valor de verdade para todas as interpretações.
Conjunto de Conectivos Completo: Um conjunto de conectivos a partir do qual todos os outros conectivos da LP podem ser expressos de forma equivalente.
Literal (LP): Um símbolo proposicional ou sua negação.
Forma Normal Conjuntiva (FNC): Uma fórmula da LP que é uma conjunção de disjunções de literais.
Forma Normal Disjuntiva (FND): Uma fórmula da LP que é uma disjunção de conjunções de literais.
Método da Negação (Redução ao Absurdo): Um método de prova que assume a falsidade da tese e busca uma contradição para provar a tese original.
Tableaux Semânticos (LP/LPO): Um sistema de dedução que constrói uma árvore lógica para verificar a satisfatibilidade, validade ou consequência lógica de uma fórmula. Um ramo fechado indica contradição; um ramo aberto indica satisfatibilidade.
Teorema da Correção (LP/LPO): Afirma que tudo o que pode ser provado sintaticamente (e.g., via tableaux ou sistemas axiomáticos) é semanticamente válido. (Se ⊢ H, então ⊨ H).
Teorema da Completude (LP/LPO): Afirma que tudo o que é semanticamente válido pode ser provado sintaticamente. (Se ⊨ H, então ⊢ H).
Consequência Lógica Sintática (LP/LPO): Uma fórmula H é uma consequência lógica sintática de um conjunto de hipóteses β (β ⊢ H) se existe uma prova formal de H a partir de β.
Sistema Axiomático (℘a/℘r): Um sistema formal composto por um alfabeto, um conjunto de fórmulas, axiomas (fórmulas consideradas verdadeiras a priori) e regras de inferência.
Modus Ponens (MP): Uma regra de inferência que permite deduzir o consequente de uma implicação se o antecedente é verdadeiro.
Consistência de um Sistema Axiomático: Um sistema é consistente se não é possível provar uma fórmula e sua negação dentro dele.
Lógica de Predicados (LPO): Um sistema lógico que estende a LP, permitindo a representação da estrutura interna das proposições através de predicados, funções, variáveis e quantificadores.
Termo (LPO): Uma expressão que se refere a um objeto no domínio do discurso (e.g., variáveis, constantes, aplicações de funções).
Átomo (LPO): A unidade mais básica da LPO que tem um valor de verdade (e.g., um símbolo proposicional ou a aplicação de um predicado a termos).
Variável Livre: Uma ocorrência de variável em uma fórmula que não está sob o escopo de um quantificador que a quantifica.
Variável Ligada: Uma ocorrência de variável em uma fórmula que está sob o escopo de um quantificador que a quantifica.
Fórmula Fechada (Sentença): Uma fórmula da LPO que não contém variáveis livres.
Fecho Universal/Existencial: Uma fórmula obtida adicionando quantificadores universais/existenciais no início de uma fórmula para ligar todas as suas variáveis livres.
Interpretação (LPO): Uma estrutura que define um domínio do discurso e atribui significado a todos os símbolos não lógicos (constantes, símbolos de função, símbolos de predicado) e valores a variáveis livres.
Interpretação Estendida (<x←d>I): Uma interpretação que é idêntica a uma interpretação I, exceto pelo fato de que a variável x é interpretada como o elemento d do domínio.
Validade (LPO): Uma fórmula da LPO é válida se é verdadeira em todas as interpretações possíveis (para qualquer domínio e qualquer atribuição de significado aos símbolos).
Fórmula Tautologicamente Válida: Uma fórmula da LPO cuja validade pode ser determinada apenas pela sua estrutura proposicional, ignorando a estrutura interna dos átomos e quantificadores.
Aritmética de Robinson (Q): Um sistema formal na LPO com axiomas para os números naturais, sucessor, adição, multiplicação e igualdade. É incompleto para negação.
Aritmética de Peano (PA): Uma extensão da Aritmética de Robinson que inclui o axioma do princípio de indução finita.
Teoremas de Incompletude de Gödel: Resultados fundamentais que mostram que qualquer sistema formal consistente e suficientemente expressivo para a aritmética contém proposições verdadeiras que não podem ser provadas dentro do sistema, e sua própria consistência não pode ser provada dentro do sistema.
Teorema de Tarski: Afirma a impossibilidade de definir a propriedade "verdade" dentro do próprio sistema formal em que essa verdade é expressa, para sistemas suficientemente expressivos.
Indecidibilidade (LPO): A propriedade de que não existe um algoritmo que possa decidir, para qualquer fórmula da LPO, se ela possui uma determinada propriedade (e.g., satisfatibilidade ou validade) em um tempo finito garantido.
Dedução Natural: Um sistema de prova que utiliza regras de introdução e eliminação para os conectivos lógicos, permitindo a construção de provas formais.