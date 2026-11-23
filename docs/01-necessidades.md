# 1. Levantamento de necessidades

## Organização e contexto

O Centro Administrativo Pantanal é uma organização **fictícia** de Cuiabá/MT, com 35 colaboradores distribuídos entre administração, atendimento, financeiro, gestão e TI. Considera-se um modelo híbrido no qual parte da equipe trabalha de casa em alguns dias da semana.

## Problemas identificados no cenário hipotético

- Documentos ficam em computadores locais, dificultando o compartilhamento e o controle de versões.
- Acesso remoto a sistemas internos depende de procedimentos improvisados.
- Solicitações e decisões circulam em canais diferentes e se perdem.
- Não há padrão documentado de autenticação, backup e atendimento de incidentes.
- Pessoas com diferentes dispositivos e condições de conectividade precisam realizar as mesmas tarefas.

## Requisitos funcionais

| ID | Requisito | Prioridade |
|---|---|---|
| RF01 | Acessar arquivos compartilhados com permissões por equipe | Alta |
| RF02 | Realizar reuniões e troca de mensagens corporativas | Alta |
| RF03 | Acessar aplicações internas por canal remoto protegido | Alta |
| RF04 | Registrar solicitações de suporte e acompanhar resolução | Média |
| RF05 | Recuperar versões e arquivos conforme política de retenção | Alta |

## Requisitos não funcionais

| ID | Requisito | Critério proposto |
|---|---|---|
| RNF01 | Segurança | MFA, privilégio mínimo e registros de acesso |
| RNF02 | Usabilidade | Fluxos principais concluídos em testes com usuários |
| RNF03 | Acessibilidade | Avaliação orientada pelas WCAG 2.2 nível AA |
| RNF04 | Continuidade | Backups testados e plano de contingência |
| RNF05 | Conectividade | Documentos leves e alternativas assíncronas |

## Validação necessária

Antes da contratação, entrevistas com representantes de cada setor deverão confirmar volumes de dados, sistemas legados, horários de atendimento, orçamento e exigências legais. O levantamento aqui apresentado é uma simulação de planejamento.
