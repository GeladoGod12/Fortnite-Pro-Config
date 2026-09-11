# Fortnite Pro Config Hub 2026

Hub competitivo de Fortnite em uma única página HTML: configurações de **controle**, **teclado + mouse** e **mobile**, rotinas de treino, códigos de mapas Creative, vídeos de piece control, builds dos tops e gravação de tela.

**Atualizado · Setembro 2026**

---

## Demonstração

Abra o arquivo `index.html` no navegador (Chrome, Edge ou Firefox recomendados).

Não precisa de build, servidor Node nem dependências — é HTML, CSS e JavaScript puro.

---

## Funcionalidades

### Configurações competitivas
| Plataforma | Conteúdo |
|---|---|
| **Controle** | Builder Pro, sensibilidade avançada (Exponential), deadzone, multiplicadores de build/edit, aim assist |
| **Teclado + Mouse** | DPI 800, eDPI, sensibilidade, keybinds (mouse buttons, edit, reset) |
| **Mobile** | Gráficos, look/ADS/scope, turbo building |
| **Vídeo** | Performance Mode, 1080p, NVIDIA Reflex, sombras/AA off |

### Treinos
- **30 min** — aquecimento (aim, piece control, box 2v2)
- **1 hora** — sessão completa
- **2 horas** — evolução + VOD review

### Mapas Creative
Clique no código para copiar:
- **MECÂNICA PRO V4** — `9235-0277-4070`
- Piece Control 2v2, Piece Moving Bots, PANDVIL e outros

### Vídeos de truques
Tutoriais embutidos do YouTube (piece control, edits, mecânicas de pro).

### Tops do mundo
Cards com estilo e settings de **Sky**, **Malibuca** e **Peterbot** (incluindo binds e sens públicas).

### Ferramentas
- **Gravar tela** — API nativa do navegador (`getDisplayMedia` + `MediaRecorder`) → download `.webm`
- **Print / Screenshot** — dicas por sistema operacional
- **Imprimir página** — versão limpa para PDF
- **Modal de dicas** — atalhos e uso rápido

---

## Como usar

### 1. Abrir o app
1. Baixe ou clone o repositório.
2. Abra `index.html` com duplo clique ou arraste para o navegador.
3. (Opcional) Sirva com um servidor local para HTTPS/recursos restritos:

```bash
# Python 3
python -m http.server 8080

# Node (npx)
npx serve .
```

Acesse: `http://localhost:8080`

### 2. Navegar
Use o menu sticky no topo:
**Controle · Teclado + Mouse · Mobile · Vídeo · Treinos · Mapas · Vídeos Truques · Top 3 Builds**

### 3. Aplicar configs
1. Escolha sua plataforma (controle / KBM / mobile).
2. Ative **Opções Avançadas** no Fortnite quando indicado.
3. Copie os valores (sens, binds, vídeo).
4. Ajuste ao conforto — consistência > cópia cega.

### 4. Treinar
1. Vá em **Treinos** e escolha 30 min, 1 h ou 2 h.
2. Copie o código do mapa em **Mapas** (clique no código).
3. Cole no Creative (Descobrir) e siga a rotina.

### 5. Gravar a tela
1. Clique em **Gravar Tela**.
2. Escolha a janela/aba/tela e confirme o compartilhamento.
3. Treine ou jogue.
4. **Parar & Baixar** gera um arquivo `.webm`.

> Funciona melhor em Chrome, Edge ou Firefox atualizado. Pode exigir HTTPS ou `localhost`.

### 6. Imprimir / salvar PDF
Use **Imprimir Página** (ou `Ctrl+P` / `Cmd+P`) e escolha “Salvar como PDF”. A navegação e os botões de ferramenta somem na versão impressa.

---

## Estrutura do projeto

```text
.
├── index.html    # App completo (HTML + CSS + JS)
└── README.md     # Este arquivo
```

Tudo está em um único arquivo para facilitar o uso e o deploy estático.

---

## Tecnologias

- HTML5
- CSS3 (variáveis, grid, sticky nav, responsivo)
- JavaScript (vanilla)
  - Navegação e abas
  - Cópia de códigos de mapa (`clipboard` API)
  - Gravação de tela (`getDisplayMedia`, `MediaRecorder`)
  - Modais e observer de seções

**Sem frameworks, sem npm, sem build.**

---

## Compatibilidade

| Recurso | Suporte |
|---|---|
| Layout e configs | Todos os navegadores modernos |
| Copiar código de mapa | Chrome, Edge, Firefox, Safari |
| Gravação de tela | Chrome, Edge, Firefox (permissão do usuário) |
| Impressão / PDF | Todos |

Mobile: layout responsivo; gravação de tela depende do suporte do navegador no dispositivo.

---

## Deploy

Qualquer host estático serve:

- **GitHub Pages** — ative Pages na branch com `index.html` na raiz
- **Netlify / Vercel / Cloudflare Pages** — arraste a pasta ou conecte o repo
- **itch.io / itch** — upload como HTML

Exemplo GitHub Pages:
1. Repo público com `index.html` na raiz (ou em `/docs`).
2. Settings → Pages → Source: branch `main` / pasta `/`.
3. Acesse `https://SEU_USUARIO.github.io/NOME_DO_REPO/`.

---

## Fontes dos dados

Configurações e referências baseadas em dados públicos de:

- Power Rankings e resultados competitivos (2026)
- Settings divulgados por pros (ex.: Peterbot)
- Guias e agregadores (ProSettings, setup.gg e similares)
- Mapas Creative da comunidade

Valores são **pontos de partida**. Sensibilidade e binds devem ser adaptados ao hardware e à preferência pessoal.

---

## Avisos

- Este projeto **não é afiliado** à Epic Games.
- Fortnite é marca da Epic Games, Inc.
- Códigos de mapa e settings de jogadores podem mudar; confira sempre no jogo.
- A gravação de tela grava o que o navegador compartilhar — respeite privacidade e termos de uso das plataformas.

---

## Contribuindo

Sugestões e correções são bem-vindas:

1. Fork do repositório
2. Branch (`git checkout -b feature/melhoria`)
3. Commit claro
4. Pull request

Ideias úteis: novos mapas, settings atualizados de pros, traduções, melhorias de acessibilidade.

---

## Licença

Uso livre para fins educacionais e da comunidade competitiva.  
Não redistribua como produto pago sem permissão do autor do repositório.

---

## Créditos

Feito para a comunidade competitiva de Fortnite.  
Consistência > cópia cega. Treine, ajuste e evolua.
