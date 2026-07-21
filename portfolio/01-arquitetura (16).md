# Dicionário de KPIs Ágeis

| KPI | Definição | Fórmula | Meta |
|---|---|---|---|
| **Lead Time** | Da criação ao done | data_done − data_created (dias úteis) | ↓ tendência |
| **Cycle Time** | Do "In Progress" ao done | data_done − data_in_progress | ↓ tendência |
| **Throughput** | Itens concluídos por sprint | count(done) por sprint | ↑ tendência |
| **WIP** | Itens em progresso | count(status ∈ EmAndamento) | ≤ 2/pessoa |
| **CFD** | Área acumulada por status | count por status por dia | — |
| **Burnup** | Escopo × concluído por sprint | soma pontos | Concluído ≤ Escopo |
| **% Bugs** | Bugs / total | bugs / itens_concluídos | ≤ 15% |
| **SLA P1** | Incidentes P1 no prazo | on_time / total_P1 | ≥ 95% |
| **MTTR P1** | Tempo médio de resolução | avg(resolved − created) | ↓ tendência |
| **Retrabalho** | Reabertos / total | reopened / done | ≤ 10% |

## Semáforo
- 🟢 Meta atendida
- 🟡 Até 10% abaixo
- 🔴 Mais de 10% abaixo
