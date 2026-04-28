# /tech-design-doc

Gera o Tech Design Doc completo para uma iniciativa de growth no AVS 9.3.

## Como usar
```
/tech-design-doc iniciativa="[nome]" objetivo="[objetivo de negócio]" apis="[APIs AVS impactadas]"
```

## Fluxo de execução
Use o agente `orchestrator` para:

1. Receber nome da iniciativa, objetivo e contexto técnico
2. Consultar `tech-architect` para seções técnicas (APIs, NFRs, riscos, rollback)
3. Consultar `data-specialist` para seção de dados e instrumentação
4. Consultar `growth-scientist` para contexto de negócio e critérios de sucesso
5. Aplicar gates 1, 2 e 3 obrigatoriamente
6. Solicitar aprovação humana antes de finalizar
7. Gerar TDD com seções fixas:

## Estrutura do TDD
```
# Tech Design Doc — [Iniciativa] v1.0
## 1. Visão Geral
## 2. Objetivo de Negócio e KPIs
## 3. Solução Técnica Proposta
## 4. APIs AVS 9.3 Impactadas
## 5. Modelo de Dados (sem PII)
## 6. Fluxo de Integração
## 7. NFRs e Observabilidade
## 8. Plano de Dados e Instrumentação
## 9. Riscos e Mitigações
## 10. Plano de Rollback
## 11. Estimativa de Esforço
## 12. Critérios de Aceite Técnicos
## Apêndice: Quality Gates Checklist
```

## Output esperado
Arquivo: `tdd-[iniciativa]-v1.0.md`
