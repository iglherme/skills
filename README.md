# Skills para projetos pessoais e homelab

Coleção de instruções reutilizáveis para transformar pedidos do dia a dia em trabalho verificável. As skills não dependem de uma stack específica: usam as ferramentas, os arquivos e as convenções do projeto em questão.

## Catálogo

| Skill | Quando usar | Exemplo de pedido |
| --- | --- | --- |
| [planejar-projeto](skills/planejar-projeto/SKILL.md) | Tirar uma ideia do papel e escolher a próxima entrega | “Organize um MVP do meu painel do homelab para trabalhar nos fins de semana.” |
| [implementar-tarefa](skills/implementar-tarefa/SKILL.md) | Desenvolver funcionalidades e corrigir bugs | “Corrija a expiração da sessão e valide o comportamento.” |
| [revisar-alteracoes](skills/revisar-alteracoes/SKILL.md) | Revisar mudanças antes de integrar ou entregar | “Revise este diff procurando regressões e problemas na migração.” |
| [homelab-inventario](skills/homelab-inventario/SKILL.md) | Documentar serviços e dependências | “Mapeie os serviços a partir destes arquivos Compose e liste o que falta documentar.” |
| [homelab-diagnostico](skills/homelab-diagnostico/SKILL.md) | Investigar falhas e lentidão | “O serviço retorna 502; investigue os logs e a cadeia de dependências.” |
| [homelab-mudanca](skills/homelab-mudanca/SKILL.md) | Preparar atualizações e mudanças com reversão | “Prepare a atualização deste serviço, valide a configuração e descreva a reversão.” |
| [homelab-backup](skills/homelab-backup/SKILL.md) | Verificar cobertura e recuperação de dados | “Confira se consigo recuperar este serviço e prepare um teste de restauração isolado.” |
| [retomar-trabalho](skills/retomar-trabalho/SKILL.md) | Preservar contexto entre sessões | “Registre onde paramos e os próximos passos para o fim de semana.” |
| [pesquisar-tecnologia](skills/pesquisar-tecnologia/SKILL.md) | Comparar opções com evidências | “Compare estas ferramentas de monitoramento considerando meu ambiente.” |
| [diagnosticar-bug](skills/diagnosticar-bug/SKILL.md) | Investigar defeitos difíceis no código | “Encontre a causa desta regressão de desempenho com um caso mínimo.” |
| [prototipar-ideia](skills/prototipar-ideia/SKILL.md) | Explorar uma ideia antes de implementá-la | “Monte um experimento para validar os estados deste fluxo.” |
| [registrar-decisoes](skills/registrar-decisoes/SKILL.md) | Registrar escolhas duráveis e esclarecer termos | “Documente por que escolhemos esta solução e suas consequências.” |
| [entrevistar-ideia](skills/entrevistar-ideia/SKILL.md) | Questionar premissas e amadurecer decisões | “Faça um grill-me desta ideia de projeto; depois registre as decisões.” |


## Por onde começar

Para o homelab, comece pelo inventário e pelo backup: eles tornam diagnósticos e mudanças mais informados. Para projetos pessoais, comece pelo planejamento e pela implementação. Use revisão quando houver uma mudança concreta para avaliar.

Um fluxo possível é: planejar uma entrega → implementar → revisar → preparar a mudança no homelab → verificar o serviço e atualizar a documentação. Em um incidente, comece pelo diagnóstico; acione uma mudança somente quando houver uma correção justificada.

## Como usar

Cada pasta em `skills/` é uma skill independente, com nome e descrição no cabeçalho de `SKILL.md` e instruções no corpo. Para usar sem instalar, peça explicitamente ao agente que leia o arquivo, por exemplo:

> Leia `skills/homelab-diagnostico/SKILL.md` e use essas instruções para investigar este erro, considerando os arquivos e logs que forneci.

Para adicionar à sua coleção de skills, solicite à skill `skill-installer` a instalação da pasta desejada deste repositório. Esta preparação não instala nem ativa as skills no ambiente do usuário.

As skills orientam o agente; não fornecem acesso a servidores, credenciais ou integrações. Informe o projeto ou ambiente alvo e o resultado desejado. A execução usa as permissões e autorizações da sessão.

## Personalização

### Uso na rotina do Codex

A preferência global para consultar esta coleção está em [docs/global-AGENTS.md](docs/global-AGENTS.md). Seu conteúdo pode ser incorporado ao `AGENTS.md` do diretório de configuração do Codex (normalmente `~/.codex/AGENTS.md`), preservando instruções já existentes. Um `AGENTS.override.md` global tem precedência sobre esse arquivo.

Essa regra orienta o agente a consultar o catálogo ao iniciar tarefas, carregar apenas as skills pertinentes e anunciar seu uso. Etapas opcionais, como uma entrevista crítica, são sugeridas conforme o contexto. Você pode continuar escrevendo pedidos normalmente, sem decorar os nomes das skills.

O caminho absoluto registrado corresponde a esta máquina. Em outro ambiente, ajuste o caminho e configure a instrução global novamente. Abra uma nova sessão do Codex após configurar para carregar a orientação persistente. Isso não sincroniza memória entre contas ou dispositivos nem instala as skills como comandos nativos.

Documentação oficial: [instruções globais com AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md).

Mantenha o contexto específico nos repositórios e documentos do seu ambiente: stack, hosts, serviços, comandos de validação, convenções e referências aos segredos. Não versione credenciais. As skills consultam esse contexto sem fixar aqui uma topologia que pode ficar desatualizada.

Adicione uma skill quando houver um fluxo recorrente com decisões próprias. Prefira melhorar uma existente quando o problema for apenas um detalhe do mesmo fluxo. Recursos extras, scripts e referências devem existir apenas quando ajudarem uma tarefa real.

## Validação

Com a skill `skill-creator` disponível localmente, execute seu `scripts/quick_validate.py` para cada pasta em `skills/`. O validador verifica a estrutura; a qualidade das decisões deve ser avaliada em tarefas reais. Mudanças nesta coleção não devem executar ações em infraestrutura durante a validação.
