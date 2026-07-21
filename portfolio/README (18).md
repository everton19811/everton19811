# Modelo dbt — principais transformações

## mart_lead_time
```sql
SELECT
  issue_key, squad, tipo,
  DATE_DIFF(done_at, created_at, DAY) AS lead_time_days
FROM {{ ref('int_issue_transitions') }}
WHERE status_final = 'Done'
```

## mart_cfd
Uma linha por (data, squad, status) com contagem cumulativa.

## Testes
- not_null em issue_key, squad
- accepted_values para status (5 valores)
- relationships issue → squad
