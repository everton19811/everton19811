# Arquitetura de Dados

## Fluxo
Azure DevOps (WBS, apontamentos) → API REST → SSIS (staging) → SQL Server (DW dimensional) → Power BI Dataset → Relatórios + Power Automate.

## Modelo dimensional
- **Fato_EVM** (ProjetoID, DataID, PV, EV, AC, BAC)
- **Dim_Projeto** (ProjetoID, Nome, Sponsor, Programa, Status)
- **Dim_Tempo** (DataID, Semana, Mês, Trimestre)
- **Dim_WBS** (WBSID, Nível1..4, Pacote)

## Cargas
- Batch semanal domingo 22:00 (full refresh do fato)
- Incremental para logs de apontamento (diário)
