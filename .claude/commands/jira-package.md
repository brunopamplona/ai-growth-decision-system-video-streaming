# /jira-package

Gera o pacote Jira completo (épico → histórias → critérios de aceite → tarefas técnicas).

## Como usar
```
/jira-package iniciativa="[nome do épico]" pilar="[Aquisição|Ativação|Retenção|Receita]" objetivo="[objetivo mensurável]"
```

## Fluxo de execução
Use o agente `orchestrator` para:

1. Receber nome da iniciativa, pilar de growth e objetivo
2. Consultar `growth-scientist` para decomposição em épico + histórias + critérios de aceite
3. Consultar `tech-architect` para tarefas técnicas e estimativas
4. Consultar `data-specialist` para histórias de instrumentação e dados de teste
5. Aplicar Gate 5 (DoR) obrigatoriamente
6. Solicitar aprovação humana
7. Gerar pacote completo no formato:

## Estrutura do Pacote Jira
```
ÉPICO
  └─ HISTÓRIA 1
       ├─ Critérios de Aceite (formato Gherkin: Dado/Quando/Então)
       ├─ Tarefas Técnicas (sub-tasks)
       └─ Definition of Ready checklist
  └─ HISTÓRIA 2 ...
  └─ HISTÓRIA de Instrumentação (sempre incluída)
  └─ HISTÓRIA de QA/UAT
```

## Campos obrigatórios por item
- Story points (estimativa)
- Pilar de growth
- Dependências
- Owner sugerido (agente responsável)
- Link para TDD (se existir)

## Output esperado
Arquivo: `jira-[iniciativa]-v1.0.md`
