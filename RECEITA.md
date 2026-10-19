# 🧬 Receita para recriar: Meu projeto

_Gerada sem IA, lendo 6 arquivo(s). Serve para remontar este app como HTML modular — com qualquer IA, um arquivo por vez._

## 1. O que é

- **Nome:** Meu projeto
- **Partes de código:** 5 (3 tela, 1 logica, 0 servidor, 0 dados, 1 estilo)
- **Tem servidor (rotas /api):** não — dá para ser só HTML
- **Peças de fora (bibliotecas):** x

## 2. Estrutura modular proposta

```
index.html            ← a página; chama os módulos NA ORDEM
css/app.css           ← o visual
js/00-core.js         ← a "locomotiva": cria window.APP (registrar, guardar, avisar)
js/10-inicio.js       ← Meu projeto — Olá! 👋 (era index.html)
js/15-laboratorio-projetolens-copia.js← ProjetoLens — Analisador de Projetos — ProjetoLens (era playground/laboratorio-projetolens (cópia).html)
js/20-laboratorio-projetolens.js← ProjetoLens — Analisador de Projetos — ProjetoLens (era playground/laboratorio-projetolens.html)
js/99-app.js          ← o último: monta a tela com o que embarcou
```

## 3. As partes, uma por uma

| # | Era | Vira | Tipo | O que faz | Usa |
|---|---|---|---|---|---|
| 1 | `js/app.js` | css/app.css | logica | Cada módulo cuida de uma coisa só | — |
| 2 | `css/estilo.css` | css/app.css | estilo | — | — |
| 3 | `index.html` | `js/10-inicio.js` | tela | Meu projeto — Olá! 👋 | estilo.css, app.js |
| 4 | `playground/laboratorio-projetolens (cópia).html` | `js/15-laboratorio-projetolens-copia.js` | tela | ProjetoLens — Analisador de Projetos — ProjetoLens | ${url},  |
| 5 | `playground/laboratorio-projetolens.html` | `js/20-laboratorio-projetolens.js` | tela | ProjetoLens — Analisador de Projetos — ProjetoLens | ${url},  |

## 4. Montar passo a passo (cada bloco é um pedido pronto: 📋 Copiar → colar na IA)

### Passo 0 — combinar as regras com a IA

```text
Vamos recriar o app "Meu projeto" como HTML MODULAR, que abre pelo index.html, sem servidor e sem nada da Replit.
Regras: (1) index.html chama os arquivos js/ na ordem, antes do </body>; (2) js/00-core.js cria window.APP com APP.registrar(modulo), APP.guardar(chave, valor) em IndexedDB/localStorage e APP.avisar(texto); (3) cada arquivo js/NN-nome.js cuida de UM assunto, começa com (function (APP) { e termina com })(window.APP); (4) js/99-app.js vem por último e monta a tela com os módulos registrados; (5) textos em português do Brasil.
Vou pedir UM arquivo por vez. Responda só com o arquivo completo, sem cortar nada. Primeiro: crie index.html, css/app.css e js/00-core.js.
```

### Passo 1 — `js/10-inicio.js` (era `index.html`, 19 linhas)

```text
Crie js/10-inicio.js. Ele faz: Meu projeto — Olá! 👋.
Registre com APP.registrar({ nome, icone, abrir }). Devolva só o arquivo completo.
```

### Passo 2 — `js/15-laboratorio-projetolens-copia.js` (era `playground/laboratorio-projetolens (cópia).html`, 11933 linhas)

```text
Crie js/15-laboratorio-projetolens-copia.js. Ele faz: ProjetoLens — Analisador de Projetos — ProjetoLens.
O original usava as bibliotecas x: em HTML puro, use a versão de CDN (ou faça sem ela, se for simples).
Ele chamava estes endereços: https://registry.npmjs.org/${dep.name}/latest, https://registry.npmjs.org/${name}/latest. Em HTML, ligue cada um à função equivalente do módulo certo.
Registre com APP.registrar({ nome, icone, abrir }). Devolva só o arquivo completo.
```

### Passo 3 — `js/20-laboratorio-projetolens.js` (era `playground/laboratorio-projetolens.html`, 11933 linhas)

```text
Crie js/20-laboratorio-projetolens.js. Ele faz: ProjetoLens — Analisador de Projetos — ProjetoLens.
O original usava as bibliotecas x: em HTML puro, use a versão de CDN (ou faça sem ela, se for simples).
Ele chamava estes endereços: https://registry.npmjs.org/${dep.name}/latest, https://registry.npmjs.org/${name}/latest. Em HTML, ligue cada um à função equivalente do módulo certo.
Registre com APP.registrar({ nome, icone, abrir }). Devolva só o arquivo completo.
```

### Passo 4 — `js/99-app.js` e conferir

```text
Crie js/99-app.js: ele olha APP.modulos e monta o menu/abas com um botão para cada módulo. Depois, me mande o index.html atualizado com todos os <script src="js/…"> na ordem certa: js/00-core.js, js/10-inicio.js, js/15-laboratorio-projetolens-copia.js, js/20-laboratorio-projetolens.js, js/99-app.js.
```

## 5. Conferir no final

- [ ] Abrir o index.html na prévia: aparece a tela sem erro (▤ console vazio)?
- [ ] Cada botão abre a sua parte?
- [ ] Fechar e abrir de novo: os dados continuam?
- [ ] Nada com "replit", "REPL_", "@workspace" no código (🏗️ Preparar confere).
- [ ] 📱 PWA → deixar instalável; 📦 APK ou 🖥️ .exe.
