# Especificação de ETL

## Origens
- Azure DevOps: Work Items, Iterations, Task Board
- SharePoint List: Baselines de custo por projeto
- SAP export CSV: Custo real (AC) semanal

## Transformações
- Reconciliação de código de projeto (chave surrogate)
- Cálculo de % concluído por Work Item (regra ponderada por Story Points)
- Cálculo de EV via SP `usp_CalcularEVM`
- Snapshot semanal do Fato_EVM (Slowly Changing Dimension Tipo 2)

## Qualidade
- 12 regras DQ (nulos, integridade referencial, faixa CPI 0-2)
- Log de exceções em `dq_log`
