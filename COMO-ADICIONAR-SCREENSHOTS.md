# 📸 Guia: Como Adicionar Screenshots ao Showcase

## 🎯 Objetivo

Substituir os placeholders por screenshots reais da aplicação para tornar o showcase mais impactante.

---

## 🛠️ Ferramentas Recomendadas

### Para Screenshots Estáticas

**Windows:**
- `Win + Shift + S` - Screenshot nativo
- [ShareX](https://getsharex.com/) - Editor completo (gratuíto)

**Mac:**
- `Cmd + Shift + 4` - Screenshot de área
- [CleanShot X](https://cleanshot.com/) - Editor profissional

**Linux (Pop!_OS):**
- `Print Screen` ou `Shift + Print Screen`
- [Flameshot](https://flameshot.org/) - Screenshot + anotações

### Para GIFs Animados

**Windows:**
- [ScreenToGif](https://www.screentogif.com/) - Melhor opção gratuita

**Mac:**
- [Kap](https://getkap.co/) - Open-source e leve

**Linux:**
- [Peek](https://github.com/phw/peek) - Simples e eficiente

**Todas as plataformas:**
- [LICEcap](https://www.cockos.com/licecap/) - Leve e multi-plataforma

---

## 📜 Screenshots Necessárias

### 1. Banner Hero (1200x300px)
**Arquivo:** `banner.png`

**O que capturar:**
- Use uma ferramenta de design (Figma/Canva)
- Ou screenshot do dashboard com overlay de título
- Cores: Roxo (#6366f1) + branco

**Dica:** Use [Canva](https://canva.com) com template "GitHub Banner"

### 2. Dashboard Principal (800x450px)
**Arquivo:** `dashboard.png`

**O que capturar:**
1. Acesse [https://financas-faceis-ochre.vercel.app/](https://financas-faceis-ochre.vercel.app/)
2. Faça login com usuário teste
3. Capture a visão geral com:
   - Gráficos visíveis
   - Cards de métricas
   - Menu lateral
   - Header

**Tamanho de janela:** 1600x900px (depois redimensionar)

### 3. Controle de Gastos (800x450px)
**Arquivo:** `gastos.png`

**O que capturar:**
- Lista de transações
- Filtros visíveis
- Botão de adicionar

### 4. Gestão de Cartões (800x450px)
**Arquivo:** `cartoes.png`

**O que capturar:**
- Cards de cartões
- Faturas pendentes
- Limites

### 5. Metas Financeiras (800x450px)
**Arquivo:** `metas.png`

**O que capturar:**
- Lista de metas
- Barra de progresso
- Valores

### 6. Relatórios (800x450px)
**Arquivo:** `relatorios.png`

**O que capturar:**
- Gráficos interativos
- Comparações
- Período selecionado

### 7. Versão Mobile (375x667px)
**Arquivo:** `mobile.png`

**Como capturar:**
1. Abra DevTools (F12)
2. Ative modo mobile (Ctrl + Shift + M)
3. Selecione iPhone 12 Pro
4. Capture a tela

---

## 🎬 GIFs de Demonstração

### 1. Cadastro de Transação (5-10 segundos)
**Arquivo:** `cadastro-transacao.gif`

**O que gravar:**
1. Clique em "Adicionar Gasto"
2. Preencha formulário
3. Salve
4. Mostre item aparecendo na lista

**Configurações:**
- FPS: 15-20
- Duração: 5-8 segundos
- Loop: Sim

### 2. Navegação pelo Dashboard (8-12 segundos)
**Arquivo:** `navegacao.gif`

**O que gravar:**
1. Scroll pelo dashboard
2. Clique em um card
3. Visualize detalhes
4. Volte

### 3. Interação com Gráficos (5-8 segundos)
**Arquivo:** `dashboard-interativo.gif`

**O que gravar:**
1. Hover sobre gráficos
2. Mostre tooltips
3. Alterne entre abas

---

## 💾 Otimização de Arquivos

### Para PNGs

**Online:**
- [TinyPNG](https://tinypng.com/) - Comprime sem perder qualidade

**CLI:**
```bash
# Instalar
npm install -g pngquant

# Comprimir
pngquant dashboard.png --quality 65-80 --output dashboard-compressed.png
```

### Para GIFs

**Online:**
- [ezgif.com](https://ezgif.com/optimize) - Otimizador de GIFs

**Dicas:**
- Reduza FPS para 12-15
- Limite duração a 10 segundos
- Tamanho máximo: 5MB por GIF

---

## 📝 Como Adicionar ao Repositório

### Método 1: Via GitHub Web

1. Acesse: [https://github.com/edlucaz/financas-faceis-showcase/tree/main/.github/SCREENSHOTS](https://github.com/edlucaz/financas-faceis-showcase/tree/main/.github/SCREENSHOTS)
2. Clique em "Add file" > "Upload files"
3. Arraste suas imagens
4. Commit com mensagem: `docs: adiciona screenshots do projeto`

### Método 2: Via Git CLI

```bash
# Clone o repositório
git clone https://github.com/edlucaz/financas-faceis-showcase.git
cd financas-faceis-showcase

# Adicione os arquivos
cp ~/Downloads/dashboard.png .github/SCREENSHOTS/
cp ~/Downloads/gastos.png .github/SCREENSHOTS/
# ... outros arquivos

# Commit e push
git add .github/SCREENSHOTS/
git commit -m "docs: adiciona screenshots do projeto"
git push origin main
```

### Método 3: Drag & Drop no README

1. Edite o README.md diretamente no GitHub
2. Arraste a imagem para o editor
3. GitHub fará upload automático
4. Substitua o placeholder pela URL gerada

---

## ✏️ Atualizar o README

Depois de fazer upload, edite o `README.md` e substitua:

**Era:**
```markdown
![Banner](https://via.placeholder.com/1200x300/6366f1/ffffff?text=Finan%C3%A7as+F%C3%A1ceis)
```

**Fica:**
```markdown
![Banner](/.github/SCREENSHOTS/banner.png)
```

Faça isso para todos os placeholders:
- Banner hero
- Dashboard screenshot
- Adicione mais screenshots conforme necessário

---

## ✨ Dicas de Qualidade

### Para Screenshots

✅ Use tema claro ou escuro consistente  
✅ Esconda dados sensíveis (use dados fake)  
✅ Mostre interface completa (sem partes cortadas)  
✅ Resolução mínima: 1600x900px  
✅ Formato: PNG (melhor qualidade)  

### Para GIFs

✅ Movimentos suaves (não muito rápidos)  
✅ Foco em UMA ação por vez  
✅ Loop infinito  
✅ Tamanho máximo: 5MB  
✅ FPS: 12-15 (equilibra tamanho e fluidez)  

---

## 📊 Checklist Final

- [ ] Banner hero (1200x300px)
- [ ] Dashboard principal (800x450px)
- [ ] Tela de gastos
- [ ] Tela de cartões
- [ ] Tela de metas
- [ ] Tela de relatórios
- [ ] Versão mobile
- [ ] GIF: Cadastro de transação
- [ ] GIF: Navegação
- [ ] GIF: Gráficos interativos
- [ ] Atualizar README.md com URLs reais
- [ ] Verificar se todas as imagens carregam

---

## ❓ Dúvidas?

Se precisar de ajuda, me chame! 🚀
