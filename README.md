# SKILOFRENIKHZ | Presença Digital de Artista
## Portfólio + Ferramenta Interativa · Desenvolvido por Fluency Works

> **Cliente:** Giovanni Ramos Garcia — SkiloFrenikhz  
> **Segmento:** DJ e Produtor Musical · Psy Techno · Bounce · Acid Rave · 140+ BPM · Piraju, SP  
> **Booking:** Somma  
> **Desenvolvimento:** Claudio Santana — [Fluency Works](https://fluencyworks.com.br)  
> **Deploy:** [skilofrenikhz.github.io/skilo](https://skilofrenikhz.github.io/skilo/)

---

## Sobre o Projeto

Presença digital completa para DJ independente com identidade de marca forte. O projeto entrega dois produtos distintos: um **portfólio profissional** com player de áudio real e sistema de booking, e uma **ferramenta interativa proprietária** — o Skilo Beat Machine — que vai além do que qualquer site de artista costuma ter.

O briefing partiu de uma demanda simples: um site que "não parecesse genérico". O resultado foi uma construção com design system próprio, identidade visual brutalist-psicodélica, e uma ferramenta de engajamento interativo que se tornou parte central da presença digital do artista.

---

## O Que Foi Entregue

### 1. Site Portfólio — `index.html`

Presença digital completa do artista. Responsivo, com identidade visual coesa do primeiro ao último pixel.

| Seção | O que faz |
|-------|-----------|
| **Hero** | Apresentação do artista com efeitos de glitch, mascote interativo e cursor customizado |
| **Bio** | História e posicionamento artístico — Psy Techno, Bounce e Acid Rave |
| **Sonic Arsenal** | Player HTML5 com 4 faixas reais (WAV), controle de progresso, troca de track, BPM sync visual |
| **Galeria** | Carrossel Swiper.js com fotos do Unistellar Festival (Paranapanema, SP) |
| **Gig History** | Histórico de apresentações |
| **Rider Técnico** | Especificações técnicas para contratantes |
| **Booking** | Gerador de mensagem para WhatsApp — monta o contato automaticamente |
| **Beat Machine Teaser** | Seção de entrada para a ferramenta interativa |

### 2. Skilo Beat Machine — `skilo-beat-machine.html`

Ferramenta interativa proprietária desenvolvida com Web Audio API — sem samples externos, tudo sintetizado em código. Funciona no browser, sem instalação.

**Engine de som:**
- 6 canais: PSY KICK · ACID CLAP · CLOSED HAT · OPEN HAT · PSY BASS · TEKK STAB
- Osciladores e síntese de ruído — 100% Web Audio API
- BPM 120–160 (padrão 140) com controle de swing

**Funcionalidades:**
| Feature | Descrição |
|---------|-----------|
| **16 Steps / 4 Banks** | VOID BREAKER · ACID DROP · PSY LOCK · BLANK |
| **Tap Tempo** | Captura BPM por toque |
| **Mute / Solo** | Isolamento por canal |
| **Pitch por canal** | Slider −12/+12 semitons afeta a frequência do oscilador |
| **CAVE MODE** | Reverb cavernoso via DelayNode realimentado, escurece a UI |
| **HATE MODE** | Distorção WaveShaperNode, troca paleta para vermelho |
| **Stage Mode** | Fullscreen com UI mínima para performance ao vivo |
| **Osciloscópio** | Canvas com waveform em tempo real |
| **Visualizador de frequências** | Canvas FFT com barras responsivas ao som |
| **Share / Import Pattern** | Codifica pattern em string (btoa JSON) para copiar e compartilhar |
| **Glitch Flash no Kick** | Overlay ciano pisca em cada hit do PSY KICK |
| **BPM Pulse Sync** | UI pulsa na cadência exata do BPM via CSS custom property |
| **Mascote reativo** | persona.png treme no kick, glitch visual a cada 4 bars |

---

## Design System

Identidade visual criada do zero para o projeto — não usa template. Aplicada em ambas as páginas com consistência total.

| Token | Valor | Uso |
|-------|-------|-----|
| `--void-black` | `#0d0d0f` | Fundo geral |
| `--toxic-volt` | `#5ce1e6` | Accent principal — PSY / tecnologia |
| `--frenzy-gold` | `#eca035` | Destaque secundário — groove / calor |
| `--bloodshed-red` | `#e74c3c` | Tensão / HATE / alerta |
| `--chrome-white` | `#ffffff` | Tipografia primária |

**Tipografia:** Teko (bold italic — headers de impacto) + Space Mono (monospace — dados, labels, código)

**Estilo:** Brutalism digital com glitch effects, scanline overlay, sombras brutas, clip-path em botões, animações de distorção CSS. Visual coerente com a sonoridade psicodélica e industrial do artista.

---

## Stack Técnica

| Tecnologia | Uso |
|-----------|-----|
| HTML5 / CSS3 / Vanilla JS | Estrutura, estilo e lógica — sem framework |
| Tailwind CSS (CDN) | Utilitários de layout responsivo |
| Google Fonts | Teko + Space Mono |
| Swiper.js (CDN) | Carrossel da galeria |
| **Web Audio API** | Player HTML5 real + Beat Machine sintetizado |
| GitHub Pages | Deploy e hospedagem |

Sem build step. Sem dependências de servidor. Dois arquivos HTML autocontidos.

---

## Estrutura de Arquivos

```
skilofrenikhz/
├── index.html                          # Portfólio principal
├── skilo-beat-machine.html             # Ferramenta interativa
├── assets/
│   ├── img/
│   │   ├── logo.png
│   │   ├── persona.png                 # Mascote do artista
│   │   ├── profile/
│   │   │   ├── foto-gi.png
│   │   │   └── foto-gi-tocando.png
│   │   └── gallery/
│   │       ├── unistellar-3640.jpg
│   │       ├── unistellar-3674.jpg
│   │       ├── unistellar-3687.jpg
│   │       ├── unistellar-3693.jpg
│   │       └── unistellar-3749.jpg
│   └── audio/
│       ├── faixa-01.wav
│       ├── faixa-02.wav
│       ├── faixa-03.wav
│       └── faixa-04.wav
├── .gitattributes
├── .gitignore
└── README.md
```

---

## Como Rodar Localmente

Nenhum build necessário. Qualquer servidor web serve.

**XAMPP:**
```
Pasta: C:\xampp\htdocs\skilo\
URL:   http://localhost/skilo/
```

**VS Code Live Server:**
```
Clique direito em index.html → Open with Live Server
```

**Python:**
```bash
python -m http.server 8080
# http://localhost:8080
```

---

## Classificação do Projeto — Fluency Works

Este projeto se enquadra em **duas camadas de infraestrutura** da Fluency Works:

### Camada 01 — Brand (embutida)
Design system completo criado do zero para o artista: tokens de cor, tipografia dual, elementos visuais proprietários (scanlines, glitch, clip-paths), aplicação consistente em todas as superfícies digitais.

### Camada 02 — Presence (principal)
Site portfólio profissional com múltiplas seções, player HTML5 com áudio real, galeria de fotos, histórico de shows, rider técnico e sistema de booking via WhatsApp. Equivalente a um **Site Institucional Robusto** do portfólio Fluency.

### Camada 03 — Platform (diferencial)
O Skilo Beat Machine é uma **ferramenta digital proprietária** — não é um componente de site, é um produto interativo. Comportamento equivalente a um **Motor Simples** do Fluency OS aplicado ao setor criativo: lógica de produto, estado, síntese de áudio, persistência de pattern, interação em tempo real.

### Posição no guia de preços

| Entregável | Referência Fluency | Faixa |
|-----------|-------------------|-------|
| Portfólio + Design System | Site Institucional Robusto | R$ 3.500–5.500 |
| Beat Machine interativo | Motor Simples / Feature Custom | R$ 800–1.500 |
| Care mensal | Care Padrão | R$ 120–180/mês |
| **Total setup estimado** | | **R$ 4.300–7.000** |

### Vertical de mercado
Projeto pioneiro na vertical **"Artistas e DJs"** — demonstra que a camada Presence + Platform da Fluency se aplica ao mercado criativo com o mesmo rigor técnico dos sistemas para negócios físicos. Candidato a vertical **Fluency Stage**.

---

## Resultados e Diferenciais

- Presença digital profissional que representa a identidade sonora do artista com fidelidade
- Player HTML5 com áudio real — nenhuma simulação, nenhum embed de terceiro
- Ferramenta interativa exclusiva que gera engajamento além do portfólio padrão
- Deploy no GitHub Pages — zero custo de hospedagem para o artista
- Código limpo, semântico, sem dependências críticas — manutenção simples

---

## Créditos

**Artista:** Giovanni Ramos Garcia — SkiloFrenikhz  
**Booking:** Somma  
**Desenvolvimento:** Claudio Santana — [Fluency Works](https://fluencyworks.com.br)

---

© 2026 SKILOFRENIKHZ | 140+ BPM · Todos os direitos reservados  
Desenvolvido por Fluency Works · Piraju, SP
