# /quarterly-roadmap

Gera o Roadmap Trimestral completo para o Growth Team AVS 9.3.

## Como usar
```
/quarterly-roadmap quarter="Q3 2025" objetivo="Aumentar D30 retention de 35% para 45%" contexto="[contexto adicional opcional]"
```

## Fluxo de execução
Use o agente `orchestrator` para:

1. Receber os parâmetros: quarter, objetivo de negócio, contexto adicional
2. Consultar `data-specialist` para baseline de métricas do quarter anterior
3. Consultar `growth-scientist` para priorização RICE e OKRs
4. Consultar `tech-architect` para validar viabilidade das top 5 iniciativas
5. Aplicar os 5 quality gates obrigatórios
6. Solicitar aprovação humana
7. Gerar entregável final com:
   - Resumo executivo (1-pager)
   - OKRs do quarter
   - Backlog priorizado por RICE (top 10)
   - Mapa de dependências
   - Riscos e mitigações

## Output esperado
Arquivo: `roadmap-Q[X]-[YYYY]-v1.0.md`
