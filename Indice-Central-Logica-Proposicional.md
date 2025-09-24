# Índice Central de Lógica Proposicional

## Arquivo Principal para Consulta de IA em Questões de Lógica

Este documento serve como **ponto de entrada central** para uma IA responder questões de lógica proposicional, fornecendo um mapa conceitual organizado com referências direcionadas aos arquivos especializados do repositório.

---

## Conceitos Fundamentais (Quick Reference)

### Definições Essenciais
- **Proposição**: Sentença declarativa que pode ser verdadeira (V) ou falsa (F)
- **Fórmula Atômica**: Proposição mais simples (p, q, r, s...)
- **Fórmula Molecular**: Proposições combinadas por conectivos lógicos
- **Conectivos Verofuncionais**: ¬, ∨, ∧, →, ↔ (princípio da composicionalidade)

### Operadores Lógicos (Tabelas-Verdade)
- **Negação (¬)**: Inverte valor de verdade
- **Disjunção (∨)**: Verdadeira se pelo menos uma proposição for verdadeira
- **Conjunção (∧)**: Verdadeira apenas se ambas proposições forem verdadeiras
- **Implicação (→)**: Falsa apenas quando antecedente verdadeiro e consequente falso
- **Equivalência (↔)**: Verdadeira quando ambas têm mesmo valor de verdade

### Classificação Semântica
- **Tautologia**: Sempre verdadeira (todas as interpretações)
- **Contradição**: Sempre falsa (todas as interpretações)
- **Contingência**: Verdadeira em algumas interpretações, falsa em outras

---

## Métodos de Análise e Prova

### 1. Formalização de Argumentos
**→ Ver arquivo completo:** [Formalizacao-e-Analise-Logica-Proposicional-com-Tablos.md](./Formalizacao-e-Analise-Logica-Proposicional-com-Tablos.md)

**Processo essencial:**
1. Identificar proposições atômicas na linguagem natural
2. Atribuir variáveis proposicionais (P, Q, R...)
3. Reconhecer conectivos lógicos ("e", "ou", "se...então", "não")
4. Aplicar precedência: ¬ > (→, ↔) > (∨, ∧)
5. Estruturar como (P1 ∧ P2 ∧ ... ∧ Pn) → C

**Casos especiais importantes:**
- Condição necessária: "P é necessário para Q" → Q → P
- Condição suficiente: "P é suficiente para Q" → P → Q
- "A menos que": "P, a menos que Q" → ¬Q → P

### 2. Dedução Natural
**→ Ver arquivo completo:** [Deducao-Natural-e-Tablos-Semanticos-Guia-Pratico.md](./Deducao-Natural-e-Tablos-Semanticos-Guia-Pratico.md)

**Três métodos principais:**

#### A) Método Direto
- Aplicar regras de introdução e eliminação diretamente
- **Regras chave**: Modus Ponens (→e), Introdução ∧ (∧i), Eliminação ∧ (∧e)

#### B) Provas Hipotéticas
- Para conclusões do tipo A → B
- Assumir hipótese [A], derivar B, descarregar hipótese
- **Regra**: Introdução da Implicação (→i)

#### C) Prova por Contradição
- Assumir ¬A, derivar contradição ⊥, concluir A
- **Técnica**: Redução ao Absurdo

### 3. Tablôs Semânticos
**→ Ver arquivos:** [Logica-Proposicional_Sintaxe-Semantica-e-Tablos.md](./Logica-Proposicional_Sintaxe-Semantica-e-Tablos.md)

**Procedimento para validação:**
1. Para provar validade de argumento: negar (P1 ∧ P2 ∧ ... ∧ Pn) → C
2. Aplicar regras R1-R9 sistematicamente
3. **Heurística**: Priorizar regras não-bifurcantes (R1, R5, R7, R8)
4. **Resultado**: Se todos ramos fecham → válido; se ramo aberto → inválido (contraexemplo)

---

## Análise Semântica

### Função Interpretação
**→ Ver arquivo:** [Fundamentos-da-Logica-Proposicional_Semantica-e-Classificacoes.md](./Fundamentos-da-Logica-Proposicional_Semantica-e-Classificacoes.md)

- **I[P]**: Atribui V ou F a cada proposição atômica
- **Princípio da Composicionalidade**: Valor de fórmula complexa depende dos valores das partes
- **Definições formais** de todos os conectivos via função interpretação

### Consequência Lógica
- **Sintática (⊢)**: Dedutível por regras de inferência
- **Semântica (⊨)**: Toda interpretação que torna premissas verdadeiras, torna conclusão verdadeira
- **Equivalência**: Na LP clássica, ⊢ ≡ ⊨ (Correção + Completude)

---

## Referências Técnicas Especializadas

### Para Operadores e Interconversão
**→ [Logica-Proposicional_Operadores-Verofuncionais-Interconversao.md](./Logica-Proposicional_Operadores-Verofuncionais-Interconversao.md)**
- Definições formais completas de todos operadores
- Tabelas-verdade detalhadas
- Equivalências lógicas e transformações

### Para Material Acadêmico Oficial
**→ [lc1-2025-2-notas-de-aulas.pdf](./lc1-2025-2-notas-de-aulas.pdf)**
- Curso oficial UnB - Lógica Computacional 1
- Teoria completa: LPM → LPI → LPC
- Demonstrações de Correção e Completude

### Para Guia Abrangente
**→ [Guia-Essencial-de-Logica-para-Computacao.md](./Guia-Essencial-de-Logica-para-Computacao.md)**
- Glossário completo de termos técnicos
- Questões práticas e exercícios resolvidos
- Aplicações em Ciência da Computação

---

## Instruções para IA

### Fluxo de Trabalho Recomendado

1. **Análise da Questão**
   - Identificar tipo: formalização, prova, validação, classificação semântica
   - Determinar se é exercício teórico ou aplicação prática

2. **Seleção de Método**
   - **Formalização**: Usar processo do arquivo de Formalização
   - **Prova**: Escolher entre Dedução Natural ou Tablôs conforme complexidade
   - **Validação**: Priorizar Dedução Natural para verificação mecânica
   - **Análise Semântica**: Consultar arquivo de Fundamentos

3. **Consulta aos Arquivos**
   - **NUNCA inventar regras ou definições**
   - Sempre referenciar arquivos específicos para detalhes técnicos
   - Citar exemplos dos arquivos quando relevante

4. **Estrutura da Resposta**
   - Começar com definições relevantes (deste índice)
   - Mostrar passo-a-passo detalhado do método escolhido
   - Justificar cada inferência com regra específica
   - Concluir com verificação/validação quando aplicável

### Casos Especiais
- **Argumentos inválidos**: Usar tablôs para extrair contraexemplo
- **Fórmulas complexas**: Quebrar em subfórmulas antes de analisar
- **Ambiguidades**: Sempre explicitar precedência de operadores
- **Provas longas**: Estruturar em subprovas com hipóteses bem marcadas

### Lições Técnicas para Provas Formais

1. **Reconhecimento de Implicações Aninhadas**
   - Aplicar regra →i recursivamente para provar fórmulas do tipo A → (B → C)
   - Interpretar associatividade à direita: A → B → C significa A → (B → C)
   - Manter controle rigoroso da profundidade e escopo de cada hipótese
   - Estruturar subprovas dentro de subprovas, preservando dependências

2. **Gestão de Escopo de Hipóteses**
   - Distinguir entre **usar** uma hipótese (aplicação em regras como MP) e **descarregá-la** (→i)
   - Manter registro das hipóteses ativas no "conjunto de premissas" (Γ no sequente Γ ⊢ φ)
   - Apenas regras de introdução (→i, ∨i, etc.) descarregam hipóteses
   - Regras de eliminação apenas usam hipóteses, sem removê-las do escopo

3. **Interpretação do ⊢ (Turnstile)**
   - O símbolo ⊢ em Γ ⊢ φ representa um **objetivo** a ser alcançado/derivado
   - Não indica uma fórmula já provada ou descartada
   - Deve ser entendido como "a partir de Γ, podemos derivar φ"
   - Em sequentes, o lado esquerdo (Γ) contém todas as premissas e hipóteses ativas

4. **Ordem de Descarregamento**
   - Hipóteses DEVEM ser descarregadas na ordem inversa em que foram assumidas
   - Ordem incorreta gera implicações mal-formadas ou inválidas
   - Analogia: estrutura LIFO (Last-In-First-Out) como uma pilha
   - Verificar dependências antes de descarregar (hipóteses internas não podem depender de externas)

5. **Detalhes da Notação**
   - Justificar cada linha com regra aplicada e linhas das quais foi derivada
   - Marcar claramente hipóteses temporárias: [A]ᵏ ou [A]ⁿ (com índice ou numeração)
   - Indicar explicitamente o descarregamento com notação como →i [k]
   - Alinhar subprovas com indentação para visualizar escopo
   - Documentar o conjunto ativo de premissas em cada etapa da prova

6. **Notação e Representação em Árvore**
   - Justificativa: Cada passo de inferência na árvore deve ser justificado com o nome da regra (ex: →e, →i, Ax).

   - Hipóteses Temporárias: Marque claramente as hipóteses com colchetes e um índice numérico para indicar sua ordem, ex: [p]¹, [p → q]².

   - Axioma (Ax): Use (Ax) para indicar que uma fórmula é uma hipótese assumida naquela linha da prova. O sequente φ ⊢ φ é um axioma.

   - Descarregamento Explícito: Ao aplicar a regra →i, indique qual hipótese está sendo descarregada usando seu índice. Ex: (→i)¹.

   - Estrutura Visual: A árvore organiza visualmente as dependências. As premissas de uma regra ficam acima da linha, e a conclusão, abaixo. Isso torna o escopo de cada subprova evidente.

   
**Exemplo de Aplicação da Notação em Árvore:**

Para provar ⊢ (p → q → r) → (p → q) → p → r:
```
      [p]³         [p → q]²              [p]³    [p → (q → r)]¹
      ---- (Ax)    -------- (Ax)          ---- (Ax) ----------- (Ax)
      p ⊢ p        p→q ⊢ p→q              p ⊢ p   p→(q→r)⊢p→(q→r)
      -------------------- (→e)          ------------------------- (→e)
             p, [p→q]² ⊢ q                     p, [p→(q→r)]¹ ⊢ q→r
      ------------------------------------------------------------------ (→e)
                         [p→(q→r)]¹, [p→q]², [p]³ ⊢ r
                  ---------------------------------------------------- (→i)³
                          [p→(q→r)]¹, [p→q]² ⊢ p → r
                   --------------------------------------------------- (→i)²
                           [p→(q→r)]¹ ⊢ (p → q) → p → r
                    -------------------------------------------------- (→i)¹
                            ⊢ (p → q → r) → (p → q) → p → r
```

---

## Arquivos de Apoio por Tópico

| Tópico | Arquivo Principal | Uso |
|--------|------------------|-----|
| Formalização | `Formalizacao-e-Analise-Logica-Proposicional-com-Tablos.md` | Traduzir linguagem natural → lógica |
| Dedução Natural | `Deducao-Natural-e-Tablos-Semanticos-Guia-Pratico.md` | Construir provas sintáticas |
| Tablôs Semânticos | `Logica-Proposicional_Sintaxe-Semantica-e-Tablos.md` | Verificação mecânica de validade |
| Semântica | `Fundamentos-da-Logica-Proposicional_Semantica-e-Classificacoes.md` | Análise de interpretações |
| Operadores | `Logica-Proposicional_Operadores-Verofuncionais-Interconversao.md` | Definições e equivalências |
| Teoria Completa | `lc1-2025-2-notas-de-aulas.pdf` | Fundamentação matemática |
| Guia Geral | `Guia-Essencial-de-Logica-para-Computacao.md` | Glossário e exercícios |

---

**Nota para IA**: Este índice deve ser sua primeira consulta. Para detalhes específicos, sempre referencie os arquivos especializados indicados. Mantenha rigor formal e cite as fontes adequadas para cada conceito ou regra utilizada.