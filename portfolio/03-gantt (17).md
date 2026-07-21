# Arquitetura de Dados

```
Jira Cloud ─┐
            ├─► Fivetran ─► BigQuery (raw) ─► dbt (staging → marts) ─► Looker Studio
ServiceNow ─┘                                                          │
                                                                       └► Alertas Slack (Cloud Functions)
```

## Camadas dbt
- `stg_jira_issues`, `stg_sn_incidents`
- `int_issue_transitions`, `int_incident_sla`
- `mart_lead_time`, `mart_throughput`, `mart_cfd`, `mart_sla`

## Otimizações BigQuery
- Particionamento por `event_date`
- Clustering por `squad, tipo`
