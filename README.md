# grapeos — Landing Page

Este repositório reúne as definições de conteúdo, identidade visual, layout e ativos de marca para construir a landing page da **grapeos**. A página deve apresentar equipes autônomas de IA para empresas e converter visitantes em conversas pelo WhatsApp ou solicitações enviadas pelo formulário.

> **Estado atual:** o repositório ainda não contém código ou configuração de framework. Os arquivos presentes são as referências que devem orientar a implementação.

## Prioridade de leitura e decisão

Siga esta ordem ao construir a página. Em caso de conflito, o arquivo de maior prioridade prevalece.

| Prioridade | Arquivo | Papel na landing page |
|---:|---|---|
| 1 | [`IDENTIDADE_VISUAL_GRAPEOS_LANDING_PAGE.md`](./IDENTIDADE_VISUAL_GRAPEOS_LANDING_PAGE.md) | Fonte de verdade da marca: cores, tipografia, logo, componentes, responsividade e acessibilidade. |
| 2 | [`COPY_LANDING_PAGE_GRAPEOS.md`](./COPY_LANDING_PAGE_GRAPEOS.md) | Fonte de verdade do conteúdo: proposta de valor, textos, CTAs, FAQ, formulário, SEO e pendências comerciais. |
| 3 | [`LAYOUT_LANDING_PAGE_GRAPEOS_REFERENCIA_THRAD.md`](./LAYOUT_LANDING_PAGE_GRAPEOS_REFERENCIA_THRAD.md) | Arquitetura de informação, ordem das seções, comportamento dos componentes e direção de layout. |
| 4 | Ativos `.png` | Materiais visuais oficiais ou de referência usados conforme a finalidade indicada abaixo. |

## Mapa completo dos arquivos atuais

### Documentação essencial

| Arquivo | Importância | Uso na implementação |
|---|---|---|
| [`IDENTIDADE_VISUAL_GRAPEOS_LANDING_PAGE.md`](./IDENTIDADE_VISUAL_GRAPEOS_LANDING_PAGE.md) | **Crítica** | Implementar os tokens oficiais: roxo `#7C4DFF`, roxo escuro `#5B2EE6`, lilás `#A78BFA`, grafite `#1F1F29` e branco `#FFFFFF`; usar Poppins em títulos e Inter em textos; preservar o logo original; seguir as regras de contraste, grid, breakpoints e WCAG 2.2 AA. |
| [`COPY_LANDING_PAGE_GRAPEOS.md`](./COPY_LANDING_PAGE_GRAPEOS.md) | **Crítica** | Fonte dos textos aprovados para navegação, hero, dor, solução, áreas, benefícios, implantação, segurança, diferenciais, cenários, contratação, FAQ, formulário, rodapé e metadados SEO. Não inventar métricas, cases, promessas ou informações comerciais. |
| [`LAYOUT_LANDING_PAGE_GRAPEOS_REFERENCIA_THRAD.md`](./LAYOUT_LANDING_PAGE_GRAPEOS_REFERENCIA_THRAD.md) | **Alta** | Traduz a copy em uma página: header, hero, painel de orquestração de agentes, seções, tabs, timeline, accordion, formulário e rodapé. A referência Thrad orienta ritmo e estrutura — nunca copiar seus assets, textos ou interface literalmente. |
| [`Guia de Identidade Visual Grapeos.png`](./Guia%20de%20Identidade%20Visual%20Grapeos.png) | **Média** | Prancha visual que confirma logo, símbolo, paleta, tipografias e boas práticas. Serve para conferência rápida; as regras implementáveis e completas estão no documento de identidade visual. |

### Ativos de marca e referência

| Arquivo | Dimensões | Importância | Uso permitido/recomendado |
|---|---:|---|---|
| [`logo-transparente.png`](./logo-transparente.png) | 1983 × 793 | **Alta** | Versão horizontal roxa da marca em fundo transparente. Prioridade para aplicações em fundos escuros ou quando a transparência for necessária; validar o contraste final antes do uso. |
| [`logo.png`](./logo.png) | 1448 × 1086 | **Alta** | Logotipo horizontal aplicado sobre fundo branco. Usar como referência ou fallback em fundos claros; não é o ativo mais adequado quando for necessário transparência. |
| [`simbolo.png`](./simbolo.png) | 427 × 427 | **Alta** | Símbolo isolado, com transparência. Usar para favicon, ícone de aplicação, marcação visual e elementos pequenos — sem redesenhar, deformar ou adicionar efeitos ao arquivo oficial. |
| [`mockup.png`](./mockup.png) | 1448 × 1086 | **Média** | Referência de aplicações da marca e direção estética. **Não usar como screenshot de produto, prova social ou demonstração funcional**: contém conceitos e métricas ilustrativas. Pode orientar a criação de visuais originais da landing page. |

## Estrutura atual

```text
.
├── README.md
├── COPY_LANDING_PAGE_GRAPEOS.md
├── IDENTIDADE_VISUAL_GRAPEOS_LANDING_PAGE.md
├── LAYOUT_LANDING_PAGE_GRAPEOS_REFERENCIA_THRAD.md
├── Guia de Identidade Visual Grapeos.png
├── logo-transparente.png
├── logo.png
├── simbolo.png
└── mockup.png
```

## Roteiro para construir a landing page

1. **Criar a base técnica** — definir framework, estrutura de páginas, CSS/tokens, fontes Poppins e Inter e diretório de ativos.
2. **Aplicar identidade primeiro** — criar tokens de cor, tipografia, espaçamento, raios, foco visível e comportamento de movimento reduzido conforme o guia visual.
3. **Montar a jornada na ordem definida** — `topo` → demonstração → desafio → solução → equipes → benefícios → como funciona → segurança → diferenciais → exemplos → contratação → FAQ → contato → rodapé.
4. **Inserir a copy sem alterar a oferta** — usar o documento de copy como origem de títulos, descrições, CTAs, FAQ, mensagens de formulário e SEO.
5. **Construir conversão real** — configurar número oficial do WhatsApp, destino do formulário, consentimento/política de privacidade e eventos de conversão. Não publicar links ou confirmações fictícias.
6. **Validar antes de publicar** — testar responsividade, teclado, contraste, formulário, âncoras, redução de movimento, performance e pendências comerciais indicadas na copy.

## Regras indispensáveis

- A página deve comunicar **uma equipe coordenada de agentes de IA**, não apenas um chatbot.
- O logo e o símbolo devem ser usados como foram fornecidos: sem redesenho, deformação, sombra, brilho ou gradiente aplicado ao ativo.
- Manter fundo predominantemente claro; roxo para ações e ênfases; lilás apenas como apoio decorativo, não em textos pequenos sobre branco.
- Cenários de uso são **ilustrativos** até existirem cases autorizados e verificáveis.
- A promessa de implantação em até 48 horas deve preservar condições de escopo e disponibilidade.
- Não alegar certificações, garantias absolutas de segurança, integrações, métricas ou resultados sem validação técnica e comercial.
- A landing page deve ser responsiva, acessível e preparada para os CTAs de WhatsApp e formulário.

## Pendências para publicação

As principais pendências estão detalhadas em [`COPY_LANDING_PAGE_GRAPEOS.md`](./COPY_LANDING_PAGE_GRAPEOS.md). Antes de publicar, confirmar ao menos:

- número oficial e fluxo de atendimento do WhatsApp;
- serviço real de recebimento do formulário e mensagens de sucesso/erro;
- Política de Privacidade, Termos de Uso e dados institucionais;
- aplicabilidade comercial da implantação em até 48 horas;
- alegações de segurança, canais, integrações e limites do serviço;
- rastreamento de conversões sem expor dados pessoais.
