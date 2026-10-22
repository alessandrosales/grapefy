# grapeos — Especificação de layout da landing page

> **Versão:** 1.0 — 19/10/2026  
> **Status:** especificação para design e implementação  
> **Idioma:** pt-BR  
> **Referência estrutural:** [Thrad](https://www.thrad.ai/?ref=land-book.com)  
> **Fonte de verdade para identidade:** `IDENTIDADE_VISUAL_GRAPEOS_LANDING_PAGE.md`  
> **Fonte de verdade para textos comerciais:** `COPY_LANDING_PAGE_GRAPEOS.md`

## 1. Objetivo

Construir uma landing page **original do grapeos**, inspirada na **linguagem de composição e narrativa visual** do site Thrad: títulos grandes, hierarquia editorial clara, alternância entre áreas de impacto e demonstrações visuais, módulos que explicam o produto, conteúdo em etapas, provas de credibilidade e chamadas comerciais recorrentes.

**Não criar um clone da Thrad.** A referência orienta o **ritmo, a arquitetura de informação e os padrões de apresentação**; marca, elementos gráficos, paleta, tipografia, conteúdo, ilustrações e componentes finais devem ser próprios do grapeos.

**Meta de conversão:** gerar contatos qualificados por dois caminhos:

1. **Principal:** iniciar conversa comercial via WhatsApp.
2. **Secundário:** preencher formulário para receber contato.

**Produto comunicado:** infraestrutura preparada para equipes autônomas de agentes de IA, personalizadas, pré-treinadas e operando com baixa intervenção humana, segurança, orientação, suporte e manutenção.

### 1.1. O que foi aproveitado da referência Thrad

A página consultada apresenta, em sequência, estes padrões de arquitetura:

| Padrão observado na referência | Tradução visual para grapeos |
|---|---|
| Navegação objetiva com ação comercial | Header enxuto com CTA de WhatsApp |
| Hero de grande impacto com dois CTAs | Promessa de produtividade em tipografia expressiva |
| Faixa de marcas/cases | Faixa de diferenciais reais (sem inventar logos de clientes) |
| Demonstração por interfaces e categorias selecionáveis | Demonstração de *equipes autônomas* por área, com tabs funcionais |
| Fluxo operacional em quatro módulos (`Analyze → Rank → Bid → Deploy`) | Fluxo próprio de trabalho dos agentes (`Objetivo → Plano → Execução → Entrega`) |
| Apresentação do produto com etapas numeradas e tela | Processo de implantação, canais e exemplo de interação |
| Depoimentos e atualizações verificáveis | Exemplos ilustrativos claramente sinalizados; cases reais somente quando autorizados |
| Grande fechamento comercial com CTAs | Convite final para conversar e formulário integrado |

**Nota sobre fidelidade:** a organização e as seções acima foram verificadas no conteúdo público do site. Capturas disponíveis em buscadores mostram versões visuais anteriores da Thrad; por isso, medidas, cores, animações e detalhes *pixel-perfect* desta especificação são **decisões propostas para o grapeos**, não medições exatas do CSS atual da referência.

### 1.2. Decisões inegociáveis

- **Marca oficial:** usar o arquivo original do logotipo grapeos, sem redesenhá-lo.
- **Marca visual:** fundo predominantemente branco, grafite em texto, roxo em ações, lilás em apoio.
- **Tipos:** Poppins para títulos; Inter para textos e interface.
- **Conceito central:** visualizar **uma equipe de agentes coordenados**, não apenas um chatbot individual.
- **Conteúdo:** respeitar `COPY_LANDING_PAGE_GRAPEOS.md`; este arquivo especifica onde e como posicionar a copy, não a substitui.
- **Sem números inventados:** não usar percentuais, clientes, testemunhos ou métricas hipotéticas como se fossem reais.
- **Performance e acessibilidade** fazem parte dos critérios de aceite.

---

## 2. Direção de arte

### 2.1. Personalidade visual

- **Tech editorial:** títulos fortes, poucos elementos por bloco, comunicação de alto nível.
- **Sofisticado, mas próximo:** interfaces amigáveis, formas circulares derivadas do símbolo da uva, bastante respiro.
- **Concreto:** mostrar objetivos, papéis, atividades, canais e entregas — evitar robôs humanoides e ilustrações genéricas de cérebro de IA.
- **Modular:** cards, timelines e diagramas que expressam composição de equipes.
- **Alto contraste:** botões e elementos interativos facilmente identificáveis.

### 2.2. Paleta obrigatória

| Token | HEX | Função |
|---|---|---|
| Roxo grapeos | `#7C4DFF` | Identidade, botões, pontos de atenção |
| Roxo Escuro | `#5B2EE6` | Hover, estados ativos, links de maior contraste |
| Lilás de Apoio | `#A78BFA` | Conexões, ilustrações, indicadores secundários |
| Preto Grafite | `#1F1F29` | Títulos e texto principal; bloco de contraste eventual |
| Branco Neve | `#FFFFFF` | Superfície dominante |

**Neutros auxiliares sugeridos (não são novas cores oficiais):**

| Token | Valor | Uso |
|---|---|---|
| `surface-soft` | `#F8F6FF` | Seções alternadas e fundos sutis |
| `surface-accent` | `#F0EAFF` | Destaques de ícones e tabs |
| `border-soft` | `#E9E4F5` | Separadores e cartões |
| `text-muted` | `#606075` | Descrições e legendas |

**Distribuição orientativa:** 75–85% superfícies claras, 10–15% grafite/texto, 5–10% roxo/lilás como ênfase. São proporções de intenção, não quotas rígidas.

**Bloco escuro:** permitido em **uma** seção de alto impacto (ex.: demonstração ou CTA final) usando `#1F1F29`; preservar o restante claro. Sobre bloco escuro, usar contraste seguro e versão aprovada do logo, caso presente.

### 2.3. Tipografia

| Elemento | Fonte / peso | Desktop | Mobile | Line-height |
|---|---|---:|---:|---:|
| H1 / hero | Poppins 700 | `clamp(3.25rem, 4.5vw, 4rem)` | `2.125–2.625rem` | 1.08–1.14 |
| H2 / seções | Poppins 600/700 | `2.25–2.75rem` | `1.75–2.125rem` | 1.15–1.22 |
| H3 / cards | Poppins 600 | `1.25–1.625rem` | `1.125–1.375rem` | 1.25–1.35 |
| Lead / destaque | Inter 400/500 | `1.125–1.25rem` | `1rem` | 1.5–1.65 |
| Corpo | Inter 400 | `1rem–1.125rem` | `1rem` | 1.55–1.7 |
| Botão | Inter 600 | `0.9375–1rem` | `0.9375–1rem` | 1.2 |
| Eyebrow / label | Inter 500/600 | `0.75–0.875rem` | `0.75–0.875rem` | 1.4 |

- No máximo **um H1** na página.
- Usar negrito e **uma expressão em roxo por título** quando fizer sentido; não pintar o parágrafo inteiro.
- Evitar títulos recortados ou texto impossível de ler em zoom de 200%.
- Não tentar reconstruir o lettering da marca com Poppins: o nome no cabeçalho deve usar o logo original.

### 2.4. Formas, bordas e profundidade

- Cards: raio **20–24 px**, borda `1px solid #E9E4F5`.
- Botões: raio **14–16 px**; tamanho mínimo `44px` de altura.
- Painéis de demonstração: raio **24–28 px**.
- Chips/tags: cápsulas com bordas suaves.
- Sombra muito leve; dar preferência a contorno, espaço e contraste de fundo.
- Formas circulares do símbolo grapeos como elemento decorativo em escala ampliada e **baixa opacidade**, sem modificar o logotipo.
- Não usar gradiente no arquivo do logo; gradientes muito discretos podem existir apenas como fundo de seção ou ilustração.

---

## 3. Malha de layout e responsividade

### 3.1. Breakpoints orientativos

| Contexto | Largura | Container e colunas | Margem lateral | Espaçamento vertical |
|---|---|---|---|---|
| Wide desktop | `≥ 1440px` | `max-width: 1280px`, 12 colunas | `48px` | `96–120px` |
| Desktop | `1024–1439px` | fluido, 12 colunas | `32px` | `80–104px` |
| Tablet | `768–1023px` | fluido, 8 colunas | `24px` | `64–88px` |
| Mobile | `< 768px` | fluido, 4 colunas | `16–20px` | `56–72px` |

- Use um único container compartilhado pelo header e seções principais.
- `gap` de colunas: 24–32 px (desktop); 16–20 px (mobile).
- Alinhe bordas de cards, títulos e painéis ao mesmo eixo horizontal.
- Seções com fundo full-bleed podem ter conteúdo limitado ao container.
- Nunca provocar scroll horizontal em viewport de `320px`.

### 3.2. Ritmo da página

Alternar **tipografia em grande escala** com **interfaces tangíveis**. Evitar uma sequência monótona de grades idênticas de três cards.

**Padrão recomendado:** hero amplo → visual de demonstração → problema → fluxo de trabalho → equipes por área → benefícios → implantação → segurança → contratação → FAQ → CTA/formulário.

---

## 4. Mapa da página e âncoras

O designer/desenvolvedor deve usar a seguinte ordem inicial; alteração só depois de revisão da jornada comercial.

| Ordem | Bloco / âncora | Formato visual | Função |
|---|---|---|---|
| 01 | `#topo` | Header fixo + hero editorial | Compreensão imediata e conversão |
| 02 | `#demonstracao` | Painel grande de equipe de IA | Tangibilizar a solução |
| 03 | `#desafio` | Texto forte + três pontos de dor | Construir identificação |
| 04 | `#solucao` | Quatro cards/painéis conectados | Explicar autonomia operacional |
| 05 | `#equipes` | Seletor de áreas + conteúdo demonstrativo | Mostrar aplicações |
| 06 | `#beneficios` | Bento grid assimétrico | Associar recursos a resultados |
| 07 | `#como-funciona` | Timeline em quatro etapas | Reduzir percepção de complexidade |
| 08 | `#seguranca` | Bloco de confiança em duas colunas | Superar objeções de dados |
| 09 | `#diferenciais` | Serviço incluído + canais | Justificar contratação gerenciada |
| 10 | `#exemplos` | Três exemplos **ilustrativos** | Ajudar a imaginar o uso |
| 11 | `#contratacao` | Cards de setup e mensalidade | Esclarecer modelo comercial |
| 12 | `#faq` | Accordion | Resolver dúvidas |
| 13 | `#contato` | CTA editorial + formulário | Captar lead |
| 14 | `#rodape` | Footer enxuto | Navegação e informações legais |

**Fidelidade à copy:** as seções `A dor`, `A solução`, `Equipes e aplicações`, `Benefícios`, `Como funciona`, `Segurança`, `Diferenciais`, `Exemplos`, `Modelo de contratação`, `FAQ` e `Chamada final` devem herdar seu texto do documento de copy. Este mapa reorganiza a **apresentação**, não altera a oferta ou cria funcionalidades.

---

## 5. Especificação seção por seção

### 5.1. Header / navegação — `#topo`

**Composição:** uma linha compacta, sobre branco, alinhada com o container. Pode ter efeito *sticky* após a primeira rolagem, com fundo branco opaco ou quase opaco e borda inferior discreta.

```text
┌─────────────────────────────────────────────────────────────────┐
│ [LOGO grapeos]  Solução  Equipes  Como funciona  Segurança FAQ │
│                                        [Conversar no WhatsApp]   │
└─────────────────────────────────────────────────────────────────┘
```

- Logo horizontal à esquerda, altura visual aproximada de 28–36 px; usar o arquivo oficial.
- Links no centro/direita, sem excesso de menus aninhados.
- CTA destacado à direita: **Conversar com um especialista**.
- Altura: 72–80 px desktop; 64–72 px mobile.
- Mobile: logo + botão de menu claramente rotulado; CTA pode ficar dentro do menu ou em espaço reduzido, sem esconder navegação.
- Links funcionam com rolagem para as âncoras; compensar a altura do header com `scroll-margin-top`.
- Não incluir links sem destino ou atalhos que abram páginas inexistentes.

### 5.2. Hero editorial — `#topo`

**Referência de ritmo:** headline grande, mensagem enxuta, CTA imediato e transição para a visualização de produto. A palavra de benefício mais importante pode receber ênfase em roxo.

**Layout desktop:** texto com largura controlada no centro/esquerda de uma região ampla; um pequeno cluster de círculos decorativos ao fundo ou na extremidade oposta. **Não sobrepor desenho ao texto.** O painel de produto vem logo abaixo, como continuidade do hero, em vez de disputar atenção numa coluna estreita.

```text
┌──────────────────────────────────────────────────────────────────────┐
│ [EYEBROW: Equipes autônomas de IA para empresas]                   │
│                                                                      │
│ MULTIPLIQUE A PRODUTIVIDADE                                         │
│ da sua empresa com equipes                                           │
│ autônomas de IA.                                                     │
│                                                                      │
│ Texto de apoio limitado a 2–4 linhas no desktop.                     │
│                                                                      │
│ [Quero montar minha equipe de IA]   [Solicitar contato]              │
│                                                                      │
│ [Implantação em até 48h*] [Agentes preparados] [Ambientes isolados]  │
│                                                                      │
│          ┌──────────────────────────────────────────────┐            │
│          │ PREVIEW VISUAL DE EQUIPE DE IA                │            │
│          └──────────────────────────────────────────────┘            │
└──────────────────────────────────────────────────────────────────────┘
```

**Elementos:**

- Eyebrow pequeno em roxo escuro ou texto grafite com ponto circular roxo.
- **H1:** texto aprovado em `COPY_LANDING_PAGE_GRAPEOS.md`; preservar sem abreviações não aprovadas.
- Subtítulo com largura máxima de `660–750px`.
- CTA primário: botão roxo preenchido → WhatsApp real.
- CTA secundário: botão outline/ghost → `#contato`.
- Microbenefícios abaixo dos botões, com divisores e ícones discretos.
- **Nota de 48 h:** manter asterisco e condições aplicáveis, sem promessa universal quando houver restrições.
- Acima da dobra de um desktop típico, priorizar headline, descrição e pelo menos um CTA; o mockup pode continuar após a dobra.

**Mobile:** H1 34–42px, alinhamento à esquerda, CTAs empilhados ou um abaixo do outro em largura total. Chips em duas linhas. Ilustração passa abaixo da mensagem. Evitar animações que atrasem o surgimento do CTA.

### 5.3. Demonstração protagonista — `#demonstracao`

**Esta é a principal peça visual da landing page.** Deve transmitir a diferença entre um chatbot individual e uma **equipe orquestrada de agentes especializados**.

**Componente recomendado:** `TeamOrchestrationShowcase` — painel composto, exclusivo do grapeos, em fundo `#F8F6FF` ou branco com borda leve.

```text
┌────────────────────── SUA EQUIPE DE IA ──────────────────────────────┐
│ Objetivo recebido: "Preparar uma nova funcionalidade"              │
│                                                                      │
│      [Coordenador]                                                   │
│        ╱     ╲                                                      │
│  [Backend]  [Frontend]   [Revisor]                                    │
│        ╲     ╱          ╱                                            │
│        [Tarefas em andamento]  →  [Entrega para avaliação]           │
│                                                                      │
│ Canal: Telegram  |  Status: exemplo ilustrativo                      │
└──────────────────────────────────────────────────────────────────────┘
```

**Detalhes de composição:**

- Painel com borda `#E9E4F5`, raio 24–28px e bastante espaço interno.
- Agentes como módulos individuais com avatar geométrico abstrato, papel, status e linha de conexão.
- Um elemento maior para **objetivo compartilhado**; outros menores para agentes; saída clara para **entrega**.
- Ícones específicos por papel (ex.: código, arquivos, checklist, análise), de uma mesma biblioteca visual.
- A mini-interface pode incluir um recorte de conversa do Telegram/WhatsApp, **mas não pode ser só um chat**.
- Se não houver captura real, sinalizar `Demonstração ilustrativa do funcionamento` de modo visível.
- **Proibido inventar métricas** (`+62% de eficiência`, tarefas reais concluídas, disponibilidade etc.).
- Se houver interação, tabs/botões precisam atualizar os cartões e serem navegáveis por teclado; não criar controles decorativos.
- Fallback para imagem estática otimizada se animação/script não carregar.

### 5.4. Faixa de confiança sem logos fictícios

Na Thrad há uma sequência de marcas associadas a credibilidade. Para o grapeos **não reproduzir uma logo wall de empresas não comprovadas**.

**Alternativa apropriada:** uma faixa horizontal de três fatos do serviço, sem números não validados:

- `Ambientes preparados e personalizados`
- `Acesso seguro e integrações seguras`
- `Suporte e manutenção contínuos`

Textos alinhados horizontalmente no desktop e empilhados no mobile. Usar separadores discretos, sem cards pesados. Eventuais logos/cases de clientes somente com autorização.

### 5.5. Problema / dor — `#desafio`

**Layout:** composição editorial 40/60 ou 45/55: esquerda com título forte e parágrafo; direita com **três linhas de desafio** em cards/linhas numeradas.

```text
[TÍTULO ALTO IMPACTO]         01  Custos operacionais elevados
[PARÁGRAFO DE APOIO]         02  Contratação de especialistas
                            03  Tarefas repetitivas
```

- Fundo branco; separadores horizontais entre dores.
- Priorizar o problema em linguagem de empresário, não jargão de engenharia de agentes.
- Destaques roxos restritos a números ou palavras de ênfase.
- Mobile: título e parágrafo acima dos três itens; sem colunas minúsculas.

### 5.6. Como os agentes trabalham — `#solucao`

**Adaptação explícita dos quatro módulos da Thrad:** em vez de copiar *Analyze/Rank/Bid/Deploy*, definir **um fluxo original do grapeos**, coerente com o produto.

| Etapa | Nome | Painel visual | Conteúdo |
|---|---|---|---|
| `01` | **Recebem objetivos** | cartão de solicitação | Empresa define resultado desejado |
| `02` | **Planejam** | quadro de etapas | Equipe desdobra tarefas e prioridades |
| `03` | **Executam juntos** | conexões entre agentes | Especialistas dividem responsabilidades |
| `04` | **Entregam resultados** | cartão de entrega | Materiais ou execução são disponibilizados para acompanhamento e revisão quando necessário |

**Layout desktop:** quatro módulos visuais relacionados, preferencialmente grade `2×2` com cards grandes e assimetria moderada (ou sequência horizontal somente se a leitura ficar confortável). Cada um exibe um pequeno mockup, não apenas um ícone e texto.

**Comportamento:** scroll reveal discreto e opcional; não exigir scroll-jacking nem animação para entender a sequência. Setas/conexões apenas como ornamento, sem poluição visual.

**Mobile:** quatro cards em coluna, com `01–04` claros; sem carrossel obrigatório para conteúdo essencial.

### 5.7. Equipes por área — `#equipes`

**Referência:** apresentação por contexto/aba, na qual o visitante escolhe a aplicação e vê uma demonstração relevante.

**Áreas previstas:**

1. Desenvolvimento de software.
2. Administrativo.
3. Contabilidade e financeiro.
4. Marketing.
5. Jurídico.
6. Suporte e operações.

**Layout:** título + descrição; abaixo uma barra de tabs/chips e painel de demonstração `40% texto / 60% visual` no desktop.

```text
[Desenvolvimento] [Administrativo] [Financeiro] [Marketing] [Jurídico] [Suporte]
┌──────────────────────┬─────────────────────────────────────────────┐
│ Equipe de            │ [Coordenador] → [Agentes especializados]   │
│ desenvolvimento      │ [Atividades] → [Entrega para revisão]      │
│                      │                                             │
│ Casos de uso reais/  │ Exemplo ilustrativo claramente sinalizado │
│ planejados + CTA     │                                             │
└──────────────────────┴─────────────────────────────────────────────┘
```

- Conteúdo de cada aba precisa corresponder às áreas da copy oficial.
- Mudança de aba atualiza título, texto, papeis e visual; inclui atributos de acessibilidade de tabs.
- Não prometer que todas as integrações e tarefas estão disponíveis sem avaliar o escopo.
- Em jurídico e financeiro, sinalizar que certas saídas exigem revisão de profissional responsável.
- Mobile: tabs com rolagem horizontal *visível* e indicador de aba ativa, painel empilhado; opção alternativa é accordion.

### 5.8. Benefícios — `#beneficios`

**Layout bento**, com assimetria intencional para não parecer uma grade genérica repetitiva.

```text
┌─────────────────────────────┬───────────────────┐
│ PRODUTIVIDADE               │ ESCALABILIDADE    │
│ Card largo com demonstração │ Card de texto     │
├────────────────────┬────────┴───────────────────┤
│ MENOS REPETIÇÃO    │ DISPONIBILIDADE CONFORME    │
│                    │ CONFIGURAÇÃO E CONDIÇÕES    │
└────────────────────┴────────────────────────────┘
```

- Card principal maior para produtividade.
- Benefícios: produtividade, crescimento eficiente, operação com disponibilidade estendida, redução de tarefas repetitivas e foco humano em decisões.
- Evitar KPI inventado; usar microcenários qualitativos ou visuais abstratos.
- Cada bloco: título, uma frase curta e elemento que comunica o benefício.
- Fundo alternado `#F8F6FF`; bordas suaves.
- Mobile: uma coluna, card principal primeiro; mesmo conteúdo visível sem hover.

### 5.9. Implantação em quatro etapas — `#como-funciona`

**Fazer uma timeline com quatro passos claros**:

1. Diagnóstico das necessidades e regras.
2. Preparação do ambiente e agentes.
3. Orientação para o uso.
4. Início da utilização — **até 48 horas**, sujeito às condições do escopo.

**Desktop:** linha horizontal fina com quatro marcadores circulares roxos e cards compactos abaixo; alternativamente `50/50` com etapas à esquerda e ilustração à direita. **Escolher apenas um formato**, evitando duplicação visual.

**Mobile:** linha vertical à esquerda com marcadores; cada passo ocupa a largura disponível.

**CTA após timeline:** `Quero começar com a grapeos` → WhatsApp.

### 5.10. Segurança — `#seguranca`

**Layout:** duas colunas. Esquerda com texto e três garantias **factuais**; direita com visual de infraestrutura isolada.

```text
┌────────────────────────────────┬──────────────────────────────────┐
│ AUTONOMIA COM SEGURANÇA        │ [Ambiente Empresa A]            │
│                                │          │ acesso seguro        │
│ • Ambientes isolados           │ [Agentes / serviços isolados]   │
│ • Acesso seguro                │          │                      │
│ • Integrações seguras          │ [Conexão a canal autorizado]    │
└────────────────────────────────┴──────────────────────────────────┘
```

- O diagrama comunica **separação de ambientes**, não certificação externa ou blindagem absoluta.
- Usar linguagem técnica apenas no nível necessário para gerar confiança.
- **Não ilustrar** auditoria, criptografia ponta a ponta, selos LGPD/ISO ou monitoramento 24/7 como capacidades garantidas sem confirmação.
- Fundo branco ou grafite pontual, se o restante da página for claro; garantir contraste.
- Mobile: texto primeiro, diagrama depois.

### 5.11. Diferenciais e canais — `#diferenciais`

**Layout:** grande título `Toda a capacidade da IA, sem começar pela complexidade técnica` e quatro diferenciais com microvisuais:

- Ambiente preparado para uso.
- Agentes pré-treinados para a finalidade.
- Implantação orientada.
- Suporte e manutenção.

**Canais suportados inicialmente:** Telegram, WhatsApp e clientes personalizados. Representar esses canais como **ícones e nomes**, sem afirmar integrações adicionais não confirmadas.

**Visual:** linhas ou blocos com tipografia, em vez de replicar a seção bento. Pode incluir mini captura de um agente em canal de mensagem, com rótulo `exemplo ilustrativo` se for um conceito.

### 5.12. Exemplos de aplicação — `#exemplos`

A referência Thrad possui depoimentos/cases; o grapeos ainda não forneceu os detalhes verificáveis dos três casos informados no briefing.

**Tratar esta seção como `Cenários de aplicação`**, **não como `Depoimentos` nem `Resultados de clientes`**.

- Exemplo A: time de desenvolvimento.
- Exemplo B: rotinas administrativas e financeiras.
- Exemplo C: marketing e pesquisa de mercado.

**Layout:** três painéis com número, área, situação, ação possível e benefício potencial — sem números ou nomes inventados. Rótulo geral visível: `Exemplos ilustrativos — não representam resultados medidos de clientes`.

**Evolução futura:** substituir por cases reais somente após receber dados e autorização; manter o componente projetado para imagem real, contexto, desafio, solução, resultado validado e fonte.

### 5.13. Modelo de contratação — `#contratacao`

**Dois cards lado a lado**, discretos e fáceis de escanear, sem tabela de preços inventados:

- **Setup inicial:** diagnóstico, preparação e personalização do ambiente.
- **Mensalidade:** suporte e manutenção conforme escopo.

**Cabeçalho:** `Sua operação é única. Sua equipe de IA também deve ser.`

**Rodapé do bloco:** `Solicite uma proposta personalizada` → `#contato`; botão secundário WhatsApp conforme copy aprovada.

Não mostrar valores, `a partir de`, desconto, período de teste nem custos incluídos sem definição comercial. Esclarecer detalhes de consumo/infraestrutura e integrações na proposta.

### 5.14. FAQ — `#faq`

**Layout:** título/introdução à esquerda, accordion de perguntas à direita (desktop). Mobile em uma coluna.

Perguntas devem ser extraídas integralmente de `COPY_LANDING_PAGE_GRAPEOS.md`, sobre: diferença para chatbot, necessidade de conhecimento em IA, autonomia e revisão, prazo, canais, áreas, segurança, substituição de equipe, contratação e personalização.

- Primeira pergunta pode vir aberta; restantes fechadas.
- Ícone `+ / −` ou chevron com rotação discreta.
- Implementar `button` semântico, `aria-expanded`, região de conteúdo e navegação por teclado.
- Texto permanece disponível sem JavaScript quando tecnicamente viável (`details/summary` é opção).

### 5.15. CTA final + formulário — `#contato`

**Este é o equivalente funcional do fechamento de alto impacto da Thrad, com conversão adaptada ao grapeos.**

**Desktop:** título grande e chamada comercial em uma coluna; na coluna oposta formulário com borda leve e fundo branco. Fundo da seção `#F8F6FF` ou, caso escolhido como **único bloco escuro** da página, grafite com formulário branco. Evitar roxo saturado atrás de campos de formulário.

```text
┌────────────────────────────────────────────────────────────────┐
│ SUA PRÓXIMA EQUIPE                                              │
│ PODE SER DE IA.                 ┌────────────────────────────┐ │
│                                 │ Nome                       │ │
│ [Conversar no WhatsApp]         │ Empresa                    │ │
│                                 │ WhatsApp / E-mail          │ │
│ Ou prefira receber contato →    │ Área de interesse          │ │
│                                 │ Necessidade principal      │ │
│                                 │ [Solicitar contato]        │ │
│                                 └────────────────────────────┘ │
└────────────────────────────────────────────────────────────────┘
```

**Campos previstos:** nome, empresa, WhatsApp, e-mail corporativo, área de interesse e necessidade principal, conforme copy.

- Labels visíveis; não depender apenas de placeholder.
- Validação de campos e retorno acessível de sucesso/erro; não afirmar envio antes de confirmação real.
- Checkbox/aviso de privacidade conforme a política publicada e critérios jurídicos aplicáveis.
- Botão de formulário: `Solicitar contato`.
- WhatsApp com texto inicial da copy e número **real a configurar**, nunca um link fictício como se estivesse funcionando.
- Mobile: headline e CTA WhatsApp primeiro, depois formulário em largura total.

### 5.16. Rodapé — `#rodape`

- Logo horizontal oficial, se legível no fundo escolhido.
- Descrição curta do grapeos.
- Âncoras importantes da página e `Fale conosco`.
- Links reais para Política de Privacidade e Termos de Uso (quando publicados).
- Dados institucionais verificados; sem endereço, CNPJ ou e-mail fictícios.
- Pequeno detalhe geométrico inspirado nos círculos da marca; não criar outro logotipo.

---

## 6. Componentes reutilizáveis

| Componente conceitual | Props/dados principais | Estado / interação |
|---|---|---|
| `SiteHeader` | logo, navItems, primaryCTA | sticky, menu mobile, foco |
| `PrimaryCTA` | label, destino, trackingName | hover, foco, loading quando cabível |
| `SecondaryCTA` | label, targetId | rolagem suave com fallback |
| `SectionHeading` | eyebrow, title, description, align | responsivo |
| `TeamOrchestrationShowcase` | objective, agents, tasks, outcome, isIllustrative | estático ou animado de forma discreta |
| `AgentNode` | papel, ícone, estado, descrição | tooltips apenas para conteúdo suplementar |
| `WorkflowStage` | number, title, description, visual | sequência legível sem animação |
| `TeamCategoryTabs` | categories, selectedCategory | tabs semânticas, teclado |
| `BenefitBento` | benefits | reordenação responsiva |
| `SetupTimeline` | steps | horizontal → vertical |
| `SecurityDiagram` | nodes, labels | diagrama acessível com texto alternativo |
| `ScenarioCard` | type, problem, application, disclaimer | rotular ilustrativo |
| `FAQAccordion` | question, answer | expand/collapse |
| `LeadForm` | fields, validation, submitHandler | estados de envio reais |
| `SiteFooter` | links, legal, logo | links válidos |

**Importante:** estes são nomes de arquitetura sugeridos, **não uma imposição de framework**. A implementação pode ser Vue/Quasar, Nuxt, React ou outra, preservando comportamento e aparência.

---

## 7. Design tokens sugeridos para implementação

Os tokens abaixo complementam o guia de identidade; se algum detalhe divergir do arquivo de identidade, **o guia de identidade prevalece**.

```css
:root {
  /* Cores oficiais */
  --brand-primary: #7C4DFF;
  --brand-primary-dark: #5B2EE6;
  --brand-lilac: #A78BFA;
  --ink: #1F1F29;
  --white: #FFFFFF;

  /* Apoio visual (propostas, não cores oficiais) */
  --surface: #FFFFFF;
  --surface-soft: #F8F6FF;
  --surface-tint: #F0EAFF;
  --stroke: #E9E4F5;
  --ink-secondary: #606075;

  /* Fontes */
  --font-display: 'Poppins', sans-serif;
  --font-ui: 'Inter', sans-serif;

  /* Container / medidas */
  --container-max: 1280px;
  --gutter-mobile: 20px;
  --gutter-tablet: 24px;
  --gutter-desktop: 40px;
  --header-height: 76px;

  /* Geometria */
  --radius-sm: 12px;
  --radius-button: 14px;
  --radius-card: 22px;
  --radius-panel: 28px;

  /* Escala de espaço */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-6: 24px;
  --space-8: 32px;
  --space-12: 48px;
  --space-16: 64px;
  --space-20: 80px;
  --space-24: 96px;

  /* Efeitos sutis */
  --card-shadow: 0 12px 32px rgb(31 31 41 / 6%);
  --ease-ui: cubic-bezier(.2, .8, .2, 1);
  --duration-fast: 180ms;
  --duration-medium: 320ms;
}

@media (prefers-reduced-motion: reduce) {
  html { scroll-behavior: auto; }
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    transition-duration: 0.01ms !important;
  }
}
```

**Regra de contraste:** usar `#5B2EE6` para pequenos links quando necessário, `#1F1F29` no corpo e branco sobre botões roxos. O lilás `#A78BFA` é decorativo e não deve carregar texto pequeno essencial sobre branco.

---

## 8. Interações, movimento e comportamento

A referência sugere uma experiência viva e demonstrativa. Para o grapeos, preferir **movimento funcional** em vez de efeitos exagerados.

### 8.1. Permitidos

- Hover e foco de botões com mudança controlada de superfície/contorno.
- Revelação sutil de módulos ao entrar na viewport (`opacity` + pequeno deslocamento), mantendo o conteúdo acessível sem JS.
- Tabs funcionais na demonstração por área.
- Atualização discreta do diagrama de agentes **apenas se fizer sentido**; duração suave e estado estático legível.
- Scroll até âncoras, respeitando `prefers-reduced-motion`.
- Accordion de FAQ.

### 8.2. Evitar

- Scroll-jacking, animações longas obrigatórias ou bloqueio de rolagem.
- Carrosséis automáticos de conteúdo essencial.
- Efeitos 3D pesados, partículas constantes, vídeos em autoplay com som, paralaxe agressiva.
- Telas simuladas que se passem por dados ao vivo.
- Cursor customizado, textos piscantes ou CTAs móveis que encubram campos de formulário.

---

## 9. Imagens e ativos

### 9.1. Arquivos de referência já fornecidos pelo projeto

- `Logo grapeos Roxo Minimalista(1).png` — logotipo em versão fornecida.
- `Logotipo grapeos em Roxo Minimalista(1).png` — aplicação horizontal da marca.
- `Guia de Identidade Visual grapeos(1).png` — prancha com paleta e tipografia.
- `4e859975-2b41-4b9d-81ba-61ad4a2e5d85.png` — mockups e aplicações da marca.

Estes nomes identificam **materiais recebidos nesta conversa**, não presumem a pasta onde estarão no projeto final.

### 9.2. Ativos a produzir para o site (não estão prontos)

1. **Hero orchestration scene:** diagrama/mini-interface da equipe de IA recebendo um objetivo.
2. **Seis visualizações de áreas:** variações de conteúdo para as tabs.
3. **Quatro miniaturas de fluxo:** objetivo, plano, execução, entrega.
4. **Diagrama de ambientes isolados:** conceitual e sem promessas técnicas não confirmadas.
5. **Imagem Open Graph:** composição exclusiva com logo e proposição do grapeos.
6. **Favicon:** derivado do símbolo original, exportado em formato apropriado.

**Produção:** preferir SVG elaborado a partir de elementos de UI próprios, CSS e ilustrações vetoriais limpas. Não tentar copiar ilustrações, gráficos, mockups ou assets proprietários da Thrad. Não usar os mockups da marca como prova de interface operacional real.

---

## 10. Acessibilidade, SEO, LGPD e desempenho

### Acessibilidade

- WCAG 2.2 nível AA como meta de implementação.
- Estrutura com `header`, `main`, `section`, `nav`, `footer` e títulos semânticos.
- Todos os botões e tabs operáveis por teclado e com foco visível.
- Área de toque de ao menos 44×44 px para controles principais.
- Contraste validado na implementação real, incluindo hover/focus/disabled.
- Alternativas textuais para diagramas de equipe que contenham informação relevante.
- `prefers-reduced-motion` respeitado, com fallback estático.
- Formulário com labels, erros vinculados aos campos e anúncio de confirmação acessível.

### SEO e rastreabilidade

- Título, descrição, H1 e textos devem vir de `COPY_LANDING_PAGE_GRAPEOS.md`.
- Um H1, headings em ordem lógica, conteúdo essencial presente no HTML renderizado.
- Definir Open Graph e favicon oficiais.
- Eventos de conversão distintos: `click_whatsapp_hero`, `click_whatsapp_header`, `click_whatsapp_final`, `open_form`, `lead_form_submit_success`.
- Coletar parâmetros UTM sem expor dados pessoais em ferramentas analíticas.
- Configurar consentimento/cookies e privacidade conforme os serviços realmente utilizados e as regras aplicáveis.

### Performance

- Priorizar LCP do hero: título/CTA visíveis sem esperar animações pesadas.
- Imagens com dimensões declaradas; carregar assets abaixo da dobra sob demanda.
- Fontes otimizadas (`woff2`, subset quando apropriado, `font-display: swap`).
- Não carregar frameworks de animação apenas para pequenas transições.
- Objetivos de qualidade orientativos: boas pontuações de Core Web Vitals e ausência de grandes deslocamentos de layout.

---

## 11. Responsividade — checklist por componente

| Componente | Desktop | Mobile |
|---|---|---|
| Header | logo + links + CTA | logo + menu funcional |
| Hero | texto grande e espaço para demo abaixo | H1 menor, CTA prioritário, demo abaixo |
| Microbenefícios | faixa horizontal | wrap/empilhamento |
| Demo de agentes | painel amplo, conexões visíveis | cards reorganizados em pilha/diagrama simplificado |
| Problema | duas colunas | texto acima + itens abaixo |
| Fluxo operacional | grade 2×2 / cards largos | cards empilhados `01–04` |
| Tabs de equipes | barra de categorias + painel dividido | tabs roláveis/accordion + painel em coluna |
| Benefícios bento | composição assimétrica | uma coluna |
| Implantação | timeline horizontal | timeline vertical |
| Segurança | texto + diagrama | texto acima + diagrama simplificado |
| Contratação | dois cards | cards empilhados |
| FAQ | título ao lado do accordion | accordion largura total |
| CTA e formulário | duas colunas | CTA primeiro, formulário depois |

**Viewports mínimas a testar:** `320`, `375`, `430`, `768`, `1024`, `1280`, `1440` e `1920px`. Testar também orientação landscape e zoom do navegador.

---

## 12. Prioridade de construção

### Fase 1 — Essencial para publicar

1. Tema/tokens, fonte e assets oficiais do logotipo.
2. Header, hero e CTAs reais.
3. Demo estática da equipe com rótulo ilustrativo.
4. Dor, fluxo operacional, equipes e benefícios.
5. Implantação, segurança, diferenciais e contratação.
6. FAQ, formulário real, CTA final e rodapé.
7. Responsividade, SEO, acessibilidade, política de privacidade e eventos.

### Fase 2 — Evolução sem bloquear lançamento

- Tabs mais ricas e mudanças de cenários na demo.
- Animações de execução de agentes bem discretas.
- Vídeo demonstrativo real.
- Cases verificados/autorizados e depoimentos reais.
- Testes A/B em hero e CTAs, com mensuração.

---

## 13. Critérios de aceite

### Identidade

- [ ] Logotipo original aplicado corretamente, sem ser redesenhado.
- [ ] Cores oficiais e Poppins/Inter conforme guia.
- [ ] Estética clara e tecnológica, com elementos da uva como inspiração discreta.
- [ ] Nenhum ativo proprietário da Thrad foi copiado.

### Layout

- [ ] Hero editorial forte, CTA visível e demo protagonista.
- [ ] Seções têm ritmo visual variado: sem repetição excessiva de grades idênticas.
- [ ] O visitante entende que o grapeos fornece **equipes coordenadas de IA**, não apenas chatbot.
- [ ] Painéis de agentes, tabs e cards mantêm boa leitura no mobile.
- [ ] Todas as âncoras e ações funcionam.

### Conteúdo e confiança

- [ ] Copy alinhada ao documento aprovado.
- [ ] Benefícios sem métricas ou resultados não comprovados.
- [ ] Cenários hipotéticos sinalizados como **ilustrativos**.
- [ ] Segurança descrita somente com medidas confirmadas.
- [ ] Promessa de 48 horas apresenta condições reais de aplicabilidade.
- [ ] Conteúdos jurídico/financeiro não sugerem substituição de responsabilidade profissional.

### Conversão

- [ ] Botões de WhatsApp usam número oficial e mensagem inicial adequada.
- [ ] Formulário envia dados para serviço real, com estados de sucesso/erro.
- [ ] Mobile permite contato sem atrito e sem popups que obstruam a página.
- [ ] Eventos de conversão disparados corretamente e sem dados pessoais nos parâmetros.

### Qualidade técnica

- [ ] Layout testado nos breakpoints definidos, sem overflow horizontal.
- [ ] Navegação por teclado, contraste e movimento reduzido verificados.
- [ ] Imagens, fontes e scripts otimizados.
- [ ] Metadados SEO/OG e políticas configurados antes de publicar.

---

## 14. Como utilizar este documento no projeto

**Hierarquia de fontes (em caso de conflito):**

1. `IDENTIDADE_VISUAL_GRAPEOS_LANDING_PAGE.md` — decisões oficiais de marca.
2. `COPY_LANDING_PAGE_GRAPEOS.md` — mensagem, oferta, promessa, CTAs e conteúdo textual.
3. **Este arquivo** — organização espacial, referências de composição, componentes, interações e responsive design.

**Instrução ao implementador:** “Crie a landing page do grapeos seguindo o layout e os componentes descritos neste documento, usando a identidade visual oficial e importando os textos aprovados do arquivo de copy. Inspirar-se na hierarquia editorial e na organização modular da Thrad, sem reproduzir seus assets, cores, textos ou design de maneira literal. Usar exemplos apenas como demonstrações claramente sinalizadas. Entregar página responsiva, acessível e com CTAs/formulário funcionais.”

### Referências

- Inspiração arquitetural consultada: https://www.thrad.ai/?ref=land-book.com
- Identidade grapeos: materiais gráficos fornecidos no briefing + `IDENTIDADE_VISUAL_GRAPEOS_LANDING_PAGE.md`.
- Conteúdo grapeos: briefing de 20 perguntas + `COPY_LANDING_PAGE_GRAPEOS.md`.

> **Resultado esperado:** uma landing page com aparência própria do grapeos, estrutura editorial marcante e explicações visuais de times autônomos de IA, orientada a converter visitantes de Google Ads, Instagram, Facebook e tráfego orgânico em conversas comerciais qualificadas.
