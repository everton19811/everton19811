# Project Charter

| Campo | Conteúdo |
|---|---|
| **Projeto** | Dashboard EVM Portfólio PMO |
| **Sponsor** | Diretor de PMO |
| **Gerente do Projeto** | Everton |
| **Início / Fim** | Mês 1 / Mês 4 |
| **Orçamento** | R$ 258.000 |

## Objetivo SMART
Entregar em 4 meses um dashboard Power BI que calcule PV, EV, AC, CPI, SPI, EAC, ETC e VAC dos 24 projetos ativos do PMO, com atualização semanal automática e Status Report gerado via Power Automate.

## Escopo (alto nível)
- Modelagem de baselines de custo e prazo no Azure DevOps
- Pipeline de dados semanal (SQL Server)
- Dashboard Power BI com 5 páginas (Portfólio, Projeto, EVM, Riscos, Financeiro)
- Status Report automatizado em PDF/PowerPoint

## Fora do escopo
- Substituir o Azure DevOps como sistema fonte
- Integração com SAP financeiro (fase 2)

## Premissas / Restrições
- Todos os projetos precisam ter WBS carregada no Azure DevOps
- Licenças Power BI Pro para 30 usuários já disponíveis
- Prazo fixo: entrega antes do fechamento do trimestre
