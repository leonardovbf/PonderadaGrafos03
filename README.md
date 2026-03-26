# Ponderada de Grafos 03: Caverna Submarina Interativa

## Descrição

Visualização interativa de um **sistema de cavernas submarinas** construído com [D3.js v7](https://d3js.org/). O projeto apresenta um ecossistema aquático rico, com criaturas animadas, cenário procedural e navegação livre pelo mapa, servindo como exercício prático de manipulação de grafos visuais, bindagem de dados e interação com SVG.

## Demonstração

Abra o arquivo `cave.html` diretamente no navegador (não requer servidor).

## Funcionalidades

### Mundo e cenário

- Mapa de **7 000 × 5 000 px** dividido em três níveis de profundidade:
  - **Level 1 - Coral Reef** (superfície): corais, algas, luz solar filtrada.
  - **Level 2 - Deep Zone** (zona intermediária): iluminação reduzida, estalactites e estalagmites.
  - **Level 3 - The Abyss** (abismo): bioluminescência, escuridão profunda.
- Paredes rochosas procedurais (teto, piso, prateleiras e pilares).
- Bolhas, plâncton e feixes de luz animados continuamente.

### Criaturas marinhas

Cada criatura é um grupo SVG com gradientes próprios e animações individuais:

| Criatura      | Animação                       |
| ------------- | ------------------------------ |
| Goldfish      | Cauda oscilante                |
| Tropical Fish | Cauda oscilante (várias cores) |
| Shark         | Cauda + barbatana dorsal       |
| Octopus       | Tentáculos ondulantes          |
| Jellyfish     | Pulsação do corpo + tentáculos |
| Turtle        | Nadadeiras batendo             |
| Crab          | Pernas articuladas             |
| Eel           | Corpo serpenteante             |
| Puffer        | Cauda oscilante                |
| Anglerfish    | Lure bioluminescente pulsante  |

Todas as criaturas possuem movimentação autônoma (wander) com velocidade e alcance específicos por espécie.

### Interação

- **Zoom** via scroll do mouse ou botões `+` / `−`.
- **Pan** arrastando o fundo.
- **Drag & drop** de qualquer criatura para reposicioná-la.
- **Fit to screen** para visualizar o mapa inteiro.
- **Minimapa** (canto superior direito) mostrando a posição da viewport e das criaturas em tempo real.

## Tecnologias

- **D3.js v7:** bindagem de dados, criação de SVG, zoom/pan, drag behavior.
- **SVG:** gradientes (radial/linear), filtros (drop-shadow, glow), paths procedurais.
- **Canvas 2D:** renderização do minimapa.
- **HTML/CSS:** layout, backdrop-filter, controles de UI.

## Como executar

```bash
# Clone o repositório
git clone https://github.com/<usuario>/PonderadaGrafos03.git
```

```bash
# Abra no navegador MacOS
open cave.html
```

```bash
# Abra no navegador Linux
xdg-open cave.html
```

```bash
# Abra no navegador Windows
start cave.html
```

## Estrutura do projeto

```
├── cave.html
└── README.md
```

## Autores

Leonardo Fischel
Henrique Barone
