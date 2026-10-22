# grapeos — Diretrizes de identidade visual para landing page

> **Documento:** guia visual e de interface para a landing page da grapeos  
> **Versão:** 1.0 · 19/10/2026  
> **Status:** referência para design e desenvolvimento  
> **Base:** logotipo, guia de identidade visual e mockups fornecidos pelo projeto

## 1. Objetivo e escopo

Estabelecer regras consistentes para traduzir a identidade da **grapeos** em uma landing page moderna, clara, confiável e responsiva.

Este documento abrange **cores, tipografia, marca, composição, componentes visuais, responsividade e acessibilidade**. Não define a oferta comercial, as funcionalidades reais do produto, os preços nem os textos finais da página. Os conteúdos demonstrativos presentes nos mockups **não devem ser tratados como funcionalidades ou resultados comprovados**.

### 1.1. Atributos da marca

- **Moderna:** tecnologia apresentada com clareza e elegância.
- **Minimalista:** poucos elementos, bem hierarquizados.
- **Amigável:** linguagem visual acessível, formas arredondadas.
- **Tecnológica:** interfaces precisas, modulares e organizadas.
- **Escalável:** identidade aplicável a diversos formatos e tamanhos.
- **Colaborativa:** elementos que sugerem conexão entre pessoas, ideias e processos.

**Princípio visual:** a interface deve simplificar a mensagem, não competir com ela.

---

## 2. Identidade da marca

### 2.1. Logotipo

O logotipo é composto por:

1. **Símbolo:** composição geométrica de **seis círculos** que remete a um cacho de uvas, sem folha ou ornamentos.
2. **Wordmark:** nome **grapeos** em letras minúsculas, com aparência geométrica e arredondada.

**Versões de referência:**

- **Horizontal:** símbolo à esquerda do nome; uso preferencial no cabeçalho da landing page.
- **Símbolo isolado:** ícone para aplicações reduzidas, como favicon ou marcador visual.
- **Aplicação sobre branco:** versão principal em roxo.
- **Aplicação sobre fundo escuro:** utilizar uma versão clara/negativa **somente se existir como arquivo oficial**, sem improvisar alterações no original.

**Regras de uso:**

- Utilizar o arquivo original fornecido, priorizando SVG quando disponível ou PNG transparente de boa resolução.
- Manter proporção, orientação, espaçamento entre símbolo e texto e cores oficiais.
- Não redesenhar o símbolo manualmente para aplicações de produção.
- Não aplicar sombras, contornos, brilhos, deformações, texturas ou gradientes **ao logotipo**.
- Reservar área livre ao redor da marca; como referência inicial, usar no mínimo o diâmetro de um dos círculos do símbolo.
- Não posicionar a marca sobre fotografias ou fundos de baixo contraste.
- Evitar tamanhos em que detalhes e lettering percam legibilidade.

> A tipografia de interface é Poppins/Inter; **não substitua o wordmark original por texto digitado em Poppins**.

### 2.2. Identidade gráfica complementar

O próprio conjunto de círculos do símbolo pode inspirar grafismos de apoio, **sem substituir nem modificar o logo oficial**:

- grupos de círculos em baixa opacidade;
- conexões discretas entre nós;
- cards agrupados representando modularidade e colaboração;
- fundos com formas circulares suaves e recortes amplos.

Esses grafismos devem ser secundários em relação ao conteúdo.

---

## 3. Paleta de cores

### 3.1. Cores oficiais

| Cor | Hexadecimal | Papel na landing page |
|---|---|---|
| **Roxo grapeos** | `#7C4DFF` | Identidade, destaque, elementos de marca e ações principais |
| **Roxo Escuro** | `#5B2EE6` | Hover, links importantes, estados ativos e contrastes fortes |
| **Lilás de Apoio** | `#A78BFA` | Ilustrações, detalhes, ícones e fundos decorativos |
| **Preto Grafite** | `#1F1F29` | Títulos, texto principal e bases escuras |
| **Branco Neve** | `#FFFFFF` | Fundo predominante e áreas de respiro |

### 3.2. Cores auxiliares de interface (propostas, não oficiais)

Estes tons podem ser usados para implementar estados e superfícies. **São recomendações derivadas da paleta**, não novas cores oficiais da marca.

| Token | Valor sugerido | Aplicação |
|---|---|---|
| `--color-surface-soft` | `#F8F6FF` | Seções de fundo alternativo |
| `--color-border` | `#E9E4F5` | Bordas de cards e divisórias |
| `--color-text-muted` | `#606075` | Descrições, legendas e metadados |
| `--color-primary-tint` | `#F0EAFF` | Fundo de ícones e estados suaves |

### 3.3. Distribuição visual sugerida

- **Predominância:** branco e superfícies muito claras.
- **Estrutura:** grafite para títulos e corpo do conteúdo.
- **Ênfase:** roxo para marca, botões, links e palavras-chave.
- **Apoio:** lilás em poucos detalhes, sem competir com a ação principal.

Evitar grandes extensões de roxo saturado em todas as seções. Blocos escuros são permitidos como contraste pontual, se houver necessidade de narrativa visual.

### 3.4. Contraste

- `#1F1F29` sobre branco: adequado para texto principal.
- `#5B2EE6` sobre branco: boa opção para links e destaques textuais.
- `#7C4DFF` sobre branco: pode ser usado em texto normal com contraste AA aproximado de **4,81:1**; verificar a aplicação final.
- `#A78BFA` sobre branco: **não usar em textos pequenos**, pois o contraste é insuficiente para WCAG AA.
- Texto branco sobre botões em `#5B2EE6` ou `#7C4DFF` oferece contraste adequado para texto normal, sem depender de opacidade.

Evitar transparências sobre textos essenciais que reduzam a legibilidade.

---

## 4. Tipografia

### 4.1. Famílias tipográficas

| Uso | Família | Pesos |
|---|---|---|
| Títulos e destaques | **Poppins** | `600` (SemiBold), `700` (Bold) |
| Parágrafos e interface | **Inter** | `400` (Regular), `500` (Medium) |
| Rótulos de botões | **Inter** ou **Poppins** | `600` (SemiBold), conforme consistência do componente |

As fontes devem ser carregadas em versões otimizadas e com `font-display: swap`, sempre que possível.

### 4.2. Escala tipográfica sugerida

| Elemento | Desktop | Mobile | Entrelinha |
|---|---:|---:|---:|
| `H1` / título principal | 52–64 px | 34–42 px | 1.08–1.16 |
| `H2` / título de seção | 36–44 px | 28–34 px | 1.15–1.25 |
| `H3` / título de card | 22–26 px | 20–24 px | 1.2–1.35 |
| Texto de destaque | 18–20 px | 16–18 px | 1.5–1.65 |
| Texto comum | 16–18 px | 16 px | 1.5–1.7 |
| Legenda/rótulo | 13–14 px | 13–14 px | 1.4–1.5 |

**Diretrizes:**

- Usar uma hierarquia inequívoca: apenas um `H1`, seguido de `H2` e `H3` sem saltos arbitrários.
- Preferir títulos curtos com ênfase pontual em roxo, não parágrafos inteiros destacados.
- Limitar parágrafos extensos a aproximadamente **60–75 caracteres por linha**.
- Evitar texto todo em maiúsculas, exceto micro-rótulos curtos.
- Permitir que o texto quebre e aumente com zoom sem sobreposição.

---

## 5. Layout e composição da landing page

### 5.1. Direção visual

A estética esperada é **clean / SaaS moderno**, com predominância de fundo claro, tipografia forte, ilustrações leves e cards com cantos arredondados.

O material de referência utiliza telas de produto, métricas, ícones e conexões como **linguagem visual ilustrativa**. Na landing page real, qualquer tela, métrica ou afirmação deve refletir informações validadas sobre o produto.

### 5.2. Grid e espaçamento (recomendação de implementação)

| Parâmetro | Desktop | Tablet | Mobile |
|---|---|---|---|
| Container máximo | 1.200–1.280 px | Fluido | Fluido |
| Margem lateral | 32–48 px | 24–32 px | 16–24 px |
| Colunas de grid | 12 | 6–8 | 4 |
| Espaço entre colunas | 24 px | 20–24 px | 16 px |
| Espaçamento vertical entre seções | 80–120 px | 64–88 px | 48–72 px |

Usar escala consistente de espaçamento baseada em **múltiplos de 4 px**, com passos frequentes de `8, 12, 16, 24, 32, 48, 64, 80 e 96 px`.

### 5.3. Hierarquia visual

Cada seção deve ter um objetivo visual claro, geralmente nesta ordem:

1. Título ou mensagem central.
2. Descrição complementar.
3. Elemento visual de apoio, se necessário.
4. Ação ou próximo passo, quando pertinente.

Essa sequência é **uma convenção visual**, não uma definição antecipada da estrutura comercial da landing page.

### 5.4. Hero / primeira dobra

Diretrizes para quando a seção principal for criada:

- Dar grande destaque ao título e à proposta de valor **após sua validação**.
- Utilizar uma ou duas colunas no desktop quando a composição justificar; empilhar no mobile.
- Reservar espaço em branco em torno de título, CTA e imagem.
- Destacar uma única ação primária por região visual.
- Usar ilustração ou captura de interface somente se representar corretamente o produto.
- Evitar números inventados, depoimentos fictícios e promessas de resultados sem evidência.

---

## 6. Componentes visuais

### 6.1. Botões

**Primário**

- Fundo: `#7C4DFF`.
- Texto: `#FFFFFF`.
- Hover: `#5B2EE6`.
- Altura alvo: **44–52 px**.
- Raio de borda: **12–16 px** ou estilo pílula quando coerente com a composição.
- Padding horizontal: **20–28 px**.
- Foco por teclado: anel de destaque claramente visível.

**Secundário**

- Fundo: branco ou transparente.
- Borda e texto: `#5B2EE6`.
- Hover: superfície lilás muito clara, sem perder contraste.
- Mesma altura e alinhamento do botão primário.

Não usar mais de um botão com a mesma prioridade visual em um mesmo agrupamento.

### 6.2. Cards

- Fundo: branco ou `#F8F6FF`.
- Borda opcional: `1px solid #E9E4F5`.
- Raio: **16–24 px**.
- Padding interno: **24–32 px** no desktop e **20–24 px** no mobile.
- Sombra opcional, muito suave; preferir bordas quando a hierarquia já estiver clara.
- Ícone ou pequeno elemento ilustrativo com roxo e lilás.
- Títulos curtos, textos objetivos e alinhamentos consistentes.

### 6.3. Ícones e ilustrações

- Estilo preferencial: **outline simples ou formas geométricas limpas**.
- Espessura de traço consistente (aprox. 1,75–2 px quando aplicável).
- Cantos e extremidades levemente arredondados.
- Cores: roxo, grafite e lilás, de maneira controlada.
- Evitar misturar ícones 3D realistas, emojis e ícones de linhas diferentes sem uma decisão estética explícita.

### 6.4. Navegação e rodapé

- Cabeçalho claro, com logotipo horizontal e navegação de boa legibilidade.
- Links com estados de hover, foco e ativo reconhecíveis.
- Mobile: menu acessível por teclado, com identificação explícita para leitores de tela.
- Rodapé: composição discreta, mantendo família tipográfica, espaçamento e paleta.
- Os links e seções concretos serão definidos quando a arquitetura de informação estiver aprovada.

### 6.5. Formulários, se existirem

- Rótulos visíveis para cada campo; placeholders são exemplos, não substitutos de rótulos.
- Campos com área de toque de ao menos **44 px** de altura como referência prática.
- Bordas discretas, foco perceptível e mensagens de erro textuais.
- Estados de sucesso/erro não devem depender somente da cor.
- Não coletar informações além do necessário para a ação solicitada.

---

## 7. Superfícies, efeitos e movimento

- Preferir **fundos brancos e lilás muito suaves**.
- Gradientes e efeitos luminosos, se usados, devem ser discretos e limitados a áreas decorativas; o logotipo oficial permanece inalterado.
- Sombras baixas, com opacidade reduzida e sem contornos pesados.
- Animações curtas e funcionais em botões, cards e transições (em geral **150–250 ms**).
- Evitar paralaxe pesada, elementos que se movem continuamente e excesso de blur.
- Respeitar `prefers-reduced-motion: reduce`.

A interface deve transmitir **fluidez e organização**, nunca excesso de estímulos.

---

## 8. Responsividade e desempenho

- Projetar **mobile-first**, validando as versões para telas menores desde o início.
- Pontos de atenção sugeridos: `480px`, `768px` e `1024px` (ajustar conforme o conteúdo real).
- Empilhar composições de duas ou mais colunas em telas estreitas.
- Não depender de hover para acessar informações importantes.
- Usar imagens responsivas com dimensões definidas para reduzir mudanças de layout.
- Otimizar ícones e imagens; priorizar SVG para vetores oficiais quando disponível e WebP/AVIF para fotografias ou mockups.
- Evitar animações ou bibliotecas que prejudiquem carregamento, navegação e leitura.

### 8.1. Acessibilidade mínima

- Buscar **WCAG 2.2 AA** na implementação.
- Contraste de texto comum de pelo menos **4,5:1** e de texto grande de **3:1**.
- Estrutura semântica: `header`, `nav`, `main`, `section`, `footer`, headings em ordem.
- Imagens informativas com texto alternativo; imagens puramente decorativas sem descrição redundante.
- Ações operáveis por teclado e com foco visível.
- Zoom de texto e navegação em telas pequenas sem perda de conteúdo.
- Rótulos e feedback claros nos componentes interativos.

---

## 9. Design tokens iniciais (CSS)

Os tokens abaixo são um **ponto de partida técnico**. Os valores da paleta principal vêm do guia de marca; medidas e superfícies complementares são sugestões de implementação.

```css
:root {
  /* Cores oficiais da marca */
  --grapeos-purple: #7C4DFF;
  --grapeos-purple-dark: #5B2EE6;
  --grapeos-lilac: #A78BFA;
  --grapeos-graphite: #1F1F29;
  --grapeos-white: #FFFFFF;

  /* Cores auxiliares sugeridas para a interface */
  --color-bg: var(--grapeos-white);
  --color-surface-soft: #F8F6FF;
  --color-surface-accent: #F0EAFF;
  --color-border: #E9E4F5;
  --color-text: var(--grapeos-graphite);
  --color-text-muted: #606075;
  --color-primary: var(--grapeos-purple);
  --color-primary-hover: var(--grapeos-purple-dark);

  /* Tipografia */
  --font-heading: "Poppins", sans-serif;
  --font-body: "Inter", sans-serif;

  /* Geometria sugerida */
  --radius-button: 14px;
  --radius-card: 20px;
  --container-max: 1280px;

  /* Elevação sugerida */
  --shadow-card: 0 12px 32px rgba(31, 31, 41, 0.06);

  /* Movimento sugerido */
  --transition-fast: 180ms ease;
}

@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    transition-duration: 0.01ms !important;
  }
}
```

**Uso recomendado:** centralizar os tokens em arquivo de tema, evitar valores repetidos diretamente em componentes e documentar alterações posteriores.

---

## 10. Organização sugerida de arquivos da marca

Os nomes e caminhos abaixo são **exemplos de organização**, não caminhos já existentes no projeto. Preservar sempre os arquivos oficiais recebidos.

```text
assets/
└── brand/
    ├── grapeos-logo-horizontal.png
    ├── grapeos-logo-transparent.png
    ├── grapeos-symbol.png
    └── references/
        ├── grapeos-brand-guidelines.png
        └── grapeos-brand-mockups.png

docs/
└── IDENTIDADE_VISUAL_GRAPEOS_LANDING_PAGE.md
```

Caso sejam disponibilizados arquivos vetoriais oficiais, preferir `*.svg` para uso web e manter os PNGs como alternativas.

---

## 11. Checklist de consistência visual

- [ ] Logotipo oficial aplicado sem alterações, com margem de segurança.
- [ ] Cores principais correspondem aos hexadecimais definidos.
- [ ] Poppins nos títulos e Inter no corpo, com pesos consistentes.
- [ ] Fundo predominantemente claro; elementos roxos utilizados para hierarquia.
- [ ] Títulos, botões e links têm contraste suficiente.
- [ ] Ícones, cards, bordas e raios seguem o mesmo padrão visual.
- [ ] Componentes mantêm espaçamento consistente.
- [ ] Layout revisado em desktop, tablet e mobile.
- [ ] Navegação, botões e formulários acessíveis por teclado.
- [ ] Imagens e animações otimizadas para desempenho.
- [ ] Capturas, métricas, depoimentos e afirmações de produto foram validados antes de publicar.
- [ ] Copy, estrutura comercial e chamadas para ação aprovadas separadamente.

---

## 12. Referências e limites deste documento

Este guia foi consolidado a partir de quatro materiais fornecidos:

1. Mockup de aplicações da marca e exemplo de página em notebook e celular.
2. Prancha **“Especificação de Identidade Visual — grapeos”**, com cores, fontes e boas práticas.
3. Logotipo horizontal roxo com fundo transparente.
4. Logotipo horizontal roxo aplicado em fundo branco.

**Definições confirmadas pelos materiais:** nome, símbolo, paleta oficial, tipografia de comunicação, atributos e direção visual.

**Decisões sugeridas por este documento:** tamanhos, breakpoints, espaçamentos, raios, superfícies auxiliares, tokens e comportamentos de componentes. Essas sugestões podem ser refinadas na etapa de criação da landing page.

**Ainda não definidos:** posicionamento comercial, público-alvo, proposta de valor final, funcionalidades confirmadas, plano de seções, conteúdo, depoimentos, métricas, preços e CTAs definitivos.

> **Diretriz final:** a grapeos deve parecer uma marca tecnológica acessível e bem estruturada, com clareza de comunicação, aplicação rigorosa de sua identidade e foco em legibilidade e confiança.
