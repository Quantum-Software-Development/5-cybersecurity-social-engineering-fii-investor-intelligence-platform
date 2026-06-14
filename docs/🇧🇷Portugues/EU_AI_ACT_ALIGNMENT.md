# EU AI Act — Alinhamento e Classificação
## Investor Intelligence Platform — FIIs Brasil 🇧🇷

**Regulamento (UE) 2024/1689 do Parlamento Europeu e do Conselho**

---

## Classificação do Sistema

**Categoria de risco: MÍNIMO (Art. 6º — Sistemas não de alto risco)**

| Critério de Alto Risco | Aplicável? | Justificativa |
|---|---|---|
| Infraestrutura crítica | ❌ | Sistema analítico acadêmico |
| Decisões de crédito ou financiamento | ❌ | Não emite decisões de crédito |
| Emprego e gestão de trabalhadores | ❌ | Fora do escopo |
| Serviços públicos essenciais | ❌ | Fora do escopo |
| Aplicação da lei | ❌ | Fora do escopo |
| Migração e controle de fronteiras | ❌ | Fora do escopo |
| Administração da justiça | ❌ | Fora do escopo |
| Biometria e reconhecimento facial | ❌ | Não coletado |

**Classificação final:** Sistema de IA de **risco mínimo** — plataforma analítica e informacional.

---

## Obrigações Aplicáveis a Sistemas de Risco Mínimo

Embora sem obrigações compulsórias para risco mínimo, adotamos voluntariamente boas práticas:

| Prática Voluntária | Implementação |
|---|---|
| Transparência para usuários | Disclaimer em todos os outputs do chatbot |
| Documentação técnica | Este documento + RESPONSIBLE_AI.md + CRISP_DM_MAPPING.md |
| Supervisão humana | Pipeline manual — nenhuma ação autônoma |
| Gestão de qualidade | Quality gates NB02 + logging estruturado |
| Data lineage | `source`, `ingestion_method`, `article_id` preservados |

---

## Disclaimer Obrigatório no Chatbot (Art. 52, EU AI Act)

Todo output do chatbot Groq inclui:

```python
DISCLAIMER = (
    "Esta análise é gerada por IA com base em dados públicos. "
    "Não constitui recomendação de investimento. "
    "Consulte um assessor financeiro certificado antes de tomar decisões."
)
```

---

## Uso Geral vs Uso Específico

**Este sistema NÃO é um GPAI (General Purpose AI Model)** conforme Art. 3(63):
- Não é um modelo de fundação (foundation model)
- Não é distribuído comercialmente para múltiplos propósitos
- É uma pipeline analítica especializada com domínio e propósito definidos

---

## Documentação Técnica (Art. 11 — Voluntária)

| Documento | Localização |
|---|---|
| Descrição do sistema | `README_FINAL.md` |
| Metodologia CRISP-DM | `docs/methodology/CRISP_DM_MAPPING.md` |
| Schema de dados | `docs/architecture/bronze_schema.md` + `silver_schema.md` + `gold_schema.md` |
| Fontes de dados | `docs/data_sources.md` |
| Métricas de qualidade | `data/silver/silver_processing_report.json` |
| Léxico de sentimento | `docs/methodology/SENTIMENT_METHODOLOGY.md` |
| Fundação BM25 | `docs/methodology/BM25_FOUNDATION.md` |
| Alinhamento LGPD | `docs/governance/LGPD_ALIGNMENT.md` |
| IA Responsável | `docs/governance/RESPONSIBLE_AI.md` |

---

*EU AI Act Alignment v1.0.0 · Investor Intelligence Platform FIIs Brasil*
