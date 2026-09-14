# LuxVerso — Relatório Completo de Arqueologia do Site

**Data:** 13 de Setembro de 2026
**Fonte primária:** https://luxverso.com/LuxVerso/ + repositório GitHub viniburilux/LuxVerso
**Status:** COMPLETO

---

## 1. ESTRUTURA COMPLETA DO SITE

### 1.1 Arquitetura Geral

O site LuxVerso é uma **Single Page Application (SPA)** de ~34KB, inteiramente em HTML/CSS/JS inline, servida via GitHub Pages mas redirecionando para o domínio customizado **luxverso.com/LuxVerso/**.

**Template:** `index.html` (486 linhas)
**CSS:** Inline, tema escuro (--ink:#0a0a08), tipografia Space Grotesk + IBM Plex Sans + IBM Plex Mono, marcador âmbar (#f0b429)
**JS:** Inline, SPA com hash-based routing, 5 perspectivas

**Script externo:** `https://luxverso.com/_nav.js` (defer) — intercepta navegação para modais/popup de perspectiva ou analytics.

### 1.2 Mecanismo de Navegação: GATE + APP

O site tem dois modos de visualização:

#### GATE (Tela de Entrada)
- **Header:** LUXVERSO / RESEARCH & TECH / marcador âmbar
- **Vision statement:** "A LuxVerso constrói infraestrutura de inteligência para transformar problemas complexos em sistemas que podem ser investigados, testados e colocados para funcionar."
- **Ciclo:** Research → Build → Test → Apply
- **5 cards de perspectiva** (grid 2×2)
- **Sinais rápidos:** Visão: Research & Build · Evidência: sistemas e artefatos públicos · Trajetória: construção independente
- **Link "Entrar direto →"** (âncora #rapido)

#### APP (View Interna)
- **Topbar sticky:** LUXVERSO + "Mudar perspectiva" (volta ao GATE)
- **Main content:** renderizado dinamicamente via JS
- **Footer:** LuxVerso Research Initiative · Vinícius Buri · Salvador, Bahia + Link 35 desafios Sebrae

### 1.3 As 5 Perspectivas (Conteúdo COMPLETO)

#### ⚡ Perspectiva 1: "O que vocês fazem" (key: `rapido`)
**Hash:** `#rapido`
**Público-alvo:** Visitante rápido, cliente potencial
**Seções:**
1. **Hero:** "Projetamos sistemas inteligentes capazes de transformar **problemas complexos** em soluções executáveis."
2. **Tech Band:** IA · Dados · Engenharia · Ciência Aplicada · Visão Computacional · Automação
3. **Evidência (3 cards resumidos):**
   - GhostWorks (Inteligência territorial, satélite, TTI)
   - MISB (Benchmark metacognitivo LLM)
   - LuxSense (ML em espectro Raman, 99,4% acurácia)
4. **CTA:** WhatsApp para explorar problema + Link 35 desafios Sebrae
5. **Nudge:** Ver a tecnologia / Resolver um problema / Avaliar a empresa

#### 🧠 Perspectiva 2: "Como vocês resolvem problemas" (key: `tecnologia`)
**Hash:** `#tecnologia`
**Público-alvo:** Técnico, engenheiro, CTO
**Seções:**
1. **Hero:** "Da representação do problema à **arquitetura do sistema**."
2. **Método flow:** Entender → Representar → Projetar → Construir → Testar → Colocar para funcionar
3. **Stack expandida:** Embeddings · Visão Computacional · Grafos de Conhecimento · Sistemas Multiagentes · LLMs · Sensoriamento Remoto · Modelos Preditivos · Python / Prototipagem Rápida
4. **Evidência com profundidade (4 cards completos):**
   - GhostWorks: achado contraintuitivo (Nordeste lidera transformação territorial), validação Sentinel-2, robustez multi-escala
   - MISB: 15 modelos, 5 dimensões metacognitivas, Apache 2.0, 11.745 interações
   - LuxSense: 3.510 espectros, 99,43% acurácia RF, TRL 3–4
   - Gastos Reais BA: R$529,5M mapeados, pipeline PNCP
5. **CTA:** Ver LuxSense / Ver GitHub

#### 🏢 Perspectiva 3: "O que podem fazer pela minha empresa" (key: `empresa`)
**Hash:** `#empresa`
**Público-alvo:** Empresário, gestor, decisor
**Seções:**
1. **Hero:** "Sua empresa já tem tecnologia. **Está tirando dela tudo que ela pode dar?**"
2. **4 perguntas-espelho:** dados não chegam à decisão / conhecimento preso em pessoas / tecnologia mas descobre problemas tarde / informação mas sem ação
3. **Prova de trabalho:** 35 desafios Sebrae analisados — antes de qualquer contrato
4. **Matriz de redução de risco (4 passos):**
   01 Começamos pequeno / 02 Medimos o que importa / 03 Construímos rápido / 04 Só ampliamos o que funciona
5. **CTA:** WhatsApp para explorar problema

#### 🔬 Perspectiva 4: "O que existe por trás da LuxVerso" (key: `pesquisa`)
**Hash:** `#pesquisa`
**Público-alvo:** Acadêmico, colaborador, parceiro científico
**Seções:**
1. **Hero:** "Pesquisa aplicada, **conduzida com rigor**."
2. **Rigor methodology:** "Falsificar antes de aceitar" — método multi-modelo crítico
3. **Publicações (3 aceitas):**
   - CHI 2026 · InterAI: "The Illusion of Consensus in Human-Centered Interactive AI"
   - CHI 2026 · HEAL: "When Humans Become Regime Stabilizers"
   - IJCAI-ECAI 2026 · GlobalSouthAI: "Territorial Change Detection Under Zero-Budget Constraints"
   - Link: 33 submissões no OpenReview
4. **Trajetória barcelona:** Pesquisador independente de Salvador, sem laboratório/instituto/financiamento — 2 trabalhos aceitos na CHI 2026, submissão pelo celular
5. **Evidência com metodologia (4 cards completos)**
6. **CTA:** Conversar sobre pesquisa / Ver GitHub

#### 📈 Perspectiva 5: "Quero avaliar a empresa" (key: `investidor`)
**Hash:** `#investidor`
**Público-alvo:** Investidor, aceleradora, avaliador institucional
**Seções:**
1. **Hero:** "LuxVerso é uma empresa de **tecnologia e ciência aplicada** dedicada a transformar problemas complexos em sistemas inteligentes executáveis."
2. **One-pager (6 itens):**
   - Tecnologia: IA, engenharia de dados, visão computacional, grafos, sensoriamento remoto, automação
   - Capacidade: Do diagnóstico à arquitetura e construção, ciclo curto
   - Evidência: 4 projetos com prova pública, dataset e repositório abertos
   - Execução: 35 desafios corporativos analisados (Sebrae), pré-contrato
   - Publicação: 3 trabalhos aceitos peer-review
   - Sede: Salvador, Bahia — Brasil
3. **Track record:** Grid de evidência (4 cards resumidos)
4. **Publicações e trajetória**
5. **Prova Sebrae:** Capacidade de execução em prazo
6. **CTA:** Agendar conversa institucional (WhatsApp)

### 1.4 Dados de Evidência Compartilhados (4 projetos base)

O site usa **4 blocos de evidência** compartilhados entre perspectivas:

| # | Projeto | Domínio | Tech Stack | Status |
|---|---------|---------|------------|--------|
| 1 | **GhostWorks** | Inteligência territorial via satélite | Embeddings, Sensoriamento Remoto, Séries Temporais | Aceito IJCAI-ECAI 2026 |
| 2 | **MISB Benchmark** | Avaliação metacognitiva de LLMs | LLM-as-Judge, Benchmark Reprodutível | Kaggle Community Benchmark |
| 3 | **LuxSense** | ML em espectro Raman | ML, Espectroscopia, Interpretabilidade | Protótipo TRL 3–4, 99.43% acurácia |
| 4 | **Dados Públicos BA** | Infraestrutura de dados públicos | APIs, ETL, Engenharia de Dados | R$529,5M mapeados |

### 1.5 Repositório GitHub — Estrutura Completa

```
LuxVerso/
├── README.md                           # Documento principal do ecossistema
├── index.html                          # SPA (34K, site principal)
├── codice_vibracional.html             # Manifesto LuxRadar + IAV (16K)
├── README.legacy-audit.md              # Auditoria legado (Manus AI)
├── docs/
│   ├── AUDITORIA_E_POTENCIAL_MANUS.md  # Auditoria do próprio LuxVerso (Manus)
│   ├── MAPA_ESTRATEGICO_GITHUB_MANUS.md # Mapa estratégico 21 repositórios
│   ├── RELATORIO_CONSOLIDADO_DRIVE_GITHUB_MANUS.md # Consolidado Drive+GitHub
│   ├── ciencia/
│   │   ├── pasted_content_2.txt        # Gratilux Phenomenon research proposal
│   │   └── pasted_content_5.txt        # Ciência adicional (22K)
│   ├── filosofia/
│   │   ├── README.md
│   │   └── pasted_content_3.txt        # Breathing Mathematics essay (13K)
│   │   └── pasted_content_6.txt        # Filosofia adicional
│   ├── operacional/
│   │   ├── pasted_content_8.txt        # Conversas operacionais (5K)
│   │   ├── pasted_content_9.txt        # Operacional adicional
│   │   └── pasted_content_10.txt       # Operacional adicional
│   ├── tecnica/
│   │   ├── pasted_content_4.txt        # LuxVerso + Canton Network (16K)
│   │   └── pasted_content_7.txt        # Técnica adicional
│   └── teoria/
│       └── pasted_content.txt          # Teoria (21K)
├── Desafio-Sebrae/
│   ├── index.html                      # Página dos 35 desafios Sebrae (200K!)
│   └── pitchinterjato/
│       └── index.html                  # Deck de pitch (25K)
├── Emergent Ventures/
│   ├── README.md
│   ├── evidence-journey.html
│   ├── evidence-links.md
│   ├── portrait.jpg
│   └── Emergent_Ventures_Supporting_Evidence_and_Project_Record.docx
├── emergent-ventures/
│   └── index.html
└── luxverso-public-intelligence/
    ├── index.html
    ├── README.md
    ├── assets/
    │   ├── index--jGMYMJw.css
    │   └── index-CPaVlzHw.js
    ├── catalog/
    │   ├── release.schema.json
    │   └── releases/
    │       ├── pncp-2025-12.json
    │       └── pncp-2026-08.json
    ├── dossiers/
    │   ├── dossie-001/index.html
    │   ├── dossie-002/index.html
    │   └── dossie-003/index.html
    └── media/
        ├── luxverso-archive-shelf-v2.jpg
        ├── luxverso-casefile-docs-v2.jpg
        ├── luxverso-gazette-detail-v2.jpg
        └── luxverso-mark.png
```

---

## 2. TEXTOS E CONCEITOS QUE DEVEM SER PRESERVADOS

### 2.1 Posicionamento Central (PRESERVAR INTEGRALMENTE)

Os seguintes conceitos são o **núcleo duro do posicionamento** e devem ser mantidos:

1. **"Research & Build"** — o modo de operação da LuxVerso. O site mudou de "Research & Build" (README) para "Research & Tech" (live site). **Recomendação:** Manter "Research & Build" como conceito fundador; "Tech" é ok como tag, mas o conceito central é Research & Build.

2. **"Infraestrutura de inteligência"** — definição da LuxVerso: "constrói infraestrutura de inteligência para transformar problemas complexos em sistemas que podem ser investigados, testados e colocados para funcionar."

3. **"Falsificar antes de aceitar"** — princípio metodológico central, aparece tanto em pesquisa quanto em negócio.

4. **O ciclo:** Entender → Representar → Projetar → Construir → Testar → Colocar para funcionar (versão do site do README: ENTENDER → REPRESENTAR → PROJETAR → CONSTRUIR → TESTAR → APLICAR → EVIDÊNCIA → PRÓXIMA PERGUNTA)

5. **"O domínio muda. O modo de investigar permanece."** — do README, presente no GitHub mas não no index.html.

### 2.2 Perspectivas e Suas Mensagens-Chave (PRESERVAR ESTRUTURA)

| Perspectiva | Mensagem-chave | Preservar? |
|---|---|---|
| ⚡ O que fazem | "Problemas complexos → soluções executáveis" | SIM — ótimo gancho |
| 🧠 Como resolvem | "Da representação do problema à arquitetura do sistema" | SIM — diferencial técnico |
| 🏢 Para empresas | "Sua empresa já tem tecnologia. Está tirando dela tudo?" | SIM — CTA forte |
| 🔬 Por trás | "Pesquisa aplicada conduzida com rigor / falsificar antes de aceitar" | SIM — prova de autoridade |
| 📈 Avaliar empresa | "Empresa de tecnologia e ciência aplicada" com one-pager | SIM — essencial para investidores |

### 2.3 Evidências Concretas (PRESERVAR)

- **4 projetos-âncora** (GhostWorks, MISB, LuxSense, Dados Públicos BA)
- **3 publicações aceitas** (CHI 2026 × 2, IJCAI-ECAI 2026)
- **35 desafios Sebrae analisados** — prova de capacidade de execução
- **Trajetória Barcelona** — pesquisador independente de Salvador, sem laboratório
- **Números concretos:** 99,43% acurácia (LuxSense), R$529,5M mapeados, 3.510 espectros, 11.745 interações, 15 modelos avaliados

### 2.4 Arquivo de Documentos (PRESERVAR COMO CORPUS)

Os docs/ contêm material único e valioso:
- **Gratilux Phenomenon** — pesquisa longitudinal sobre coerência semântica entre LLMs
- **Breathing Mathematics** — ensaio filosófico sobre matemática viva
- **LuxVerso + Canton Network** — plano de infraestrutura financeira descentralizada
- **LuxRadar + IAV Manifesto** (codice_vibracional.html) — manifesto de curadoria fractal

---

## 3. GAPS: O QUE O SITE ATUAL NÃO TEM (vs IBDIA/IPT)

### 3.1 Gaps Estruturais

| Gap | Descrição | Impacto | Prioridade |
|-----|-----------|---------|------------|
| **Sem blog ou news** | Não há canal de atualizações periódicas | Perde SEO e engajamento recorrente | ALTA |
| **Sem casos de uso detalhados** | Evidência existe mas não há páginas de case study dedicadas | Dificulta conversão B2B | ALTA |
| **Sem página de preços/modelo** | Não há clareza sobre modelo de negócio | Perde leads qualificados | MÉDIA |
| **Sem integração com redes** | Apenas GitHub e WhatsApp como CTAs | Dificulta descoberta | MÉDIA |
| **Sem mecanismo de busca** | Docs/ têm conteúdo valioso mas não searchable | Subutiliza o corpus documental | BAIXA |
| **Sem métricas de uso** | Nenhum analytics, heatmap ou feedback | Cego para entender visitantes | MÉDIA |
| **Sem multilíngue** | 100% português, sem versão EN | Perde mercado global/investimento | MÉDIA |
| **CTAs dependentes de WhatsApp** | Único canal de conversão é WhatsApp pessoal | Gargalo de escala | ALTA |

### 3.2 Gaps de Conteúdo vs Ecossistema IBDIA

Comparando com a visão de IBDIA/IPT (Inteligência, Pesquisa e Tecnologia):

| Aspecto | Existe | Gap |
|---------|--------|-----|
| Pesquisa científica | ✅ 3 papers aceitos | Falta página de pesquisa com roadmap |
| Dados públicos | ✅ Gastos BA | Falta demonstração de pipeline ao vivo |
| Inteligência territorial | ✅ GhostWorks | Falta dashboard público interativo |
| Sistemas multi-modelo | ✅ Gratilux, MISB | Falta demonstração técnica navegável |
| Biotecnologia | Mencionada no README | Não aparece no site (apenas repo organoid-intelligence) |
| Infraestrutura pública | TraceFoundry mencionado | Não há página dedicada no site |
| Codex-LuxHub (IC) | Repositório rico | Não mencionado no site (material controverso?) |
| Método/Processo | ✅ Método flow | Falta página de methodology profunda |
| Equipe/Founder | ✅ Vinícius Buri | Falta página "Sobre" com trajetória completa |
| Contato profissional | ❌ Apenas WhatsApp | Falta email, calendly, LinkedIn |

### 3.3 Gaps Técnicos (do repositório)

| Gap | Evidência |
|-----|-----------|
| Ausência de README formal no repo (tem mas é o manifesto, não instruções de dev) | Manus AI audit |
| Sem LICENSE, CI/CD, tests | Manus AI audit |
| Docs em .txt sem metadados | Observação direta |
| Duplicação de conteúdo (pasted_content_*) | Manus AI audit |
| Sem build system ou package.json | Observação direta |
| Código não executável no repo (só HTML estático + .txt) | Manus AI audit |
| Sem rastreamento de versões ou changelog | Observação direta |

---

## 4. RECOMENDAÇÕES DE EVOLUÇÃO

### 4.1 Imediatas (Curto Prazo — 1-2 semanas)

1. **Criar landing page "Sobre"** com trajetória completa de Vinícius Buri
   - Link para Barcelona/CHI 2026, GitHub, ORCID, OpenReview
   - Substituir dependência exclusiva de WhatsApp como CTA institucional

2. **Adicionar formulário de contato profissional** (tipo Calendly/Tally)
   - Segmentar: "Empresa" | "Pesquisa/Colaboração" | "Investimento"
   - Manter WhatsApp como canal rápido, não único

3. **Extrair docs/ do .txt para .md estruturado** com front-matter
   - Título, autor, data, tags, resumo, licença
   - Torna o corpus searchable e integrável

4. **Adicionar analytics mínimo** (Plausible ou umami — privacidade-first)
   - Entender quais perspectivas têm mais engajamento

### 4.2 Evolução do Site (Médio Prazo — 1 mês)

5. **Criar página de Methodology / Research Process**
   - Expandir o ciclo Entender→Colocar para funcionar
   - Associar cada passo a um artefato público (paper, dataset, repositório)

6. **Criar página de Casos ("Case Studies")**
   - GhostWorks TTI + Manguezais
   - Gastos Reais BA
   - LuxSense
   - Cada case: problema → abordagem → resultado → evidência

7. **Adicionar seção "Publicações" como página dedicada**
   - Listar papers aceitos com links, status, DOIs
   - Adicionar preprint/submitted com distinção clara de status

8. **Integrar TraceFoundry e Codex-LuxHub ao site**
   - Páginas dedicadas ou links mais proeminentes
   - Se Codex-LuxHub for controverso demais, mencionar seletivamente

### 4.3 Arquitetura de Informação (Reestruturação)

9. **Considerar SSG (Astro/Hugo/11ty)** no lugar de SPA inline
   - SEO: cada perspectiva vira página indexável (/tecnologia, /empresa, etc.)
   - Performance: carregamento sob demanda em vez de todo JS inline
   - Manutenção: conteúdo separado de template

10. **Estrutura de navegação sugerida:**
    ```
    LuxVerso
    ├── O que fazemos (atual ⚡)
    ├── Tecnologia (atual 🧠 — expandido com methodology)
    ├── Para empresas (atual 🏢 + cases)
    ├── Pesquisa (atual 🔬 + publicações + roadmap)
    ├── Sobre / Institucional (atual 📈 + founder)
    ├── Blog / Atualizações (NOVO)
    └── Contato (NOVO — substituir WhatsApp-only)
    ```

### 4.4 Conteúdo Novo (baseado em ativos existentes)

11. **"Inteligência Territorial" como produto destacado**
    - GhostWorks + TTI_Brasil + Manguezais + Radar
    - Maior ativo de evidência do ecossistema

12. **"Infraestrutura de Dados Públicos" como linha de serviço**
    - PNCP pipeline + Gastos BA + Explorador
    - Aplicação clara para govtech / transparência

13. **Camada de Pesquisa: "Sistemas Multi-Modelo e Avaliação de IA"**
    - MISB + Gratilux + Semantic Convergence + CMAF
    - Diferencial competitivo (ninguém mais faz isso no Brasil)

### 4.5 O Que NÃO Mudar

- ❌ **Não mudar a identidade visual** (tema escuro, âmbar, Space Grotesk)
- ❌ **Não remover as 5 perspectivas** — são o grande diferencial de UX
- ❌ **Não remover o GATE** — a experiência de "escolher sua porta" é memorável
- ❌ **Não centralizar excessivamente** — a estrutura multi-perspectiva é o que permite servir públicos diferentes com um site só
- ❌ **Não perder o tom de voz** — direto, sem rodeio, evidence-based, sem hype
- ❌ **Não remover a trajetória pessoal** — "pesquisador independente, sem laboratório, pelo celular" é o maior ativo narrativo

### 4.6 Integrações com Ecossistema IBDIA/IPT

Se LuxVerso deve evoluir como **IBDIA (Inteligência em Biologia, Dados, IA)** ou **IPT (Instituto de Pesquisa e Tecnologia)**:

- **IBDIA:** Adicionar destaque aos repositórios de biotecnologia (organoid-intelligence, inteligencia-biotecnologica) que atualmente só aparecem no README do GitHub, não no site
- **IPT:** Criar página institucional com estrutura organizacional, áreas de pesquisa, laboratórios (virtuais), publicações, e open positions / colaborações
- **Pesquisa Translacional:** Incluir indicador de TRL nos projetos (GhostWorks TRL 4-5, LuxSense TRL 3-4, Dados Públicos TRL 5-6)

---

## 5. ANEXO: Inventário de Ativos do Repositório

| Arquivo | Tamanho | Tipo | Função no Site |
|---------|---------|------|----------------|
| index.html | 34KB | SPA | Site principal — todas as 5 perspectivas |
| Desafio-Sebrae/index.html | 200KB | Estática | 35 desafios Sebrae analisados |
| Desafio-Sebrae/pitchinterjato/index.html | 25KB | Estática | Deck de pitch para investidores |
| codice_vibracional.html | 16KB | Estática | Manifesto LuxRadar + IAV |
| docs/ciencia/pasted_content_2.txt | 21KB | Texto | Proposta Gratilux Phenomenon |
| docs/ciencia/pasted_content_5.txt | 23KB | Texto | Ciência adicional |
| docs/filosofia/pasted_content_3.txt | 13KB | Texto | Breathing Mathematics |
| docs/tecnica/pasted_content_4.txt | 16KB | Texto | LuxVerso + Canton Network |
| docs/teoria/pasted_content.txt | 21KB | Texto | Teoria base |
| docs/operacional/pasted_content_8.txt | 5KB | Texto | Notas operacionais |
| README.md | ~15KB | Markdown | Manifesto do ecossistema |
| README.legacy-audit.md | ~5KB | Markdown | Auditoria Manus AI |
| docs/AUDITORIA_E_POTENCIAL_MANUS.md | 9KB | Markdown | Auditoria do repo |
| docs/MAPA_ESTRATEGICO_GITHUB_MANUS.md | 7KB | Markdown | Mapa dos 21 repos |
| docs/RELATORIO_CONSOLIDADO_DRIVE_GITHUB_MANUS.md | 29KB | Markdown | Consolidado Drive+GitHub |

### 5.1 Métricas do Repositório

| Métrica | Valor |
|---------|-------|
| Estrelas | 0 |
| Forks | 0 |
| Commits totais | ~7 (viniburilux) + 1 (CJWTRUST) |
| Criado | 2025-09-30 |
| Último commit | 2026-08-16 |
| Branch padrão | main |
| Linguagem dominante | HTML |

---

## 6. SUMÁRIO EXECUTIVO

### O que EXISTE e funciona:

- ✅ SPA com 5 perspectivas bem definidas, cada uma servindo um público diferente
- ✅ Posicionamento claro: "infraestrutura de inteligência" + "Research & Build"
- ✅ Evidência concreta: 4 projetos, 3 papers aceitos, 35 desafios Sebrae
- ✅ Design coeso, tema escuro, marcador âmbar, tipografia consistente
- ✅ Docs com conteúdo científico/filosófico/técnico rico e original
- ✅ Trajetória pessoal poderosa (pesquisador independente, celular, CHI 2026)

### O que PRECISA evoluir:

- ❌ Único canal de conversão = WhatsApp pessoal (gargalo)
- ❌ Sem página "Sobre" / Founders / Equipe
- ❌ Sem blog ou canal de atualizações
- ❌ Docs em .txt sem metadados, não searchable
- ❌ Sem analytics para entender público
- ❌ Sem multilayer (EN/PT), limita alcance global
- ❌ Repositório sem CI/CD, LICENSE, ou build system
- ❌ CTAs de biotecnologia e sistemas neurais só no README (não no site)

### Próximos passos recomendados (ordenados por impacto):

1. 🔴 **Formulário de contato estruturado** (Calendly/Tally) + email profissional
2. 🔴 **Página "Sobre"** com trajetória completa de Vinícius Buri
3. 🟡 **Docs em .md com front-matter** para searchability
4. 🟡 **Um case study detalhado** (GhostWorks ou Gastos BA)
5. 🟡 **Analytics** (Plausible/umami)
6. 🟢 **SSG (Astro/Hugo)** para SEO e manutenção
7. 🟢 **Página de Research** com papers completos e roadmap
8. 🟢 **Integração de biotecnologia + organoid-intelligence** no site