# Algebra Visualizer

Visualizador interativo de **álgebra abstrata** na web: tabelas e grafos de Cayley, reticulados de subgrupos, classes laterais e simetrias de polígonos.

Os cálculos são feitos pelo [Mini CAS](https://github.com/daniel-fbo/mini-cas), compilado para WebAssembly e executado num Web Worker, para a interface nunca travar.

> 🚧 Em fase inicial: por enquanto o repositório contém apenas a estrutura planejada.

## Visualizações previstas

- Tabela de Cayley, com destaque de subgrupos e classes laterais
- Grafo de Cayley a partir dos geradores
- Reticulado de subgrupos
- Simetrias de polígonos regulares (grupos diedrais)

## Estrutura

```
src/
├── engine/      # ponte com o CAS (Worker + WASM) e motor falso para desenvolvimento
├── models/      # tipos do domínio e do contrato JSON
├── views/       # visualizações
├── components/  # componentes de interface
├── state/       # estado global
├── hooks/       # lógica reutilizável
└── utils/       # layouts, paletas de cor, exportação SVG
```

## Stack

`TypeScript` · `React` · `Vite` · `Zustand` · `SVG` · `Web Workers` · `WebAssembly` · `Vitest`
