---
name: homelab-backup
description: Planejar, verificar e testar backup e restauração de dados e serviços do homelab. Use para definir cobertura, avaliar backups existentes ou conduzir restauração autorizada.
---

Identifique dados persistentes, configurações, dependências e o mecanismo atual de backup. Levante tolerância a perda de dados e tempo de recuperação quando isso afetar a estratégia. Não confunda snapshots, replicação e cópias independentes.

Mapeie por serviço: origem, destino, frequência, retenção, criptografia, referência às credenciais, consistência dos dados e procedimento de restauração. Para bancos e aplicações em escrita, use um método de backup compatível com a aplicação; cópia de arquivos abertos pode ser inconsistente.

Verifique execução recente, erros, cobertura e acesso ao material necessário à recuperação. Existência ou checksum de um arquivo não prova recuperação funcional.

Teste restauração em destino isolado autorizado, sem sobrescrever dados ativos. Evite colisões de portas, nomes, tarefas agendadas e integrações que poderiam enviar mensagens ou modificar sistemas reais. Valide integridade e leitura pela aplicação e registre duração e ponto recuperado.

Restauração em produção, exclusão de cópias e mudanças de retenção exigem escopo explícito no pedido. Não apague o ambiente de teste sem observar a autorização e os dados produzidos. Entregue evidências do teste e lacunas que ainda impeçam recuperar o serviço.
