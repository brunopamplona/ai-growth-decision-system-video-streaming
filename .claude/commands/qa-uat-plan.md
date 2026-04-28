# /qa-uat-plan

Gera o Plano de QA/UAT completo para uma iniciativa de growth no AVS 9.3.

## Como usar
```
/qa-uat-plan iniciativa="[nome]" historias="[STORY-XXX, STORY-YYY]" ambiente="[staging|homologação]"
```

## Fluxo de execução
Use o agente `orchestrator` para:

1. Receber iniciativa, histórias incluídas no escopo e ambiente de teste
2. Consultar `tech-architect` para cenários de teste técnicos e NFRs a validar
3. Consultar `data-specialist` para dados de teste sintéticos (sem PII de produção)
4. Consultar `growth-scientist` para cenários de negócio e critérios de aceite funcionais
5. Aplicar Gates 1, 2 e 5 obrigatoriamente
6. Solicitar aprovação humana
7. Gerar plano completo com:

## Estrutura do Plano QA/UAT
```
# Plano QA/UAT — [Iniciativa] v1.0

## 1. Escopo
   - Histórias incluídas
   - Histórias excluídas (out of scope)
   - Ambientes de teste

## 2. Cenários Críticos (Happy Path)
   | ID  | Cenário | Pré-condição | Passos | Resultado Esperado | Evidência |

## 3. Cenários de Erro e Edge Cases
   | ID  | Cenário | Comportamento Esperado |

## 4. Testes de Performance/NFR
   - Testes de carga nos endpoints AVS afetados
   - Thresholds de latência e disponibilidade

## 5. Dados de Teste
   - Perfis de usuário sintéticos necessários
   - Estados de conta para cobrir cenários
   - ZERO uso de dados reais de produção

## 6. Critérios de Aceite de QA (DoD)
   - Cobertura mínima de testes automatizados
   - Aprovação de testes de regressão
   - Sign-off dos critérios de aceite das histórias

## 7. Plano de UAT
   - Usuários de teste (internos, beta)
   - Roteiro de validação
   - Formulário de feedback estruturado

## 8. Evidências Obrigatórias
   - Screenshots / gravações dos cenários críticos
   - Resultados dos testes de performance
   - Relatório de bugs encontrados e resolvidos
```

## Output esperado
Arquivo: `qa-uat-[iniciativa]-v1.0.md`
