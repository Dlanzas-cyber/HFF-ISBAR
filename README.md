# HFF-ISBAR

**Ferramenta de suporte à passagem de turno em enfermagem** baseada na metodologia ISBAR.  
Desenvolvida para o Hospital Prof. Doutor Fernando Fonseca (HFF).

---

## O que é?

Aplicação web progressiva (PWA) que orienta os enfermeiros na estruturação da passagem de turno segundo as 5 componentes do ISBAR:

| Letra | Componente | Descrição rápida |
|-------|-----------|-----------------|
| **I** | Identificação | Quem é o doente e quem comunica |
| **S** | Situação | Estado clínico atual |
| **B** | Background | Contexto e antecedentes relevantes |
| **A** | Avaliação | Dados clínicos e interpretação |
| **R** | Recomendações | Próximas ações e pendências |

---

## Estrutura de ficheiros

```
hff-isbar/
├── index.html        ← Aplicação completa (HTML + CSS + JS)
├── manifest.json     ← Manifesto PWA (instalação no telemóvel)
├── sw.js             ← Service Worker (modo offline)
├── icons/
│   ├── icon-192.png  ← Ícone para Android / Chrome
│   └── icon-512.png  ← Ícone splash screen
└── README.md
```

---

## Publicar no GitHub Pages

### 1. Criar repositório

```bash
# Criar novo repositório no GitHub (ex: hff-isbar)
# Depois clonar e copiar os ficheiros
git clone https://github.com/SEU_USERNAME/hff-isbar.git
cp -r * hff-isbar/
cd hff-isbar
git add .
git commit -m "Initial commit — HFF-ISBAR PWA"
git push origin main
```

### 2. Ativar GitHub Pages

1. Aceder ao repositório no GitHub  
2. **Settings** → **Pages**  
3. Em *Source*, selecionar **Deploy from a branch**  
4. Branch: `main` / Folder: `/ (root)`  
5. Clicar **Save**

Após alguns minutos a app estará disponível em:  
`https://SEU_USERNAME.github.io/hff-isbar/`

---

## Instalar no telemóvel

### Android (Chrome)
1. Abrir a URL da app no Chrome  
2. Aparece automaticamente um banner **"Instalar HFF-ISBAR"**  
3. Tocar em **Instalar** → A app aparece no ecrã inicial  

### iPhone / iPad (Safari)
1. Abrir a URL no Safari  
2. Tocar no botão **Partilhar** (ícone de caixa com seta para cima)  
3. Selecionar **"Adicionar ao Ecrã de Início"**  
4. Confirmar com **Adicionar**  

A app funciona **offline** após a primeira visita.

---

## Tecnologias

- HTML5 + CSS3 + JavaScript vanilla (sem dependências)
- Progressive Web App (PWA) com Service Worker
- Cache-first com atualização em background
- Suporte a safe-area (notch) em iOS
- Fontes: [Sora](https://fonts.google.com/specimen/Sora) + [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono)

---

## Licença

Uso interno — Hospital Prof. Doutor Fernando Fonseca, EPE.
