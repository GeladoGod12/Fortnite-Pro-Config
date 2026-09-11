# Fortnite Pro Config Hub 2026

Hub competitivo de Fortnite: configurações de **controle**, **teclado + mouse** e **mobile**, rotinas de treino, mapas Creative, vídeos, builds dos tops, gravação de tela e **IA Coach** (Grok + Gemini).

**Atualizado · Setembro 2026**

---

## Demonstração

Abra os arquivos no navegador (Chrome, Edge ou Firefox recomendados).

Não precisa de build, servidor Node nem dependências — é HTML, CSS e JavaScript puro.

| Arquivo | O que é |
|---|---|
| `index.html` | Hub principal (configs, treinos, mapas, vídeos, tops) |
| `Tutorial.html` | IA Coach (chat com Grok ou Gemini) |

---

## Funcionalidades do Hub (`index.html`)

### Configurações competitivas
| Plataforma | Conteúdo |
|---|---|
| **Controle** | Builder Pro, sensibilidade avançada (Exponential), deadzone, multiplicadores de build/edit, aim assist |
| **Teclado + Mouse** | DPI 800, eDPI, sensibilidade, keybinds |
| **Mobile** | Gráficos, look/ADS/scope, turbo building |
| **Vídeo** | Performance Mode, 1080p, NVIDIA Reflex, sombras/AA off |

### Treinos
- **30 min** — aquecimento (aim, piece control, box 2v2)
- **1 hora** — sessão completa
- **2 horas** — evolução + VOD review

### Mapas Creative
Clique no código para copiar:
- **MECÂNICA PRO V4** — `9235-0277-4070`
- Piece Control 2v2 — `0148-0322-5437`
- Piece Moving Bots — `9510-9643-4467`
- PANDVIL Piece Control — `8321-0751-6633`

### Vídeos, tops e ferramentas
- Tutoriais de piece control (YouTube embutido)
- Builds de **Sky**, **Malibuca** e **Peterbot**
- Gravar tela → download `.webm`
- Imprimir / salvar PDF
- Botão **ℹ️ IA Coach** → abre `Tutorial.html`

---

## IA Coach (`Tutorial.html`)

Chat focado em Fortnite com suporte a **duas IAs**:

| Provedor | Onde pegar a key | Modelos |
|---|---|---|
| **Grok (xAI)** | [console.x.ai](https://console.x.ai) → API Keys | `grok-3` |
| **Gemini (Google)** | [aistudio.google.com](https://aistudio.google.com) → Get API key | `gemini-2.0-flash`, `1.5-flash`, `1.5-pro` |

### O que a IA faz
- Monta treinos de 30 min / 1h / 2h
- Dicas de piece control, aim, box fights, high ground
- Sugestões de mapas Creative
- Settings de controle e KBM
- Ideias de vídeo, títulos, thumbnails e roteiros de Shorts
- Meta e loadouts

### Como usar a IA

1. Abra `Tutorial.html` (ou clique em **ℹ️ IA Coach** no Hub).
2. No topo, escolha o provedor: **Grok** ou **Gemini**.
3. Clique em **🔑 Keys**.
4. Cole a API key correspondente e salve.
5. (Gemini) Escolha o modelo no mesmo modal.
6. Use os atalhos da barra lateral ou digite sua pergunta.
7. Enter envia · Shift+Enter faz nova linha.

### Atalhos prontos
- Treino 30 min / 1 hora
- Melhores mapas
- Melhorar aim / piece control
- Ideias de vídeo e roteiro de Short
- Sens controle / keybinds KBM / meta atual

### Avisos da IA
- As keys ficam só no **seu navegador** (`localStorage`).
- Colocar API key no frontend é **apenas para uso pessoal/teste**.
- Não compartilhe o arquivo HTML com a key salva.
- Em produção o ideal é um backend/proxy para esconder a key.
- Uso das APIs consome cota/créditos da sua conta (Grok ou Google).

---

## Como usar o Hub

### 1. Abrir
1. Baixe os arquivos.
2. Abra `index.html` no navegador.

(Opcional) Servidor local:

```bash
python -m http.server 8080
# ou
npx serve .
```

Acesse: `http://localhost:8080`

### 2. Navegar
Menu sticky: **Controle · Teclado + Mouse · Mobile · Vídeo · Treinos · Mapas · Vídeos Truques · Top 3 Builds**

### 3. Aplicar configs
1. Escolha a plataforma.
2. Ative **Opções Avançadas** no Fortnite quando indicado.
3. Copie os valores e ajuste ao conforto.

### 4. Treinar
1. Vá em **Treinos** e escolha 30 min, 1 h ou 2 h.
2. Copie o código do mapa em **Mapas**.
3. Cole no Creative e siga a rotina.

### 5. Gravar a tela
1. Clique em **Gravar**.
2. Escolha a janela/aba e confirme.
3. **Parar & Baixar** gera o `.webm`.

> Melhor em Chrome, Edge ou Firefox. Pode exigir HTTPS ou `localhost`.

### 6. IA Coach
Clique em **ℹ️ IA Coach** na toolbar ou abra `Tutorial.html` direto.

---

## Estrutura

```text
.
├── index.html      # Hub principal
├── Tutorial.html   # IA Coach (Grok + Gemini)
└── README.md       # Este arquivo
```

---

## Tecnologias

- HTML5 + CSS3 (variáveis, grid, sticky nav, responsivo)
- JavaScript vanilla
  - Navegação, abas, cópia de códigos
  - Gravação de tela (`getDisplayMedia` + `MediaRecorder`)
  - Chat com APIs (xAI Grok + Google Gemini)
  - `localStorage` para keys e preferências

**Sem frameworks, sem npm, sem build.**

---

## Compatibilidade

| Recurso | Suporte |
|---|---|
| Layout e configs | Navegadores modernos |
| Copiar código de mapa | Chrome, Edge, Firefox, Safari |
| Gravação de tela | Chrome, Edge, Firefox |
| IA Coach (API) | Chrome, Edge, Firefox (requer internet + key) |
| Impressão / PDF | Todos |

---

## Deploy

Qualquer host estático:

- GitHub Pages
- Netlify / Vercel / Cloudflare Pages
- itch.io

Coloque `index.html` e `Tutorial.html` na mesma pasta.

> Se for publicar online, **não deixe API keys salvas** no navegador de quem for usar. Cada usuário deve colocar a própria key.

---

## Fontes dos dados

- Power Rankings e resultados competitivos (2026)
- Settings públicos de pros (ex.: Peterbot)
- Guias (ProSettings, setup.gg e similares)
- Mapas Creative da comunidade

Valores são **pontos de partida**. Adapte ao seu hardware e preferência.

---

## Avisos

- Não afiliado à Epic Games.
- Fortnite é marca da Epic Games, Inc.
- Códigos de mapa e settings podem mudar.
- Respeite privacidade ao gravar a tela.
- API keys são de responsabilidade do usuário (custos e limites das plataformas).

---

## Licença

Uso livre para fins educacionais e da comunidade competitiva.

---

## Créditos

Feito para a comunidade competitiva de Fortnite.  
Consistência > cópia cega. Treine, ajuste e evolua.
