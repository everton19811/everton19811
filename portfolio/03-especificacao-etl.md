# Dicionário de KPIs

| KPI | Fórmula | Frequência | Dono | Meta |
|---|---|---|---|---|
| **PV** — Planned Value | Custo orçado do trabalho planejado até a data | Semanal | PM | — |
| **EV** — Earned Value | % concluído × BAC da tarefa | Semanal | PM | — |
| **AC** — Actual Cost | Custo real apropriado | Semanal | Financeiro | — |
| **CV** — Cost Variance | EV − AC | Semanal | PMO | ≥ 0 |
| **SV** — Schedule Variance | EV − PV | Semanal | PMO | ≥ 0 |
| **CPI** — Cost Perf. Index | EV / AC | Semanal | PMO | ≥ 0,95 |
| **SPI** — Schedule Perf. Index | EV / PV | Semanal | PMO | ≥ 0,95 |
| **EAC** | BAC / CPI | Semanal | PMO | ≤ BAC×1,05 |
| **ETC** | EAC − AC | Semanal | PMO | — |
| **VAC** | BAC − EAC | Semanal | PMO | ≥ 0 |
| **TCPI** | (BAC − EV) / (BAC − AC) | Semanal | PMO | ≤ 1,1 |

## Semáforo RAG
- 🟢 Verde: CPI e SPI ≥ 0,95
- 🟡 Amarelo: 0,85 ≤ CPI ou SPI < 0,95
- 🔴 Vermelho: CPI ou SPI < 0,85
