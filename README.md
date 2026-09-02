Aqui está a tradução completa para o português do Brasil (pt-BR):

---

# 🎭 The Agency: Especialistas em IA Prontos para Transformar seu Fluxo de Trabalho

> **Uma agência de IA completa ao seu alcance** — De magos do frontend a ninjas de comunidades no Reddit, de injetores de criatividade e bom humor a verificadores de realidade. Cada agente é um especialista dedicado com personalidade, processos e entregáveis comprovados.

[![GitHub stars](https://img.shields.io/github/stars/msitarzewski/agency-agents?style=social)](https://github.com/msitarzewski/agency-agents)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
[![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-pink?logo=github)](https://github.com/sponsors/msitarzewski)
[![Download the app](https://img.shields.io/github/v/release/msitarzewski/agency-agents-app?label=Download%20app&color=2563eb)](https://github.com/msitarzewski/agency-agents-app/releases/latest)

> ### 🆕 Agora temos um aplicativo
>
> O **[Agency Agents](https://agencyagents.app)** é um aplicativo nativo para **macOS, Linux e Windows** que permite navegar por todo o catálogo de agentes e instalá-los no Claude Code, Cursor, Codex, Gemini, Osaurus e outros — com apenas um clique. Sem necessidade de clonar repositórios, sem scripts e com atualizações automáticas.
>
> **→ [Baixar a versão mais recente](https://github.com/msitarzewski/agency-agents-app/releases/latest) · [agencyagents.app](https://agencyagents.app)**

---

## 🚀 O que é isso?

Nascido de uma thread no Reddit e de meses de iteração, **The Agency** é uma coleção crescente de personas de agentes de IA meticulosamente construídas. Cada agente é:

- **🎯 Especializado**: Conhecimento profundo em seu domínio (não são modelos de prompts genéricos)
- **🧠 Orientado por Personalidade**: Voz, estilo de comunicação e abordagem únicos
- **📋 Focado em Entregáveis**: Código real, processos claros e resultados mensuráveis
- **✅ Pronto para Produção**: Fluxos de trabalho testados em batalha e métricas de sucesso definidas

**Pense nisto como**: Montar o time dos seus sonhos, só que formado por especialistas em IA que nunca dormem, nunca reclamam e sempre entregam.

---

## ⚡ Início Rápido

### Opção 1: Instalar o aplicativo (Recomendado)

A maneira mais rápida — sem clone, sem terminal. O [**Agency Agents**](https://agencyagents.app) é um aplicativo desktop nativo (macOS · Linux · Windows) que navega por todo o catálogo e instala os agentes no Claude Code, Cursor, Codex, Gemini CLI, OpenCode, Qwen e Osaurus para você, mantendo-os sempre atualizados.

**[⬇ Baixar a versão mais recente](https://github.com/msitarzewski/agency-agents-app/releases/latest)** — ou no Mac:

```bash
brew install --cask msitarzewski/agency-agents/agency-agents
```

Prefere a linha de comando? As opções baseadas em scripts abaixo instalam os mesmos agentes.

### Opção 2: Usar com o Claude Code

```bash
# Instala todos os agentes no diretório do Claude Code
./scripts/install.sh --tool claude-code

# Ou copie manualmente uma categoria se desejar apenas uma divisão
cp engineering/*.md ~/.claude/agents/

# Em seguida, ative qualquer agente nas suas sessões do Claude Code:
# "Ei Claude, ative o modo Frontend Developer e me ajude a criar um componente React"
```

### Opção 3: Usar como Referência

O arquivo de cada agente contém:
- Identidade e traços de personalidade
- Missão principal e fluxos de trabalho
- Entregáveis técnicos com exemplos de código
- Métricas de sucesso e estilo de comunicação

Navegue pelos agentes abaixo e copie/adapte os que precisar!

### Opção 4: Usar com Outras Ferramentas (GitHub Copilot, Antigravity, Gemini CLI, OpenCode, OpenClaw, Cursor, Aider, Windsurf, Kimi Code, Codex, Osaurus, Hermes, Mistral Vibe)

```bash
# Passo 1 -- gerar arquivos de integração para todas as ferramentas suportadas
./scripts/convert.sh

# Passo 2 -- instalar interativamente (detecta automaticamente o que você tem instalado)
./scripts/install.sh

# Ou direcione para uma ferramenta específica diretamente
./scripts/install.sh --tool antigravity
./scripts/install.sh --tool gemini-cli
./scripts/install.sh --tool opencode
./scripts/install.sh --tool copilot
./scripts/install.sh --tool openclaw
./scripts/install.sh --tool cursor
./scripts/install.sh --tool aider
./scripts/install.sh --tool windsurf
./scripts/install.sh --tool kimi
./scripts/install.sh --tool codex
./scripts/install.sh --tool osaurus
./scripts/install.sh --tool hermes
./scripts/install.sh --tool vibe
```

**Instale apenas os times necessários** (nem todo mundo precisa de todas as divisões):

```bash
./scripts/install.sh                                    # assistente interativo: escolha ferramentas + times
./scripts/install.sh --tool claude-code --division engineering,security
./scripts/install.sh --tool cursor --agent frontend-developer,ui-designer
./scripts/install.sh --list teams                       # ver todos os times + contagem de agentes
./scripts/install.sh --tool opencode --division engineering --dry-run
```

> **Nota para OpenCode:** O runtime do OpenCode atualmente registra apenas ~119 agentes e descarta silenciosamente o restante ([bug upstream](https://github.com/anomalyco/opencode/issues/27988)). Instalar um subconjunto com `--division` mantém você abaixo desse limite. O instalador avisará caso a seleção ultrapasse o valor.

Veja a seção [Integrações Multi-Ferramenta](#-integrações-multi-ferramenta) abaixo para mais detalhes.

---

## 🎨 O Catálogo de Agentes

### 💻 Divisão de Engenharia

Construindo o futuro, um commit por vez.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎨 [Frontend Developer](engineering/engineering-frontend-developer.md) | React/Vue/Angular, implementação de UI, performance | Aplicações web modernas, interfaces pixel-perfect, otimização de Core Web Vitals |
| 🏗️ [Backend Architect](engineering/engineering-backend-architect.md) | Design de APIs, arquitetura de banco de dados, escalabilidade | Sistemas server-side, microsserviços, infraestrutura em nuvem |
| 📱 [Mobile App Builder](engineering/engineering-mobile-app-builder.md) | iOS/Android, React Native, Flutter | Aplicativos móveis nativos e multiplataforma |
| 🤖 [AI Engineer](engineering/engineering-ai-engineer.md) | Modelos de ML, deploy, integração de IA | Recursos de machine learning, pipelines de dados, apps potencializados por IA |
| 🚀 [DevOps Automator](engineering/engineering-devops-automator.md) | CI/CD, automação de infraestrutura, cloud ops | Desenvolvimento de pipelines, automação de deploy, monitoramento |
| 🌐 [Network Engineer](engineering/engineering-network-engineer.md) | Cisco IOS/IOS-XE, Juniper Junos, Palo Alto PAN-OS | Configuração de roteadores/switches/firewalls, BGP/OSPF, ACLs, troubleshooting de saídas de comandos |
| ⚡ [Rapid Prototyper](engineering/engineering-rapid-prototyper.md) | Desenvolvimento rápido de POCs, MVPs | Provas de conceito ágeis, projetos de hackathon, iteração rápida |
| 💎 [Senior Developer](engineering/engineering-senior-developer.md) | Laravel/Livewire, padrões avançados | Implementações complexas, decisões de arquitetura |
| 🔧 [Filament Optimization Specialist](engineering/engineering-filament-optimization-specialist.md) | UX do admin Filament PHP, redesign estrutural de formulários, otimização de recursos | Reestruturação de recursos/formulários/tabelas do Filament para fluxos de admin mais rápidos e limpos |
| ⚡ [Autonomous Optimization Architect](engineering/engineering-autonomous-optimization-architect.md) | Roteamento de LLMs, otimização de custos, testes sombra (shadow testing) | Sistemas autônomos que exigem seleção inteligente de APIs e controle de custos |
| 🔩 [Embedded Firmware Engineer](engineering/engineering-embedded-firmware-engineer.md) | Bare-metal, RTOS, firmware para ESP32/STM32/Nordic | Sistemas embarcados de nível de produção e dispositivos IoT |
| 🚨 [Incident Response Commander](engineering/engineering-incident-response-commander.md) | Gestão de incidentes, post-mortems, plantão (on-call) | Gerenciamento de incidentes em produção e criação de prontidão operacional |
| ⛓️ [Solidity Smart Contract Engineer](engineering/engineering-solidity-smart-contract-engineer.md) | Contratos EVM, otimização de gas, DeFi | Smart contracts seguros e otimizados para gas e protocolos DeFi |
| 🧭 [Codebase Onboarding Engineer](engineering/engineering-codebase-onboarding-engineer.md) | Onboarding rápido de desenvolvedores, exploração somente-leitura de repositórios, explicação factual | Ajudar novos desenvolvedores a entender repositórios desconhecidos rapidamente lendo o código, rastreando caminhos e explicando fatos sobre estrutura e comportamento |
| 📚 [Technical Writer](engineering/engineering-technical-writer.md) | Documentação para devs, referências de API, tutoriais | Documentação técnica clara e precisa |
| 💬 [WeChat Mini Program Developer](engineering/engineering-wechat-mini-program-developer.md) | Ecossistema WeChat, Mini Programs, integração de pagamentos | Criação de aplicativos performáticos para o ecossistema WeChat |
| 👁️ [Code Reviewer](engineering/engineering-code-reviewer.md) | Revisão construtiva de código, segurança, manutenibilidade | Revisões de PR, portões de qualidade de código, mentoria através de reviews |
| 🗄️ [Database Optimizer](engineering/engineering-database-optimizer.md) | Design de schema, otimização de queries, estratégias de indexação | Ajuste de PostgreSQL/MySQL, depuração de queries lentas, planejamento de migração |
| 🌿 [Git Workflow Master](engineering/engineering-git-workflow-master.md) | Estratégias de ramificação (branching), conventional commits, Git avançado | Design de fluxos Git, limpeza de histórico, gestão de branches amigável ao CI |
| 🏛️ [Software Architect](engineering/engineering-software-architect.md) | Design de sistemas, DDD, padrões arquiteturais, análise de trade-offs | Decisões arquiteturais, modelagem de domínio, estratégia de evolução de sistemas |
| 🛡️ [SRE](engineering/engineering-sre.md) | SLOs, orçamentos de erro (error budgets), observabilidade, engenharia de caos | Confiabilidade de produção, redução de trabalho repetitivo (toil), planejamento de capacidade |
| 🧬 [AI Data Remediation Engineer](engineering/engineering-ai-data-remediation-engineer.md) | Pipelines auto-regenerativos, SLMs air-gapped, clustering semântico | Correção de dados corrompidos em escala com zero perda de dados |
| 🔧 [Data Engineer](engineering/engineering-data-engineer.md) | Pipelines de dados, arquitetura lakehouse, ETL/ELT | Construção de infraestrutura de dados confiável e data warehousing |
| 🔗 [Feishu Integration Developer](engineering/engineering-feishu-integration-developer.md) | Plataforma aberta Feishu/Lark, bots, fluxos de trabalho | Construção de integrações para o ecossistema Feishu |
| 🧱 [CMS Developer](engineering/engineering-cms-developer.md) | Temas WordPress e Drupal, plugins/módulos, arquitetura de conteúdo | Implementação e customização de CMS code-first |
| 📧 [Email Intelligence Engineer](engineering/engineering-email-intelligence-engineer.md) | Parsing de e-mails, extração MIME, dados estruturados para agentes de IA | Transformação de threads de e-mail brutas em contexto pronto para raciocínio |
| 🎙️ [Voice AI Integration Engineer](engineering/engineering-voice-ai-integration-engineer.md) | Pipelines speech-to-text, Whisper, ASR, diarização de locutores | Pipelines de transcrição ponta a ponta, pré-processamento de áudio, entrega de transcrições estruturadas |
| 🖧 [IT Service Manager](engineering/engineering-it-service-manager.md) | Gerenciamento de serviços ITIL 4 | Gerenciamento de incidentes/problemas/mudanças, SLAs, CMDB |
| 🪡 [Minimal Change Engineer](engineering/engineering-minimal-change-engineer.md) | Diffs mínimos viáveis | Corrigir estritamente o que foi solicitado, sem escopo inflado |
| 📜 [OrgScript Engineer](engineering/engineering-orgscript-engineer.md) | Gramática OrgScript e validação de AST | Criação e parsing de definições de lógica de negócios em OrgScript |
| 🧬 [Prompt Engineer](engineering/engineering-prompt-engineer.md) | Design e otimização de prompts para LLM | Transformação de instruções vagas em comportamentos confiáveis de IA |
| 🕸️ [Multi-Agent Systems Architect](engineering/engineering-multi-agent-systems-architect.md) | Design e governança de pipelines multi-agente | Topologia, contexto, confiança e recuperação de falhas para sistemas de agentes |
| 🛒 [Drupal Shopping Cart Engineer](engineering/engineering-drupal-shopping-cart.md) | Lojas virtuais Drupal Commerce | Catálogo, pagamentos, checkout e pedidos no Drupal 10/11 |
| 🛍️ [WordPress Shopping Cart Engineer](engineering/engineering-wordpress-shopping-cart.md) | Lojas virtuais WooCommerce | Catálogo, pagamentos, checkout e conversão no WordPress |
| 💳 [Payments & Billing Engineer](engineering/engineering-payments-billing-engineer.md) | Integração de PSPs, fluxos de pagamento idempotentes, cobrança recorrente | Integrações com Stripe/Adyen/Braintree, processamento de webhooks, régua de cobrança (dunning), conciliação |
| 🌍 [Internationalization Engineer](engineering/engineering-i18n-engineer.md) | ICU MessageFormat, layouts RTL/bidirecionais, formatação CLDR, pseudo-localização | Preparação de apps para tradução, formatação sensível a localidade, suporte a RTL, auditorias de i18n |
| ⚡ [Drupal Performance Engineer](engineering/engineering-drupal-performance.md) | Performance no Drupal e Core Web Vitals | Caching, otimização de DB/queries, pipeline de renderização, profiling em sites Drupal de alto tráfego |
| ⚡ [WordPress Performance Engineer](engineering/engineering-wordpress-performance.md) | Performance no WordPress e Core Web Vitals | Caching, otimização de queries/assets, ajuste fino de plugins, profiling em sites WP de alto tráfego |
| ♿ [Section 508 Accessibility Specialist](engineering/engineering-section-508-specialist.md) | Acessibilidade federal dos EUA (Section 508 / WCAG) | ARIA, testes com leitores de tela, criação de VPAT/ACR, remediação de acessibilidade |
| 🏛️ [USWDS Developer](engineering/engineering-uswds-developer.md) | Sistema de Design Web dos EUA (USWDS) | Componentes de interface acessíveis para governos e padrões de design system |
| 🔎 [Search Relevance Engineer](engineering/engineering-search-relevance-engineer.md) | Ranqueamento e relevância de busca | Compreensão de consultas, embeddings, ranking/avaliação, ajuste fino de relevância |
| 🔐 [Identity & Access Engineer](engineering/engineering-identity-access-engineer.md) | AuthN/AuthZ e IAM | OAuth/OIDC/SAML, SSO, RBAC/ABAC, segurança de tokens e sessões |
| 🤝 [Realtime Collaboration Engineer](engineering/engineering-realtime-collaboration-engineer.md) | Sincronização e presença em tempo real | CRDTs/OT, resolução de conflitos, cursores ao vivo, sincronização offline |
| 💻 [Desktop App Engineer](engineering/engineering-desktop-app-engineer.md) | Aplicativos desktop multiplataforma | Electron/Tauri, integração nativa, empacotamento, atualização automática |
| 🚀 [Mobile Release Engineer](engineering/engineering-mobile-release-engineer.md) | Release mobile e CI/CD | Submissão na App Store/Play Store, assinatura digital, rollout em etapas, triagem de falhas (crashes) |
| 🎬 [Video Streaming Engineer](engineering/engineering-video-streaming-engineer.md) | Streaming de vídeo e transcodificação | HLS/DASH, ABR, codecs, entrega via CDN, streaming de baixa latência |
| 💰 [FinOps Engineer](engineering/engineering-finops-engineer.md) | Engenharia de custos em nuvem | Alocação de custos, rightsizing, unit economics, controle de orçamento e anomalias |
| 🧩 [WebAssembly Engineer](engineering/engineering-webassembly-engineer.md) | WebAssembly e WASI | Rust/C++ para WASM, sandboxing, bindings com o host, performance |
| 🔌 [API Platform Engineer](engineering/engineering-api-platform-engineer.md) | Gateways e plataformas de API | Design de gateways, versionamento, rate limiting, portais para desenvolvedores |
| 🛟 [Database Reliability Engineer](engineering/engineering-database-reliability-engineer.md) | Confiabilidade de banco de dados (DBRE) | Alta disponibilidade/replicação, failover automatizado, backups PITR, operações com downtime zero |
| 🛠️ [Developer Tooling Engineer](engineering/engineering-developer-tooling-engineer.md) | CLI e ferramentas para desenvolvedores | Ferramentas de linha de comando, DX interna, fluxos de build e desenvolvimento |
| 📡 [IoT Fleet Engineer](engineering/engineering-iot-fleet-engineer.md) | Frotas IoT e edge computing | Provisionamento/identidade de dispositivos, telemetria MQTT, atualizações OTA |
| 🔍 [RAG Pipeline Engineer](engineering/engineering-rag-pipeline-engineer.md) | Pipelines RAG de produção | Chunking, qualidade de recuperação, busca híbrida, re-ranking, iteração orientada a avaliação |
| 🗄️ [GaussDB Expert Engineer](engineering/engineering-gaussdb-expert.md) | Huawei GaussDB OLTP | Performance empresarial OLTP, alta disponibilidade e migração no Huawei GaussDB |
| 🕵️ [Privacy Engineer](engineering/engineering-privacy-engineer.md) | Descoberta de PII, minimização de dados, consentimento, pipelines de DSAR/deleção | Implementação de privacidade em código, direito ao esquecimento entre serviços, automação de retenção |
| 🦀 [Rust Refactoring Specialist](engineering/engineering-rust-refactoring-specialist.md) | Refatoração de Rust com preservação de comportamento | Reestruturação de crates/traits/módulos com alterações baseadas em evidências que preservam o comportamento |
| 🧪 [LLM Post-Training Engineer](engineering/engineering-llm-post-training-engineer.md) | Stack de pós-treinamento (SFT/DPO/GRPO/RLVR) | Validação de experimentos por evidências, integridade de checkpoints, classificação de falhas |
| 📈 [Data Visualization Engineer](engineering/engineering-data-visualization-engineer.md) | Visualização de dados perceptual e honesta | Seleção de tipos de gráfico, paletas acessíveis para daltônicos, renderização performática em D3/Vega |
| 🧠 [Knowledge Graph Engineer](engineering/engineering-knowledge-graph-engineer.md) | Grafos de conhecimento, extração entidade-relacionamento, Graph RAG | Estruturação de documentos em grafos Neo4j consultáveis com LangGraph; proveniência, rastreamento de contradições, recuperação de subgrafos |

### 🎨 Divisão de Design

Tornando tudo bonito, utilizável e encantador.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎯 [UI Designer](design/design-ui-designer.md) | Design visual, bibliotecas de componentes, design systems | Criação de interfaces, consistência de marca, design de componentes |
| 🔍 [UX Researcher](design/design-ux-researcher.md) | Testes com usuários, análise de comportamento, pesquisa | Compreensão dos usuários, testes de usabilidade, insights de design |
| 🏛️ [UX Architect](design/design-ux-architect.md) | Arquitetura técnica, sistemas CSS, implementação | Fundações amigáveis aos desenvolvedores, orientações de implementação |
| 🎭 [Brand Guardian](design/design-brand-guardian.md) | Identidade de marca, consistência, posicionamento | Estratégia de marca, desenvolvimento de identidade, manuais de marca |
| 📖 [Visual Storyteller](design/design-visual-storyteller.md) | Narrativas visuais, conteúdo multimídia | Histórias visuais envolventes, storytelling de marca |
| ✨ [Whimsy Injector](design/design-whimsy-injector.md) | Personalidade, encantamento, interações divertidas | Adicionar alegria, microinterações, easter eggs e personalidade à marca |
| 📷 [Image Prompt Engineer](design/design-image-prompt-engineer.md) | Prompts para geração de imagem por IA, fotografia | Prompts fotográficos para Midjourney, DALL-E, Stable Diffusion |
| 🌈 [Inclusive Visuals Specialist](design/design-inclusive-visuals-specialist.md) | Representatividade, mitigação de vieses, imagens autênticas | Geração de imagens e vídeos por IA culturalmente precisos |
| 🎭 [Persona Walkthrough Specialist](design/design-persona-walkthrough.md) | Walkthroughs cognitivos orientados por personas | Simulação de reações e atritos dos usuários a cada rolagem de página |
| 🧱 [UI Finish-Gate Reviewer](design/design-ui-finish-gate-reviewer.md) | Portão de revisão contra interfaces genéricas | Evitar UIs genéricas antes do lançamento usando evidências e um contrato de design por escrito |

### 💰 Divisão de Mídia Paga

Transformando investimento em anúncios em resultados comerciais mensuráveis.

| Agente | Especialidade | Quando Usar |
| --- | --- | --- |
| 💰 [PPC Campaign Strategist](paid-media/paid-media-ppc-strategist.md) | Google/Microsoft/Amazon Ads, arquitetura de contas, lances (bidding) | Estruturação de contas, alocação de orçamento, escala, diagnóstico de desempenho |
| 🔍 [Search Query Analyst](paid-media/paid-media-search-query-analyst.md) | Análise de termos de busca, palavras-chave negativas, mapeamento de intenção | Auditorias de consultas, eliminação de verba desperdiçada, descoberta de palavras-chave |
| 📋 [Paid Media Auditor](paid-media/paid-media-auditor.md) | Auditoria de contas com mais de 200 itens, análise competitiva | Assunção de novas contas, revisões trimestrais, apresentações comerciais (pitches) |
| 📡 [Tracking & Measurement Specialist](paid-media/paid-media-tracking-specialist.md) | GTM, GA4, rastreamento de conversão, CAPI | Novas implementações, auditorias de rastreamento, migrações de plataforma |
| ✍️ [Ad Creative Strategist](paid-media/paid-media-creative-strategist.md) | Textos para anúncios responsivos (RSA), criativos Meta, assets Performance Max | Lançamento de criativos, programas de testes, renovação de anúncios saturados |
| 📺 [Programmatic & Display Buyer](paid-media/paid-media-programmatic-buyer.md) | GDN, DSPs, mídia parceira, display para ABM | Planejamento de display, prospecção de parceiros, programas de ABM |
| 📱 [Paid Social Strategist](paid-media/paid-media-paid-social-strategist.md) | Meta, LinkedIn, TikTok, social multiplataforma | Programas de anúncios sociais, seleção de plataformas, estratégia de audiência |

### 💼 Divisão de Vendas

Transformando pipeline em receita através de técnica, e não de trabalho burocrático no CRM.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎯 [Outbound Strategist](sales/sales-outbound-strategist.md) | Prospecção baseada em sinais, cadências multicanal, segmentação por ICP | Criação de pipeline por meio de prospecção orientada por pesquisa, não por volume |
| 🔍 [Discovery Coach](sales/sales-discovery-coach.md) | SPIN, Gap Selling, Sandler — estruturação de ligações e elaboração de perguntas | Preparação para chamadas de descoberta, qualificação de oportunidades, coaching de vendedores |
| ♟️ [Deal Strategist](sales/sales-deal-strategist.md) | Qualificação MEDDPICC, posicionamento competitivo, planos de vitória | Pontuação de oportunidades, exposição de riscos no pipeline, montagem de planos para fechar negócios |
| 🛠️ [Sales Engineer](sales/sales-engineer.md) | Demonstrações técnicas, escopo de POCs, battlecards competitivos | Fechamentos técnicos pré-venda, preparação de demonstrações, posicionamento contra concorrentes |
| 🏹 [Proposal Strategist](sales/sales-proposal-strategist.md) | Respostas a RFPs, propostas de valor vencedoras, estrutura narrativa | Redação de propostas que convencem, em vez de apenas cumprir requisitos |
| 📊 [Pipeline Analyst](sales/sales-pipeline-analyst.md) | Previsão (forecasting), integridade do pipeline, velocidade de negócios, RevOps | Revisão de pipeline, precisão de projeções, operações de receita |
| 🗺️ [Account Strategist](sales/sales-account-strategist.md) | Land-and-expand, QBRs, mapeamento de partes interessadas (stakeholders) | Expansão pós-venda, planejamento de contas-chave, crescimento de NRR |
| 🏋️ [Sales Coach](sales/sales-coach.md) | Desenvolvimento de representantes, coaching em ligações, facilitação de revisões de pipeline | Melhoria contínua de representantes e negociações por meio de coaching estruturado |
| 🎯 [Sales Outreach](specialized/sales-outreach.md) | Prospecção fria, cadências multitoque, tratamento de objeções, propostas | Prospecção B2B de topo de funil — do cold mail à primeira chamada de diagnóstico agendada |
| 🧲 [Offer & Lead Gen Strategist](sales/sales-offer-lead-gen-strategist.md) | Ofertas e iscas digitais (lead magnets) | Construção de ofertas de topo de funil e geração de leads |

### 📢 Divisão de Marketing

Crescendo seu público, uma interação autêntica de cada vez.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🚀 [Growth Hacker](marketing/marketing-growth-hacker.md) | Aquisição rápida de usuários, loops virais, experimentos | Crescimento explosivo, aquisição de usuários, otimização de conversão |
| 📝 [Content Creator](marketing/marketing-content-creator.md) | Conteúdo multiplataforma, calendários editoriais | Estratégia de conteúdo, copywriting, storytelling de marca |
| 🐦 [Twitter Engager](marketing/marketing-twitter-engager.md) | Engajamento em tempo real, liderança de pensamento | Estratégia no Twitter/X, campanhas no LinkedIn, presença social profissional |
| 🛰️ [X/Twitter Intelligence Analyst](marketing/marketing-x-twitter-intelligence-analyst.md) | Escuta social (social listening), detecção de tendências, monitoramento de contas | Risco de marca, concorrência e inteligência de audiência no X/Twitter |
| 📱 [TikTok Strategist](marketing/marketing-tiktok-strategist.md) | Conteúdo viral, otimização para algoritmos | Crescimento no TikTok, conteúdo viral, alcance de públicos Gen Z/Millennials |
| 📸 [Instagram Curator](marketing/marketing-instagram-curator.md) | Storytelling visual, construção de comunidade | Estratégia de Instagram, desenvolvimento estético, conteúdo visual |
| 🤝 [Reddit Community Builder](marketing/marketing-reddit-community-builder.md) | Engajamento autêntico, conteúdo focado em valor | Estratégia no Reddit, geração de confiança na comunidade, marketing não-invasivo |
| 📱 [App Store Optimizer](marketing/marketing-app-store-optimizer.md) | ASO, otimização de conversão, descoberta | Marketing para apps, otimização em lojas de aplicativos, crescimento mobile |
| 🌐 [Social Media Strategist](marketing/marketing-social-media-strategist.md) | Estratégia multicanal, campanhas | Estratégia social global, campanhas em múltiplas plataformas |
| 📕 [Xiaohongshu Specialist](marketing/marketing-xiaohongshu-specialist.md) | Conteúdo de lifestyle, estratégia baseada em tendências | Crescimento no Xiaohongshu (RED), narrativas estéticas, público Gen Z |
| 💬 [WeChat Official Account Manager](marketing/marketing-wechat-official-account.md) | Engajamento de inscritos, marketing de conteúdo | Estratégia de contas oficiais no WeChat, comunidades, conversão |
| 🧠 [Zhihu Strategist](marketing/marketing-zhihu-strategist.md) | Liderança de pensamento, engajamento baseado em conhecimento | Construção de autoridade no Zhihu, estratégia de P&R, captação de leads |
| 🇨🇳 [Baidu SEO Specialist](marketing/marketing-baidu-seo-specialist.md) | Otimização para o Baidu, SEO China, conformidade com ICP | Posicionamento nas buscas do Baidu e alcance do mercado de busca chinês |
| 🎬 [Bilibili Content Strategist](marketing/marketing-bilibili-content-strategist.md) | Algoritmo do Bilibili, cultura danmaku, crescimento de criadores (UP主) | Construção de audiência no Bilibili com foco comunitário |
| 🎠 [Carousel Growth Engine](marketing/marketing-carousel-growth-engine.md) | Carrosséis para TikTok/Instagram, publicação autônoma | Criação e publicação de carrosséis com potencial viral |
| 💼 [LinkedIn Content Creator](marketing/marketing-linkedin-content-creator.md) | Marca pessoal, liderança de pensamento, conteúdo profissional | Crescimento no LinkedIn, audiência corporativa, conteúdo B2B |
| 🛒 [China E-Commerce Operator](marketing/marketing-china-ecommerce-operator.md) | Taobao, Tmall, Pinduoduo, live commerce | Operação de e-commerce multiplataforma na China |
| 🎥 [Kuaishou Strategist](marketing/marketing-kuaishou-strategist.md) | Kuaishou, comunidade 老铁, crescimento orgânico de base | Construção de audiências autênticas em mercados e cidades menores |
| 🔍 [SEO Specialist](marketing/marketing-seo-specialist.md) | SEO técnico, estratégia de conteúdo, link building | Impulsionamento de crescimento orgânico sustentável nas buscas |
| 📘 [Book Co-Author](marketing/marketing-book-co-author.md) | Livros de liderança intelectual, ghostwriting, publicação | Coautoria estratégica de livros para fundadores e especialistas |
| 🌏 [Cross-Border E-Commerce Specialist](marketing/marketing-cross-border-ecommerce.md) | Amazon, Shopee, Lazada, logística cross-border | Estratégia de e-commerce internacional de ponta a ponta |
| 🎵 [Douyin Strategist](marketing/marketing-douyin-strategist.md) | Plataforma Douyin, marketing de vídeos curtos, algoritmo | Crescimento de audiência na principal plataforma de vídeos curtos da China |
| 🎙️ [Livestream Commerce Coach](marketing/marketing-livestream-commerce-coach.md) | Treinamento de apresentadores, otimização de salas ao vivo, conversão | Operações de live commerce de alta performance |
| 🎧 [Podcast Strategist](marketing/marketing-podcast-strategist.md) | Estratégia de conteúdo para podcasts, otimização de plataformas | Operações e estratégias voltadas ao mercado chinês de podcasts |
| 🔒 [Private Domain Operator](marketing/marketing-private-domain-operator.md) | WeCom, tráfego privado, gestão de comunidades | Ecossistemas de tráfego e domínio privado no WeChat corporativo |
| 🎬 [Short-Video Editing Coach](marketing/marketing-short-video-editing-coach.md) | Pós-produção, fluxos de edição, especificações por plataforma | Treinamento prático de edição de vídeos curtos e otimização |
| 🔥 [Weibo Strategist](marketing/marketing-weibo-strategist.md) | Sina Weibo, tópicos em alta (trending topics), engajamento de fãs | Operações completas e crescimento no Weibo |
| 🎙️ [Global Podcast Strategist](marketing/marketing-global-podcast-strategist.md) | Posicionamento de programas, crescimento de audiência, monetização | Lançamento de podcasts, algoritmos de plataformas, patrocínios, comunidade |
| 🔮 [AI Citation Strategist](marketing/marketing-ai-citation-strategist.md) | AEO/GEO, visibilidade em recomendações de IA, auditoria de citações | Aumento da visibilidade da marca no ChatGPT, Claude, Gemini e Perplexity |
| 🇨🇳 [China Market Localization Strategist](marketing/marketing-china-market-localization-strategist.md) | Localização completa de mercado chinês, GTM via Douyin/Xiaohongshu/WeChat | Transformação de sinais de tendências em estratégias de go-to-market na China |
| 🎬 [Video Optimization Specialist](marketing/marketing-video-optimization-specialist.md) | Estratégia para o algoritmo do YouTube, capítulos, ideias de miniaturas (thumbnails) | Crescimento de canais no YouTube, SEO de vídeo, retenção de público |
| 🏗️ [AEO Foundations Architect](marketing/marketing-aeo-foundations.md) | Infraestrutura de Otimização para Motores de IA (AEO) | llms.txt, robots.txt amigável a IA, arquivos de descoberta para agentes |
| 🤖 [Agentic Search Optimizer](marketing/marketing-agentic-search-optimizer.md) | WebMCP e conclusão de tarefas por agentes | Tornar sites utilizáveis por agentes de IA com navegação autônoma |
| 📧 [Email Marketing Strategist](marketing/marketing-email-strategist.md) | Ciclo de vida por e-mail e entregabilidade | Campanhas de CRM, automação, segmentação |
| 📡 [Multi-Platform Publisher](marketing/marketing-multi-platform-publisher.md) | Publicação em um clique em múltiplas plataformas chinesas | Distribuição simultânea de artigos para Zhihu/Xiaohongshu/CSDN/Bilibili/WeChat/Juejin |
| 📣 [PR & Communications Manager](marketing/marketing-pr-communications-manager.md) | Relações públicas, assessoria de imprensa e comunicação de crise | Comunicados de imprensa, liderança de pensamento, reputação |

### 📊 Divisão de Produto

Construindo a coisa certa no momento certo.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎯 [Sprint Prioritizer](product/product-sprint-prioritizer.md) | Planejamento ágil, priorização de recursos | Planejamento de sprints, alocação de recursos, gerenciamento de backlog |
| 🔍 [Trend Researcher](product/product-trend-researcher.md) | Inteligência de mercado, análise competitiva | Pesquisa de mercado, avaliação de oportunidades, identificação de tendências |
| 💬 [Feedback Synthesizer](product/product-feedback-synthesizer.md) | Análise de feedback de usuários, extração de insights | Análise de opiniões, insights de usuários, definição de prioridades de produto |
| 🧠 [Behavioral Nudge Engine](product/product-behavioral-nudge-engine.md) | Psicologia comportamental, design de nudges, engajamento | Maximização da motivação do usuário através de ciência comportamental |
| 🧭 [Product Manager](product/product-manager.md) | Gestão de ciclo de vida completo de produto | Descoberta, PRDs, planejamento de roadmap, GTM, mensuração de resultados |

### 🎬 Divisão de Gestão de Projetos

Mantendo os prazos em dia (e dentro do orçamento).

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎬 [Studio Producer](project-management/project-management-studio-producer.md) | Orquestração de alto nível, gestão de portfólio | Supervisão multiprojeto, alinhamento estratégico, alocação de recursos |
| 🐑 [Project Shepherd](project-management/project-management-project-shepherd.md) | Coordenação multifuncional, gerenciamento de cronogramas | Coordenação de ponta a ponta, relacionamento com stakeholders |
| ⚙️ [Studio Operations](project-management/project-management-studio-operations.md) | Eficiência do dia a dia, otimização de processos | Excelência operacional, suporte ao time, aumento de produtividade |
| 🧪 [Experiment Tracker](project-management/project-management-experiment-tracker.md) | Testes A/B, validação de hipóteses | Gestão de experimentos, decisões orientadas a dados, testes |
| 👔 [Senior Project Manager](project-management/project-manager-senior.md) | Escopo realista, quebra de tarefas | Conversão de especificações em tarefas, controle de escopo |
| 📋 [Jira Workflow Steward](project-management/project-management-jira-workflow-steward.md) | Fluxo Git, estratégia de branches, rastreabilidade | Aplicação de disciplina Git associada ao Jira e entregas |
| 📋 [Meeting Notes Specialist](project-management/project-management-meeting-notes-specialist.md) | Resumos estruturados de reuniões | Extração de decisões, planos de ação (action items) e perguntas abertas |

### 🧪 Divisão de Testes (QA)

Quebrando as coisas para que os usuários não precisem passar por isso.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 📸 [Evidence Collector](testing/testing-evidence-collector.md) | QA baseado em capturas de tela, prova visual | Testes de interface, verificação visual, documentação de bugs |
| 🔍 [Reality Checker](testing/testing-reality-checker.md) | Certificação baseada em evidências, portões de qualidade | Prontidão para produção, aprovação de qualidade, certificação de lançamentos |
| 📊 [Test Results Analyzer](testing/testing-test-results-analyzer.md) | Avaliação de testes, análise de métricas | Análise de resultados de testes, insights de qualidade, relatórios de cobertura |
| ⚡ [Performance Benchmarker](testing/testing-performance-benchmarker.md) | Testes de performance, otimização | Testes de velocidade, testes de carga (load testing), ajuste de performance |
| 🔌 [API Tester](testing/testing-api-tester.md) | Validação de APIs, testes de integração | Testes de API, verificação de endpoints, QA de integração |
| 🛠️ [Tool Evaluator](testing/testing-tool-evaluator.md) | Avaliação tecnológica, seleção de ferramentas | Escolha de ferramentas, recomendações de software, decisões de stack |
| 🔄 [Workflow Optimizer](testing/testing-workflow-optimizer.md) | Análise de processos, melhoria de fluxos de trabalho | Otimização de processos, ganhos de eficiência, oportunidades de automação |
| ♿ [Accessibility Auditor](testing/testing-accessibility-auditor.md) | Auditoria WCAG, testes com tecnologias assistivas | Conformidade de acessibilidade, leitores de tela, validação de design inclusivo |
| 🎭 [Test Automation Engineer](testing/testing-test-automation-engineer.md) | E2E com Playwright/Cypress, eliminação de instabilidade (flakiness), paralelização em CI | Suítes de testes de navegador, pipelines determinísticos, depuração por rastros (traces) |

### 🔒 Divisão de Segurança

Defendendo toda a stack — desde a arquitetura segura por design até a resposta a incidentes.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🛡️ [Security Architect](security/security-architect.md) | Modelagem de ameaças, secure-by-design, limites de confiança | Modelos de segurança de sistemas, revisões de arquitetura, defesa em profundidade |
| 🔐 [Application Security Engineer](security/security-appsec-engineer.md) | Segurança no SDLC, SAST/DAST, revisão segura de código | Proteção do ciclo de desenvolvimento, vulnerabilidades a nível de código |
| 🗡️ [Penetration Tester](security/security-penetration-tester.md) | Pentests autorizados, operações de red team, exploração | Localizar brechas exploráveis antes que invasores as encontrem |
| ☁️ [Cloud Security Architect](security/security-cloud-security-architect.md) | Zero trust, defesa em profundidade nativa em nuvem | Proteção de infraestrutura e arquiteturas em nuvem |
| 🚨 [Incident Responder](security/security-incident-responder.md) | DFIR, investigação de vazamentos, contenção de ameaças | Resposta a invasões ativas, perícia forense, contenção de crises |
| 🔍 [Threat Intelligence Analyst](security/security-threat-intelligence-analyst.md) | Rastreamento de adversários, mapeamento de campanhas, ATT&CK | Identificar quem está atacando e quais técnicas estão sendo utilizadas |
| 🎯 [Threat Detection Engineer](security/security-threat-detection-engineer.md) | Regras SIEM, threat hunting, mapeamento ATT&CK | Criação de camadas de detecção e caça ativa a ameaças |
| 🛡️ [Senior SecOps Engineer](security/security-senior-secops.md) | Varredura de segredos, envios seguros por padrão | Segurança defensiva a nível de código em cada alteração |
| 📋 [Compliance Auditor](security/security-compliance-auditor.md) | SOC 2, ISO 27001, HIPAA, PCI-DSS | Orientação de empresas em auditorias de certificação e conformidade |
| 🛡️ [Blockchain Security Auditor](security/security-blockchain-security-auditor.md) | Auditorias de contratos inteligentes, análise de exploits | Localização de vulnerabilidades em smart contracts antes do deploy |
| 🔎 [AI-Generated Code Security Auditor](security/security-ai-generated-code-auditor.md) | Revisão de segurança de apps gerados por IA ("vibe coding") | Busca por segredos expostos, falhas de RLS, vulnerabilidades a injeção de prompt |
| 🔑 [Secrets & Credential Hygiene Engineer](security/security-secrets-credential-engineer.md) | Ciclo de vida de segredos e credenciais | Detecção, armazenamento em cofre (vault), rotação e resposta a vazamentos |

### 🛟 Divisão de Suporte

A espinha dorsal das operações.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 💬 [Support Responder](support/support-support-responder.md) | Atendimento ao cliente, resolução de chamados | Suporte ao cliente, experiência do usuário, operações de atendimento |
| 📊 [Analytics Reporter](support/support-analytics-reporter.md) | Análise de dados, dashboards, insights | Business intelligence, acompanhamento de KPIs, visualização de métricas |
| 💰 [Finance Tracker](support/support-finance-tracker.md) | Planejamento financeiro, controle orçamentário | Análise financeira, fluxo de caixa, desempenho do negócio |
| 🏗️ [Infrastructure Maintainer](support/support-infrastructure-maintainer.md) | Confiabilidade de sistemas, otimização de performance | Gerenciamento de infraestrutura, operações de sistemas, monitoramento |
| ⚖️ [Legal Compliance Checker](support/support-legal-compliance-checker.md) | Conformidade regulatória, legislações, revisão jurídica | Conformidade legal, requisitos regulatórios, gestão de riscos |
| 📑 [Executive Summary Generator](support/support-executive-summary-generator.md) | Comunicação executiva (C-level), resumos estratégicos | Relatórios executivos, comunicação estratégica, apoio à tomada de decisão |

### 🥽 Divisão de Computação Espacial

Construindo o futuro imersivo.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🏗️ [XR Interface Architect](spatial-computing/xr-interface-architect.md) | Design de interação espacial, UX imersiva | Design de interfaces AR/VR/XR, UX em computação espacial |
| 💻 [macOS Spatial/Metal Engineer](spatial-computing/macos-spatial-metal-engineer.md) | Swift, Metal, 3D de alta performance | Computação espacial no macOS, apps nativos para Vision Pro |
| 🌐 [XR Immersive Developer](spatial-computing/xr-immersive-developer.md) | WebXR, AR/VR baseados em navegador | Experiências imersivas no navegador, aplicações WebXR |
| 🎮 [XR Cockpit Interaction Specialist](spatial-computing/xr-cockpit-interaction-specialist.md) | Controles de cabine/cockpit, sistemas imersivos | Sistemas de controle em cockpit, interfaces de simulação imersiva |
| 🍎 [visionOS Spatial Engineer](spatial-computing/visionos-spatial-engineer.md) | Desenvolvimento para Apple Vision Pro | Aplicativos para Vision Pro, experiências espaciais |
| 🔌 [Terminal Integration Specialist](spatial-computing/terminal-integration-specialist.md) | Integração de terminal, ferramentas de linha de comando | Ferramentas CLI, fluxos de trabalho no terminal, ferramentas para desenvolvedores |

### 🎯 Divisão Especializada

Especialistas únicos que não cabem em caixas tradicionais.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎭 [Agents Orchestrator](specialized/agents-orchestrator.md) | Coordenação multi-agente, gestão de fluxos de trabalho | Projetos complexos que exigem orquestração entre múltiplos agentes |
| 🔍 [LSP/Index Engineer](specialized/lsp-index-engineer.md) | Protocolo LSP, inteligência de código | Sistemas de inteligência de código, implementação de LSP, indexação semântica |
| 📥 [Sales Data Extraction Agent](specialized/sales-data-extraction-agent.md) | Monitoramento de Excel, extração de métricas de vendas | Ingestão de dados comerciais, métricas MTD, YTD e de fim de ano |
| 📈 [Data Consolidation Agent](specialized/data-consolidation-agent.md) | Agregação de dados de vendas, relatórios em painéis | Resumos territoriais, desempenho de representantes, fotos do pipeline |
| 📬 [Report Distribution Agent](specialized/report-distribution-agent.md) | Envio automatizado de relatórios | Distribuição de relatórios por território, envios agendados |
| 🔐 [Agentic Identity & Trust Architect](specialized/agentic-identity-trust.md) | Identidade de agentes, autenticação, verificação de confiança | Sistemas de identidade multi-agente, autorização de agentes, trilhas de auditoria |
| 🔗 [Identity Graph Operator](specialized/identity-graph-operator.md) | Resolução compartilhada de identidade para sistemas multi-agente | Deduplicação de entidades, propostas de mesclagem, consistência entre agentes |
| 💸 [Accounts Payable Agent](specialized/accounts-payable-agent.md) | Processamento de pagamentos, gestão de fornecedores, auditoria | Execução autônoma de contas a pagar em cripto, moedas fiduciárias e stablecoins |
| 🌍 [Cultural Intelligence Strategist](specialized/specialized-cultural-intelligence-strategist.md) | UX global, representatividade, exclusão cultural | Garantir que o software ressoe de forma adequada entre diferentes culturas |
| 🗣️ [Developer Advocate](specialized/specialized-developer-advocate.md) | Construção de comunidade, DX, conteúdo técnico | Ponte entre o produto e a comunidade de desenvolvedores |
| 🔬 [Model QA Specialist](specialized/specialized-model-qa.md) | Auditorias de ML, análise de variáveis, interpretabilidade | QA de ponta a ponta para modelos de machine learning |
| 🗃️ [ZK Steward](specialized/zk-steward.md) | Gestão do conhecimento, Zettelkasten, notas | Construção de bases de conhecimento conectadas e validadas |
| 🔌 [MCP Builder](specialized/specialized-mcp-builder.md) | Servidores Model Context Protocol (MCP), ferramentas para agentes | Criação de servidores MCP para estender capacidades de agentes de IA |
| 📄 [Document Generator](specialized/specialized-document-generator.md) | Geração de PDF, PPTX, DOCX, XLSX via código | Criação de documentos profissionais, relatórios, visualização de dados |
| ⚙️ [Automation Governance Architect](specialized/automation-governance-architect.md) | Governança de automação, n8n, auditoria de fluxos | Avaliação e governança de automações corporativas em escala |
| 📚 [Corporate Training Designer](specialized/corporate-training-designer.md) | Treinamento corporativo, desenvolvimento de currículos | Criação de programas de aprendizagem e capacitação profissional |
| 🌱 [Personal Growth Mentor](specialized/personal-growth-mentor.md) | Clareza de metas, sistemas de hábitos, responsabilidade, estratégia de vida | Desenvolvimento pessoal prático e sem clichês motivacionais |
| 🏛️ [Government Digital Presales Consultant](specialized/government-digital-presales-consultant.md) | Pré-vendas ToG (governo) na China, transformação digital | Propostas e licitações para projetos públicos digitais |
| ⚕️ [Healthcare Marketing Compliance](specialized/healthcare-marketing-compliance.md) | Conformidade de publicidade em saúde na China | Adequação regulatória de marketing médico e de saúde |
| 🎯 [Recruitment Specialist](specialized/recruitment-specialist.md) | Aquisição de talentos, operações de recrutamento | Estratégia de recrutamento, sourcing e processos seletivos |
| 🎓 [Study Abroad Advisor](specialized/study-abroad-advisor.md) | Educação internacional, planejamento de candidaturas | Planejamento de intercâmbio/estudos nos EUA, Reino Unido, Canadá e Austrália |
| 🔗 [Supply Chain Strategist](specialized/supply-chain-strategist.md) | Gestão de cadeia de suprimentos, estratégia de compras | Otimização de suprimentos e planejamento de procurement |
| 🗺️ [Workflow Architect](specialized/specialized-workflow-architect.md) | Descoberta, mapeamento e especificação de fluxos de trabalho | Mapeamento de todos os caminhos do sistema antes do início da codificação |
| ☁️ [Salesforce Architect](specialized/specialized-salesforce-architect.md) | Design multi-cloud em Salesforce, limites de governor, integrações | Arquitetura corporativa em Salesforce, estratégia de instâncias (orgs), pipelines |
| 🇫🇷 [French Consulting Market Navigator](specialized/specialized-french-consulting-market.md) | Ecossistema ESN/SI, portage salarial, precificação | Atuação como consultor freelancer no mercado francês de TI |
| 🇰🇷 [Korean Business Navigator](specialized/specialized-korean-business-navigator.md) | Cultura de negócios coreana, processo 품의, dinâmicas de relacionamento | Navegação em parcerias e relações corporativas no mercado sul-coreano |
| 🏗️ [Civil Engineer](specialized/specialized-civil-engineer.md) | Análise estrutural, projeto geotécnico, normas globais de construção | Engenharia estrutural multi-normas (Eurocode, ACI, AISC e outras) |
| 🎧 [Customer Service](specialized/customer-service.md) | Suporte omnichannel, tratamento de reclamações, retenção, escalonamento | Atendimento ao cliente para qualquer setor: varejo, SaaS, hotelaria, logística |
| 🏥 [Healthcare Customer Service](specialized/healthcare-customer-service.md) | Suporte ao paciente com conformidade HIPAA, faturamento, convênios | Suporte empático e em conformidade regulatória para o setor de saúde |
| 🏨 [Hospitality Guest Services](specialized/hospitality-guest-services.md) | Reservas, concierge, resolução de reclamações, fidelidade | Hotéis, resorts, restaurantes e eventos |
| 🤝 [HR Onboarding](specialized/hr-onboarding.md) | Pré-onboarding, conformidade, benefícios, planos de 30-60-90 dias | Onboarding de novos colaboradores de startups a grandes empresas |
| 🌐 [Language Translator](specialized/language-translator.md) | Tradução Espanhol ↔ Inglês, nuances de dialetos, contexto cultural | Tradução para viagens, negócios, medicina e contextos jurídicos |
| ⏱️ [Legal Billing & Time Tracking](specialized/legal-billing-time-tracking.md) | Registro de horas, descrições de faturamento, compliance IOLTA | Escritórios de advocacia que buscam precisão de faturamento e recuperação de honorários |
| 📋 [Legal Client Intake](specialized/legal-client-intake.md) | Qualificação de clientes em potencial, triagem de conflitos, agendamentos | Captação e conversão de consultas em clientes contratados para escritórios |
| ⚖️ [Legal Document Review](specialized/legal-document-review.md) | Revisão contratual, identificação de riscos, comparação de versões | Primeira análise detalhada de documentos e contratos pronta para advogados |
| 🏦 [Loan Officer Assistant](specialized/loan-officer-assistant.md) | Ingestão de tomadores, conformidade TRID, pipeline, coordenação de fechamento | Equipes de originação de crédito imobiliário e financiamentos |
| 🏠 [Real Estate Buyer & Seller](specialized/real-estate-buyer-seller.md) | Representação de compradores/vendedores, ofertas, coordenação de transações | Negociações e transações no mercado imobiliário residencial e comercial |
| 🛒 [Retail Customer Returns](specialized/retail-customer-returns.md) | Processamento de devoluções, prevenção a fraudes, trocas | Varejo físico, e-commerce e operações omnichannel |
| ♟️ [Business Strategist](specialized/business-strategist.md) | Estratégia estilo consultoria de gestão | Análise competitiva, entrada de mercado, planos de crescimento |
| 🔄 [Change Management Consultant](specialized/change-management-consultant.md) | Gestão de mudanças com frameworks ADKAR/Kotter/Prosci | Condução de organizações em processos de transformação e adoção cultural |
| 🧭 [Chief of Staff](specialized/specialized-chief-of-staff.md) | Coordenação executiva | Filtragem de ruídos, liderança de processos internos, direcionamento de decisões |
| 🌟 [Customer Success Manager](specialized/customer-success-manager.md) | Onboarding, saúde da conta e retenção | QBRs, prevenção de churn, renovações e expansão de receita |
| 📝 [Grant Writer](specialized/grant-writer.md) | Propostas de financiamento e submissão a editais/grants | Cartas de intenção (LOIs), redação de propostas e orçamentos para ONGs e pesquisa |
| 🏥 [Medical Billing & Coding Specialist](specialized/medical-billing-coding-specialist.md) | Faturamento médico, ICD-10/CPT/HCPCS e ciclo de receita | Faturamento, gestão de glosas/recusas e otimização do ciclo de receita em saúde |
| 💰 [Pricing Analyst](specialized/specialized-pricing-analyst.md) | Modelos de precificação e otimização de margem | Análise de custos e concorrência, precificação baseada em valor |
| 💼 [Chief Financial Officer](specialized/chief-financial-officer.md) | Alocação de capital e estratégia financeira | Tesouraria, FP&A, finanças de M&A, relatórios para investidores e conselhos |
| 🌱 [ESG & Sustainability Officer](specialized/esg-sustainability-officer.md) | Programas de ESG e relatórios de sustentabilidade | Estratégia de sustentabilidade, descarbonização, relatórios regulatórios |
| 🔐 [Data Privacy Officer](specialized/data-privacy-officer.md) | Conformidade de privacidade (LGPD/GDPR/CCPA) | Mapeamento de dados, relatórios de impacto (DPIA/RIPD), consentimento, resposta a incidentes |
| ⚙️ [Operations Manager](specialized/operations-manager.md) | Operações com metodologia Lean/Six Sigma | Mapeamento de processos, planejamento de capacidade, governança de KPIs |
| 🤝 [M&A Integration Manager](specialized/ma-integration-manager.md) | Integração pós-fusão/aquisição | Planos para o Dia 1 / 100 dias, acompanhamento de sinergias, acordos de transição (TSA) |
| 🧠 [Organizational Psychologist](specialized/organizational-psychologist.md) | Dinâmica de equipes e saúde cultural | Segurança psicológica, riscos de burnout, desenvolvimento de times de alta performance |
| ⚔️ [Strategy Duel Agent](specialized/specialized-strategy-duel-agent.md) | Teoria dos jogos e Os 36 Estratagemas | Duelos de estratégia por turnos, simulação de cenários adversariais |
| 🛡️ [FedRAMP & RMF Compliance Engineer](specialized/specialized-fedramp-rmf-compliance.md) | Autorização para nuvem governamental dos EUA (ATO) | NIST 800-53, FedRAMP Rev5/20x, SSP/POA&M, ConMon, OSCAL |
| 🏺 [Codebase Archaeologist](specialized/specialized-codebase-archaeologist.md) | Auditorias de desvio estrutural (drift) causadas por múltiplas ferramentas | Detecção de desvios silenciosos no código gerados por edições com Claude/Cursor/Copilot/Windsurf |
| 🧾 [Resume Tailor](specialized/resume-tailor.md) | Otimização de currículos para candidatos | Mapeamento de requisitos de vagas, alinhamento a palavras-chave de ATS, correspondência de experiências |
| 🧡 [Aging Parent Care Companion](specialized/healthcare-aging-parent-care-companion.md) | Suporte à tomada de decisão para cuidadores familiares | Coordenação de consultas/medicamentos, comunicação médica, bem-estar do cuidador |
| 🏛️ [Master Plan Architect](specialized/specialized-master-plan-architect.md) | Ensino arquitetural, crítica red-team de planos | Ensino de arquitetura, crítica de riscos, planos de implementação detalhados em Markdown (sem execução de código) |

### 💵 Divisão Financeira

Especialistas em contabilidade, modelagem financeira, estratégia fiscal e pesquisa de investimentos.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 📒 [Bookkeeper & Controller](finance/finance-bookkeeper-controller.md) | Fechamento mensal, conciliação, GAAP/IFRS, controles internos | Operações contábeis diárias, prontidão para auditoria, organização financeira |
| 📊 [Financial Analyst](finance/finance-financial-analyst.md) | Modelagem financeira, projeções, análise de cenários, suporte a decisões | Modelos de 3 demonstrações, análise de variância, inteligência de negócios |
| 📈 [FP&A Analyst](finance/finance-fpa-analyst.md) | Orçamento, previsões contínuas (rolling forecasts), revisões de negócios | Planos operacionais anuais, revisões mensais, alocação estratégica de recursos |
| 🔍 [Investment Researcher](finance/finance-investment-researcher.md) | Due diligence, análise de portfólio, valuation de ativos, equity research | Criação de teses de investimento, avaliação de riscos, estudos de mercado |
| 🏛️ [Tax Strategist](finance/finance-tax-strategist.md) | Otimização tributária, conformidade multijurisdicional, preços de transferência | Estruturação de entidades, análise de alíquota efetiva (ETR), planejamento tributário estratégico |

### 🎮 Divisão de Desenvolvimento de Jogos

Construindo mundos, sistemas e experiências para as principais engines do mercado.

#### Agentes Multi-Engine (Agnósticos de Engine)

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎯 [Game Designer](game-development/game-designer.md) | Design de sistemas, criação de GDD, balanceamento de economia, gameplay loops | Criação de mecânicas de jogo, sistemas de progressão, elaboração de documentos de design |
| 🗺️ [Level Designer](game-development/level-designer.md) | Teoria de layout, ritmo (pacing), design de encontros, narrativa ambiental | Criação de fases, fluxo de combates/encontros, narrativa através do espaço |
| 🎨 [Technical Artist](game-development/technical-artist.md) | Shaders, VFX, pipeline de LOD, otimização da arte para a engine | Ponte entre arte e programação, criação de shaders, pipelines de assets leves e performáticos |
| 🔊 [Game Audio Engineer](game-development/game-audio-engineer.md) | FMOD/Wwise, música adaptativa, áudio espacial, limites de processamento sonoro | Sistemas de áudio interativo, trilha sonora dinâmica, desempenho acústico |
| 📖 [Narrative Designer](game-development/narrative-designer.md) | Sistemas narrativos, diálogos ramificados, arquitetura de lore | Escrita de narrativas não-lineares, implementação de árvores de diálogo, lore do mundo |
| 💰 [Economy Designer](game-development/economy-designer.md) | Moedas virtuais, geradores/escoadouros (sources/sinks), monetização, controle inflacionário | Design da economia do jogo, equilíbrio de monetização F2P, ajuste de economia em tempo real |

#### Unity

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🏗️ [Unity Architect](game-development/unity/unity-architect.md) | ScriptableObjects, modularidade orientada a dados, DOTS/ECS | Projetos Unity de grande escala, arquitetura baseada em dados, performance via ECS |
| ✨ [Unity Shader Graph Artist](game-development/unity/unity-shader-graph-artist.md) | Shader Graph, HLSL, URP/HDRP, Renderer Features | Materiais personalizados na Unity, shaders para VFX, passes de pós-processamento |
| 🌐 [Unity Multiplayer Engineer](game-development/unity/unity-multiplayer-engineer.md) | Netcode for GameObjects, Unity Relay/Lobby, autoridade de servidor, predição | Jogos multiplayer na Unity, predição de cliente, integração com serviços da Unity Gaming |
| 🛠️ [Unity Editor Tool Developer](game-development/unity/unity-editor-tool-developer.md) | EditorWindows, AssetPostprocessors, PropertyDrawers, validação de builds | Ferramental customizado para a Unity Editor, automação de pipeline, validação de conteúdo |

#### Unreal Engine

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| ⚙️ [Unreal Systems Engineer](game-development/unreal-engine/unreal-systems-engineer.md) | Híbrido C++/Blueprint, GAS, restrições do Nanite, gerenciamento de memória | Sistemas complexos na Unreal, Gameplay Ability System, programação C++ de baixo nível |
| 🎨 [Unreal Technical Artist](game-development/unreal-engine/unreal-technical-artist.md) | Material Editor, Niagara, PCG, Substrate | Materiais na Unreal, efeitos Niagara VFX, geração procedural de conteúdo (PCG) |
| 🌐 [Unreal Multiplayer Architect](game-development/unreal-engine/unreal-multiplayer-architect.md) | Replicação de Actors, hierarquia GameMode/GameState, servidores dedicados | Jogos online na Unreal, gráficos de replicação, arquitetura com autoridade de servidor |
| 🗺️ [Unreal World Builder](game-development/unreal-engine/unreal-world-builder.md) | World Partition, Landscape, HLOD, LWC | Mundos abertos de grande escala, sistemas de streaming, terrenos massivos |

#### Godot

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 📜 [Godot Gameplay Scripter](game-development/godot/godot-gameplay-scripter.md) | GDScript 2.0, signals, composição, tipagem estática | Sistemas de gameplay na Godot, composição de cenas, GDScript performático |
| 🌐 [Godot Multiplayer Engineer](game-development/godot/godot-multiplayer-engineer.md) | MultiplayerAPI, ENet/WebRTC, RPCs, modelo de autoridade | Jogos online na Godot, replicação de cenas, arquitetura com autoridade de servidor |
| ✨ [Godot Shader Developer](game-development/godot/godot-shader-developer.md) | Linguagem de shaders da Godot, VisualShader, RenderingDevice | Materiais customizados na Godot, efeitos 2D/3D, pós-processamento, compute shaders |

#### Blender

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🧩 [Blender Addon Engineer](game-development/blender/blender-addon-engineer.md) | Python para Blender (`bpy`), operadores/painéis customizados, validação de assets, exportadores | Criação de add-ons para Blender, preparação de assets, automação de pipelines DCC |

#### Roblox Studio

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| ⚙️ [Roblox Systems Scripter](game-development/roblox-studio/roblox-systems-scripter.md) | Luau, RemoteEvents/Functions, DataStore, módulos com autoridade de servidor | Sistemas de jogo seguros no Roblox, comunicação cliente-servidor, persistência de dados |
| 🎯 [Roblox Experience Designer](game-development/roblox-studio/roblox-experience-designer.md) | Loops de engajamento, monetização, retenção D1/D7, fluxo de onboarding | Design de ciclos de jogo no Roblox, Game Passes, recompensas diárias, retenção |
| 👗 [Roblox Avatar Creator](game-development/roblox-studio/roblox-avatar-creator.md) | Pipeline UGC, rigging de acessórios, submissão ao Creator Marketplace | Itens UGC no Roblox, personalização de HumanoidDescription, lojas virtuais in-game |

### 📚 Divisão Acadêmica

Rigor científico e acadêmico para construção de mundos, narrativas e histórias.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🌍 [Anthropologist](academic/academic-anthropologist.md) | Sistemas culturais, parentesco, rituais, sistemas de crenças | Criação de sociedades culturalmente coerentes com lógica interna consistente |
| 🌐 [Geographer](academic/academic-geographer.md) | Geografia física e humana, clima, cartografia | Criação de mundos geograficamente realistas com clima, relevo e assentamentos plausíveis |
| 📚 [Historian](academic/academic-historian.md) | Análise histórica, periodização, cultura material | Validação de coerência histórica e enriquecimento de cenários com detalhes autênticos |
| 📜 [Narratologist](academic/academic-narratologist.md) | Teoria narrativa, estrutura de enredo, arcos de personagem | Análise e aprimoramento de estruturas narrativas através de teorias consolidadas |
| 🧠 [Psychologist](academic/academic-psychologist.md) | Teorias de personalidade, motivação, padrões cognitivos | Criação de personagens psicologicamente críveis e fundamentados na ciência |
| 📊 [Statistician](academic/academic-statistician.md) | Inferência estatística e planejamento experimental | Testes de hipóteses, inferência causal, amostragem, análises rigorosas |

---

### 🌍 Divisão de SIG (GIS)

Mapeando a Terra, analisando o espaço construído e extraindo inteligência de dados geoespaciais.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🧠 [Technical Consultant](gis/gis-technical-consultant.md) | Estratégia de SIG, análise de gaps, roadmaps tecnológicos, transformação digital | Mapeamento de necessidades de negócio, escolha da stack geoespacial, planejamento de programas de SIG em várias fases |
| 🔧 [Solution Engineer](gis/gis-solution-engineer.md) | Prototipagem em Esri + FOSS4G, entrega de PoCs, viabilidade técnica | Construção de demonstrações funcionais, validação de viabilidade técnica, apoio pré-venda |
| 🖥️ [GIS Analyst](gis/gis-analyst.md) | Produção cartográfica, controle de qualidade (QC) de dados, simbologia, layouts, consultas espaciais | Operações diárias de SIG, produção de mapas prontos para publicação, integridade de dados |
| 📦 [Spatial Data Engineer](gis/gis-spatial-data-engineer.md) | ETL geoespacial, conversão de formatos, reprojeção de CRS, pipelines automatizados | Ingestão de dados brutos e heterogêneos, criação de pipelines automatizados e repetíveis |
| ⚙️ [Geoprocessing Specialist](gis/gis-geoprocessing-specialist.md) | ArcPy, Python Toolbox (.pyt), Model Builder, automação em lote | Automação de rotinas em SIG, construção de caixas de ferramentas personalizadas |
| ✅ [GIS QA Engineer](gis/gis-qa-engineer.md) | Validação topológica, auditoria de metadados, consistência de CRS, avaliação de acurácia | Portão de qualidade antes de publicar dados, conformidade e integridade geoespacial |
| 🤖 [GeoAI/ML Engineer](gis/gis-geoai-ml-engineer.md) | Extração de feições, detecção de objetos, segmentação semântica, classificação de uso do solo | Extração de edificações/vias/veículos a partir de imagens de satélite, detecção de mudanças e monitoramento ambiental |
| 🏗️ [BIM/GIS Specialist](gis/gis-bim-specialist.md) | Integração Revit/IFC com SIG, mapeamento interno (indoors), gêmeos digitais | Campi inteligentes, gêmeos digitais de aeroportos, navegação interna, gestão predial |
| 🏔️ [3D & Scene Developer](gis/gis-3d-scene-developer.md) | Cesium, ArcGIS Scene Viewer, 3D Tiles, nuvens de pontos, visualização de relevo | Cenas urbanas 3D, sobrevoos de terreno, visualizadores web de nuvens de pontos |
| 📊 [Spatial Data Scientist](gis/gis-spatial-data-scientist.md) | Estatística espacial, clustering, regressão, interpolação, análise de padrões de pontos | Detecção de áreas críticas (hotspots), modelagem espacial, análise preditiva |
| 🛸 [Drone/Reality Mapping](gis/gis-drone-reality-mapping.md) | Fotogrametria, ortomosaicos, MTD/MDS, classificação de nuvens de pontos, malhas 3D | Processamento de imagens de drones, captura de realidade, monitoramento de obras |
| 🌐 [Web GIS Developer](gis/gis-web-gis-developer.md) | MapLibre GL JS, ArcGIS JS API, Leaflet, dashboards em tempo real, APIs REST | Desenvolvimento de mapas web interativos, painéis operacionais, visualização de dados em tempo real |
| 🎨 [Cartography Designer](gis/gis-cartography-designer.md) | Teoria das cores, tipografia, design de basemaps, hierarquia visual, estética para impresso e web | Criação de mapas elegantes e legíveis, paletas com acessibilidade para daltônicos, diagramação profissional |

---

### 🏥 Divisão de Saúde

Desenvolvimento de agentes de IA para contextos clínicos regulados e sistemas públicos de saúde.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🩺 [Clinical Evidence Agent](healthcare/healthcare-clinical-evidence-agent.md) | Padrões de evidência, alegações validadas vs não validadas, limites de autoridade diagnóstica | Elaboração de alegações clínicas críveis sem extrapolar limites diagnósticos regulamentados |
| 🌍 [Sovereign Health Systems Agent](healthcare/healthcare-sovereign-health-systems-agent.md) | Mandatos governamentais de saúde, políticas de cobertura universal, implementação em países emergentes | Equipes de healthtech que operam na intersecção de infraestruturas nacionais de saúde pública |
| 🧭 [Healthcare Innovation Strategist](healthcare/healthcare-innovation-strategist.md) | Narrativas para fundadores de healthtech perante investidores, reguladores e clínicos | Fundadores na área da saúde que precisam traduzir complexidades clínicas e financeiras para atrair capital e confiança |

---

### 🔍 Divisão de Pesquisa

Encontrando, avaliando e sintetizando evidências existentes em vez de gerar dados primários novos.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🔍 [Research Synthesist](research/research-synthesist.md) | Revisão bibliográfica, avaliação crítica de fontes, rastreamento de citações, síntese de evidências | Transformar um conjunto disperso de fontes em um panorama estruturado e bem fundamentado sobre o que a literatura comprova |

---

## 🎯 Casos de Uso Reais

### Cenário 1: Construindo o MVP de uma Startup

**Sua Equipe**:
1. 🎨 **Frontend Developer** — Desenvolver a aplicação React
2. 🏗️ **Backend Architect** — Projetar a API e o banco de dados
3. 🚀 **Growth Hacker** — Planejar a estratégia de aquisição de usuários
4. ⚡ **Rapid Prototyper** — Ciclos rápidos de iteração
5. 🔍 **Reality Checker** — Garantir a qualidade antes do lançamento

**Resultado**: Entregue mais rápido com especialistas cuidando de cada etapa crítica.

---

### Cenário 2: Lançamento de Campanha de Marketing

**Sua Equipe**:
1. 📝 **Content Creator** — Desenvolver o conteúdo das campanhas
2. 🐦 **Twitter Engager** — Estratégia e execução no Twitter/X
3. 📸 **Instagram Curator** — Conteúdo visual e stories
4. 🤝 **Reddit Community Builder** — Engajamento comunitário autêntico
5. 📊 **Analytics Reporter** — Rastrear e otimizar o desempenho das métricas

**Resultado**: Campanha coordenada multicanal com domínio das particularidades de cada plataforma.

---

### Cenário 3: Desenvolvimento de Recursos Corporativos

**Sua Equipe**:
1. 👔 **Senior Project Manager** — Escopo e planejamento de tarefas
2. 💎 **Senior Developer** — Implementação técnica complexa
3. 🎨 **UI Designer** — Design system e componentes visuais
4. 🧪 **Experiment Tracker** — Planejamento de testes A/B
5. 📸 **Evidence Collector** — Verificação e evidência de qualidade
6. 🔍 **Reality Checker** — Validação de prontidão para produção

**Resultado**: Entrega de nível corporativo com controle rigoroso de qualidade e documentação.

---

### Cenário 4: Assunção e Reestruturação de Conta de Mídia Paga

**Sua Equipe**:

1. 📋 **Paid Media Auditor** — Avaliação completa do histórico da conta
2. 📡 **Tracking & Measurement Specialist** — Verificação e correção do rastreamento de conversões
3. 💰 **PPC Campaign Strategist** — Redesenho da estrutura das campanhas
4. 🔍 **Search Query Analyst** — Eliminação de verba gasta em termos irrelevantes
5. ✍️ **Ad Creative Strategist** — Renovação de anúncios e extensões
6. 📊 **Analytics Reporter** (Divisão de Suporte) — Criação de dashboards de desempenho

**Resultado**: Reestruturação metódica da conta com rastreamento verificado, desperdício zerado e novos criativos — tudo dentro dos primeiros 30 dias.

---

### Cenário 5: Discovery Completo de Produto na Agência

**Sua Equipe**: 8 divisões trabalhando em paralelo em uma única missão.

Veja o exemplo em **[Nexus Spatial Discovery Exercise](examples/nexus-spatial-discovery.md)** — um exercício onde 8 agentes (Product Trend Researcher, Backend Architect, Brand Guardian, Growth Hacker, Support Responder, UX Researcher, Project Shepherd e XR Interface Architect) foram acionados simultaneamente para avaliar uma oportunidade de mercado e gerar um plano de produto unificado cobrindo viabilidade técnica, validação de mercado, estratégia de marca, go-to-market, suporte, UX e design espacial.

**Resultado**: Blueprint completo e multidisciplinar de produto produzido em uma única sessão. [Veja mais exemplos](examples/).

---

### Cenário 6: Gêmeo Digital de Campus Inteligente

**Sua Equipe**:

1. 🧠 **Technical Consultant** — Definir a estratégia: BIM para prédios, SIG para o campus, IoT para tempo real
2. 🏗️ **BIM/GIS Specialist** — Converter modelos Revit para camadas de cena SIG e plantas baixas internas
3. 🛸 **Drone/Reality Mapping** — Mapear o campus via drone e gerar ortomosaicos e malha 3D de contexto
4. 🌐 **Web GIS Developer** — Construir o dashboard do campus com MapLibre e buscador de salas
5. 🏔️ **3D & Scene Developer** — Criar a cena 3D interativa com relevo, prédios e tour virtual
6. 🤖 **GeoAI/ML Engineer** — Extrair perímetros de construções e cobertura vegetal das imagens
7. ✅ **GIS QA Engineer** — Validar topologia, precisão posicional e consistência de CRS

**Resultado**: Um gêmeo digital de campus integrando detalhes BIM, realidade capturada por drones, visualização 3D e acesso via web — executado em um pipeline unificado.

---

## 🤝 Como Contribuir

Contribuições são muito bem-vindas! Veja como participar:

### Adicionar um Novo Agente

1. Faça um Fork do repositório
2. Crie um novo arquivo de agente dentro da pasta da divisão correspondente
3. Siga a estrutura padrão de template de agente:
   - Frontmatter com nome, descrição e cor
   - Seção de Identidade e Memória
   - Missão Principal (Core Mission)
   - Regras Críticas (do domínio)
   - Entregáveis Técnicos com exemplos de código
   - Processo do Fluxo de Trabalho (Workflow Process)
   - Métricas de Sucesso
4. Abra um Pull Request com o seu agente

### Aprimorar Agentes Existentes

- Adicione exemplos do mundo real
- Melhore os exemplos de código
- Atualize as métricas de sucesso
- Aperfeiçoe os fluxos de trabalho

### Compartilhe seus Casos de Sucesso

Já usou estes agentes em seus projetos? Conte sua experiência na aba [Discussions](https://github.com/msitarzewski/agency-agents/discussions)!

---

## 📖 Filosofia de Design dos Agentes

Cada agente é construído sobre 5 pilares:

1. **🎭 Personalidade Marcante**: Nada de templates genéricos — voz e postura autênticas
2. **📋 Entregáveis Claros**: Resultados concretos, não orientações vagas
3. **✅ Métricas de Sucesso**: Padrões de qualidade claros e objetivos mensuráveis
4. **🔄 Fluxos Comprovados**: Processos passo a passo que funcionam na prática
5. **💡 Memória de Aprendizado**: Reconhecimento de padrões e busca contínua por melhoria

---

## 🎁 O que Torna Isso Especial?

### Diferente de Prompts Genéricos de IA:
- ❌ Prompts genéricos como "Aja como um desenvolvedor"
- ✅ Especialização profunda com postura, processo e contexto técnico

### Diferente de Bibliotecas de Prompts Tradicionais:
- ❌ Coleções isoladas de perguntas e respostas rápidas
- ✅ Sistemas completos de agentes com fluxos, regras e entregáveis estruturados

### Diferente de Ferramentas de IA Proprietárias:
- ❌ Ferramentas "caixa-preta" sem possibilidade de personalização
- ✅ Personas abertas, transparentes, adaptáveis e fáceis de versionar via Git

---

## 🎨 Destaques de Frases dos Agentes

> "Eu não apenas testo seu código — meu padrão é encontrar de 3 a 5 problemas e exigir prova visual para cada um."
>
> — **Evidence Collector** (Divisão de Testes)

> "Você não está fazendo marketing no Reddit — você está se tornando um membro valioso da comunidade que, por acaso, representa uma marca."
>
> — **Reddit Community Builder** (Divisão de Marketing)

> "Cada elemento lúdico precisa ter um propósito funcional ou emocional. Crie encantamento que some à experiência, em vez de distrair."
>
> — **Whimsy Injector** (Divisão de Design)

> "Deixe-me adicionar uma animação comemorativa aqui; isso reduz a ansiedade de conclusão de tarefa em 40%."
>
> — **Whimsy Injector** (durante uma revisão de UX)

---

## 📊 Números do Projeto

- 🎭 **Mais de 230 Agentes Especializados** em diversas divisões
- 📝 **Mais de 10.000 linhas** de personalidades, processos e exemplos de código
- ⏱️ **Meses de iteração contínua** a partir de casos de uso reais
- 🌟 **Testado em batalha** em ambientes de produção
- 💬 **Mais de 50 solicitações** logo nas primeiras 12 horas no Reddit

---

## 🔌 Integrações Multi-Ferramenta

O The Agency funciona nativamente com o Claude Code e inclui scripts de conversão e instalação para que você possa usar os mesmos agentes nas principais ferramentas de programação com agentes de IA.

### Ferramentas Suportadas

- **[Claude Code](https://claude.ai/code)** — agentes `.md` nativos, sem necessidade de conversão → `~/.claude/agents/`
- **[GitHub Copilot](https://github.com/copilot)** — agentes `.md` nativos, sem necessidade de conversão → `~/.github/agents/` + `~/.copilot/agents/`
- **[Antigravity](https://github.com/google-gemini/antigravity)** — `SKILL.md` por agente → `~/.gemini/config/skills/`
- **[Gemini CLI](https://github.com/google-gemini/gemini-cli)** — arquivos de agentes `.md` → `~/.gemini/agents/`
- **[OpenCode](https://opencode.ai)** — arquivos de agentes `.md` → `.opencode/agents/`
- **[Cursor](https://cursor.sh)** — arquivos de regra `.mdc` → `.cursor/rules/`
- **[Aider](https://aider.chat)** — arquivo único `CONVENTIONS.md` → `./CONVENTIONS.md`
- **[Windsurf](https://codeium.com/windsurf)** — arquivo único `.windsurfrules` → `./.windsurfrules`
- **[OpenClaw](https://github.com/openclaw/openclaw)** — `SOUL.md` + `AGENTS.md` + `IDENTITY.md` por agente
- **[Qwen Code](https://github.com/QwenLM/qwen-code)** — arquivos de SubAgentes `.md` → `~/.qwen/agents/`
- **[Kimi Code](https://github.com/MoonshotAI/kimi-cli)** — especificações de agentes em YAML → `~/.config/kimi/agents/`
- **[Codex](https://developers.openai.com/codex/overview)** — agentes personalizados em TOML → `~/.codex/agents/`
- **Osaurus** — skills em `SKILL.md` → `~/.osaurus/skills/`
- **[Hermes](integrations/hermes/README.md)** — plugin de roteamento inteligente → `~/.hermes/plugins/`

---

### ⚡ Instalação Rápida

**Passo 1 -- Gerar os arquivos de integração:**
```bash
./scripts/convert.sh
# Mais rápido (paralelo, a ordem de saída pode variar): ./scripts/convert.sh --parallel
```

**Passo 2 -- Instalar (interativo, auto-detecta suas ferramentas):**
```bash
./scripts/install.sh
# Mais rápido (paralelo, a ordem de saída pode variar): ./scripts/install.sh --no-interactive --parallel
```

O instalador escaneia o sistema, exibe uma lista de seleção e permite escolher exatamente o que instalar:

```
  +------------------------------------------------+
  |   The Agency -- Tool Installer                 |
  +------------------------------------------------+

  System scan: [*] = detected on this machine

  [x]  1)  [*]  Claude Code     (claude.ai/code)
  [x]  2)  [*]  Copilot         (~/.github + ~/.copilot)
  [x]  3)  [*]  Antigravity     (~/.gemini/antigravity)
  [ ]  4)  [ ]  Gemini CLI      (~/.gemini/agents)
  [ ]  5)  [ ]  OpenCode        (opencode.ai)
  [ ]  6)  [ ]  OpenClaw        (~/.openclaw/agency-agents)
  [x]  7)  [*]  Cursor          (.cursor/rules)
  [ ]  8)  [ ]  Aider           (CONVENTIONS.md)
  [ ]  9)  [ ]  Windsurf        (.windsurfrules)
  [ ] 10)  [ ]  Qwen Code       (~/.qwen/agents)
  [ ] 11)  [ ]  Kimi Code       (~/.config/kimi/agents)
  [ ] 12)  [ ]  Codex           (~/.codex/agents)
  [ ] 13)  [ ]  Osaurus         (~/.osaurus/skills)
  [ ] 14)  [ ]  Hermes          (~/.hermes/plugins)

  [1-14] marcar/desmarcar   [a] todos   [n] nenhum   [d] detectados
  [Enter] instalar   [q] sair
```

**Ou instale diretamente para uma ferramenta específica:**
```bash
./scripts/install.sh --tool cursor
./scripts/install.sh --tool opencode
./scripts/install.sh --tool openclaw
./scripts/install.sh --tool antigravity
./scripts/install.sh --tool codex
./scripts/install.sh --tool osaurus
./scripts/install.sh --tool hermes
```

**Modo não-interativo (para CI / scripts automatizados):**
```bash
./scripts/install.sh --no-interactive --tool all
```

**Execuções mais rápidas (paralelo)** — Em máquinas com múltiplos núcleos de processamento, utilize `--parallel` para que cada ferramenta seja processada em paralelo. Funciona tanto no modo interativo quanto no modo automatizado: por exemplo, `./scripts/install.sh --interactive --parallel` (selecione as ferramentas e instale em paralelo) ou `./scripts/install.sh --no-interactive --parallel`. O número de jobs padrão utiliza `nproc` (Linux), `sysctl -n hw.ncpu` (macOS) ou 4; configure manualmente com `--jobs N`.

```bash
./scripts/convert.sh --parallel                    # converter todas as ferramentas em paralelo
./scripts/convert.sh --parallel --jobs 8           # limitar a 8 jobs paralelos
./scripts/install.sh --no-interactive --parallel   # instalar em todas as ferramentas detectadas em paralelo
./scripts/install.sh --interactive --parallel      # escolher as ferramentas e instalar em paralelo
./scripts/install.sh --no-interactive --parallel --jobs 4
```

---

### Instruções Específicas por Ferramenta

<details>
<summary><strong>Claude Code</strong></summary>

Os agentes são copiados diretamente do repositório para `~/.claude/agents/` — sem necessidade de conversão.

```bash
./scripts/install.sh --tool claude-code
```

Depois, basta chamar no Claude Code:
```
Use the Frontend Developer agent to review this component.
```

Veja mais detalhes em [integrations/claude-code/README.md](integrations/claude-code/README.md).
</details>

<details>
<summary><strong>GitHub Copilot</strong></summary>

Os agentes são copiados diretamente do repositório para `~/.github/agents/` e `~/.copilot/agents/` — sem necessidade de conversão.

```bash
./scripts/install.sh --tool copilot
```

Depois, basta chamar no GitHub Copilot:
```
Use the Frontend Developer agent to review this component.
```

Veja mais detalhes em [integrations/github-copilot/README.md](integrations/github-copilot/README.md).
</details>

<details>
<summary><strong>Antigravity (Gemini)</strong></summary>

Cada agente vira uma skill em `~/.gemini/config/skills/agency-<slug>/`.

```bash
./scripts/install.sh --tool antigravity
```

Ative no Gemini com Antigravity:
```
@agency-frontend-developer review this React component
```

Veja mais detalhes em [integrations/antigravity/README.md](integrations/antigravity/README.md).
</details>

<details>
<summary><strong>Gemini CLI</strong></summary>

Instala como subagentes do Gemini CLI.
Ao clonar o repositório pela primeira vez, gere os arquivos de agente do Gemini antes de rodar o instalador:

```bash
./scripts/convert.sh --tool gemini-cli
./scripts/install.sh --tool gemini-cli
```

Veja mais detalhes em [integrations/gemini-cli/README.md](integrations/gemini-cli/README.md).
</details>

<details>
<summary><strong>OpenCode</strong></summary>

Os agentes são colocados na pasta `.opencode/agents/` na raiz do seu projeto (escopo por projeto).

```bash
cd /seu/projeto
/caminho/para/agency-agents/scripts/install.sh --tool opencode
```

Ou instale globalmente:
```bash
mkdir -p ~/.config/opencode/agents
cp integrations/opencode/agents/*.md ~/.config/opencode/agents/
```

Ative no OpenCode:
```
@backend-architect design this API.
```

Veja mais detalhes em [integrations/opencode/README.md](integrations/opencode/README.md).
</details>

<details>
<summary><strong>Cursor</strong></summary>

Cada agente se torna um arquivo de regra `.mdc` em `.cursor/rules/` dentro do seu projeto.

```bash
cd /seu/projeto
/caminho/para/agency-agents/scripts/install.sh --tool cursor
```

As regras são aplicadas automaticamente quando o Cursor as detecta. Você pode referenciá-las explicitamente:
```
Use the @security-engineer rules to review this code.
```

Veja mais detalhes em [integrations/cursor/README.md](integrations/cursor/README.md).
</details>

<details>
<summary><strong>Aider</strong></summary>

Todos os agentes são compilados em um único arquivo `CONVENTIONS.md`, lido automaticamente pelo Aider.

```bash
cd /seu/projeto
/caminho/para/agency-agents/scripts/install.sh --tool aider
```

Depois, mencione o agente na sessão do Aider:
```
Use the Frontend Developer agent to refactor this component.
```

Veja mais detalhes em [integrations/aider/README.md](integrations/aider/README.md).
</details>

<details>
<summary><strong>Windsurf</strong></summary>

Todos os agentes são compilados no arquivo `.windsurfrules` na raiz do projeto.

```bash
cd /seu/projeto
/caminho/para/agency-agents/scripts/install.sh --tool windsurf
```

Mencione o agente no Cascade do Windsurf:
```
Use the Reality Checker agent to verify this is production ready.
```

Veja mais detalhes em [integrations/windsurf/README.md](integrations/windsurf/README.md).
</details>

<details>
<summary><strong>OpenClaw</strong></summary>

Cada agente se torna um workspace com `SOUL.md`, `AGENTS.md` e `IDENTITY.md` em `~/.openclaw/agency-agents/`.

```bash
./scripts/convert.sh --tool openclaw
./scripts/install.sh --tool openclaw
```

Se a CLI do `openclaw` estiver disponível, o instalador registrará cada workspace automaticamente.
Execute `openclaw gateway restart` após a instalação para ativar os novos agentes.

Veja mais detalhes em [integrations/openclaw/README.md](integrations/openclaw/README.md).

</details>

<details>
<summary><strong>Qwen Code</strong></summary>

Os SubAgentes são instalados em `.qwen/agents/` na raiz do projeto (escopo por projeto).

```bash
# Converter e instalar (execute a partir da raiz do seu projeto)
cd /seu/projeto
./scripts/convert.sh --tool qwen
./scripts/install.sh --tool qwen
```

**Como usar no Qwen Code:**
- Referencie pelo nome: `Use the frontend-developer agent to review this component`
- Ou deixe o Qwen delegar automaticamente com base no contexto da tarefa
- Gerencie via comando `/agents` no modo interativo

> 📚 [Documentação de SubAgentes do Qwen](https://qwenlm.github.io/qwen-code-docs/en/users/features/sub-agents/)

</details>

<details>
<summary><strong>Kimi Code</strong></summary>

Os agentes são convertidos para o formato da CLI do Kimi Code (YAML + prompt de sistema) e instalados em `~/.config/kimi/agents/`.

```bash
# Converter e instalar
./scripts/convert.sh --tool kimi
./scripts/install.sh --tool kimi
```

**Como usar no Kimi Code:**
```bash
# Usar um agente
kimi --agent-file ~/.config/kimi/agents/frontend-developer/agent.yaml

# Dentro de um projeto
kimi --agent-file ~/.config/kimi/agents/frontend-developer/agent.yaml \
     --work-dir /seu/projeto \
     "Review this React component"
```

Veja mais detalhes em [integrations/kimi/README.md](integrations/kimi/README.md).

</details>

<details>
<summary><strong>Codex</strong></summary>

Cada agente é convertido em um arquivo TOML de agente customizado do Codex e instalado em `~/.codex/agents/`.

```bash
./scripts/convert.sh --tool codex
./scripts/install.sh --tool codex
```

Depois, mencione o agente customizado pelo nome no Codex:
```
Use the Frontend Developer agent to review this component.
```

Veja mais detalhes em [integrations/codex/README.md](integrations/codex/README.md).
</details>

---

### Regenerando Arquivos após Alterações

Sempre que adicionar novos agentes ou editar os existentes, gere novamente os arquivos de integração:

```bash
./scripts/convert.sh                    # regenerar todos (sequencial)
./scripts/convert.sh --parallel         # regenerar todos em paralelo (mais rápido)
./scripts/convert.sh --tool codex       # regenerar apenas para uma ferramenta
./scripts/convert.sh --tool cursor      # regenerar apenas para uma ferramenta
```

---

## 🗺️ Roadmap de Desenvolvimento

- [ ] Ferramenta web interativa para seleção de agentes
- [x] Exemplos de fluxos de trabalho multi-agente — veja em [examples/](examples/)
- [x] Scripts de integração multi-ferramenta (Claude Code, GitHub Copilot, Antigravity, Gemini CLI, OpenCode, OpenClaw, Cursor, Aider, Windsurf, Qwen Code, Kimi Code, Codex, Osaurus, Hermes)
- [ ] Tutoriais em vídeo sobre criação de agentes
- [ ] Marketplace comunitário de agentes
- [ ] "Quiz de personalidade" de agentes para recomendação em projetos
- [ ] Série de destaques "Agente da Semana"

---

## 🌐 Traduções e Localizações da Comunidade

Traduções e adaptações regionais mantidas pela comunidade. Estes projetos são mantidos de forma independente — consulte cada repositório para verificar a cobertura e a compatibilidade de versões.

| Idioma | Mantenedor | Link | Observações |
|----------|-----------|------|-------|
| 🇨🇳 简体中文 (zh-CN) | [@jnMetaCode](https://github.com/jnMetaCode) | [agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh) | 141 agentes traduzidos + 46 originais para o mercado chinês |
| 🇨🇳 简体中文 (zh-CN) | [@dsclca12](https://github.com/dsclca12) | [agent-teams](https://github.com/dsclca12/agent-teams) | Tradução independente com foco em Bilibili, WeChat e Xiaohongshu |
| 🇧🇷 Português brasileiro (pt-BR) | [@jnMetaCode](https://github.com/jnMetaCode) | [agency-agents-pt-BR](https://github.com/jnMetaCode/agency-agents-pt-BR) | 184 agentes traduzidos; PRs para o mercado brasileiro são bem-vindos |
| 🇷🇺 Русский (ru) | [@jnMetaCode](https://github.com/jnMetaCode) | [agency-agents-ru](https://github.com/jnMetaCode/agency-agents-ru) | 184 agentes traduzidos; PRs para o mercado russo são bem-vindos |
| 🇮🇩 Bahasa Indonesia (id) | [@jnMetaCode](https://github.com/jnMetaCode) | [agency-agents-id](https://github.com/jnMetaCode/agency-agents-id) | 184 agentes traduzidos; PRs para o mercado indonésio são bem-vindos |
| 🇸🇦 العربية (ar) | [@jnMetaCode](https://github.com/jnMetaCode) | [agency-agents-ar](https://github.com/jnMetaCode/agency-agents-ar) | 184 agentes traduzidos; PRs para o mercado árabe são bem-vindos |
| 🇰🇷 한국어 (ko) | [@jnMetaCode](https://github.com/jnMetaCode) | [agency-agents-ko](https://github.com/jnMetaCode/agency-agents-ko) | 184 agentes traduzidos; PRs específicos para a Coreia são bem-vindos |
| 🇯🇵 日本語 (ja-JP) | [@sscodeai](https://github.com/sscodeai) | [agency-agents-ja](https://github.com/sscodeai/agency-agents-ja) | 281 agentes localizados para o Japão + 97 originais + 27 fluxos de trabalho |
| 🇻🇳 Tiếng Việt (vi-VN) | [@rodonguyen](https://github.com/rodonguyen) | [agency-agents](https://github.com/rodonguyen/agency-agents) | Versão inicial em vietnamita focada no README, início rápido e docs essenciais |

Quer adicionar uma tradução? Abra uma issue no repositório para adicionarmos o link aqui.

---

## 🔗 Recursos Relacionados

- [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) — Coleção de agentes mantida pela comunidade para OpenClaw (derivada deste repositório)

---

## 📜 Licença

Licença MIT — Use livremente, seja para fins comerciais ou pessoais. Créditos são apreciados, mas não obrigatórios.

---

## 🙏 Agradecimentos

O que começou como uma simples conversa no Reddit sobre especialização de agentes de IA transformou-se em um projeto incrível — **mais de 230 agentes distribuídos por todas as divisões**, apoiados por uma comunidade global de colaboradores. Cada agente existe porque alguém se dedicou a escrever, testar e compartilhar.

A todos que abriram um Pull Request, registraram uma issue, iniciaram uma discussão ou simplesmente usaram um agente e compartilharam seu feedback: muito obrigado! Vocês são o motivo pelo qual o The Agency continua evoluindo.

---

## 💬 Comunidade

- **GitHub Discussions**: [Compartilhe suas histórias de sucesso](https://github.com/msitarzewski/agency-agents/discussions)
- **Issues**: [Reporte bugs ou sugira novas funcionalidades](https://github.com/msitarzewski/agency-agents/issues)
- **Reddit**: Participe das conversas em r/ClaudeAI
- **Twitter/X**: Compartilhe usando a hashtag #TheAgency

---

## 🚀 Como Começar

1. **Navegue** pelos agentes listados acima e escolha os especialistas necessários
2. **Copie** os arquivos para `~/.claude/agents/` caso use o Claude Code
3. **Ative** os agentes chamando seus papéis durante as conversas
4. **Personalize** as personas e processos de acordo com as necessidades do seu projeto
5. **Compartilhe** seus resultados e contribua de volta com a comunidade

---

<div align="center">

**🎭 The Agency: O Time dos Sonhos de IA à Sua Disposição 🎭**

[⭐ Dê uma estrela no repo](https://github.com/msitarzewski/agency-agents) • [🍴 Faça um Fork](https://github.com/msitarzewski/agency-agents/fork) • [🐛 Reporte um problema](https://github.com/msitarzewski/agency-agents/issues) • [❤️ Apoie o projeto](https://github.com/sponsors/msitarzewski)

Feito com ❤️ pela comunidade, para a comunidade

</div>
