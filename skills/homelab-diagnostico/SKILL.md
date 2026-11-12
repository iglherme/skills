---
name: homelab-diagnostico
description: Diagnosticar indisponibilidade, lentidão e erros em serviços do homelab. Use para investigar incidentes com logs, métricas e configuração, antes de escolher uma correção.
---

Identifique sintoma, início aproximado, componentes afetados e mudanças recentes. Consulte inventário e runbooks existentes; mantenha fatos separados de hipóteses.

Comece com observações de baixo impacto nos alvos autorizados. Siga as dependências relevantes: resolução de nomes, conectividade, TLS/proxy, processo ou container, recursos, armazenamento e serviços externos. Escolha cada consulta pela hipótese que ela pode confirmar ou descartar; limite períodos e volume de logs e oculte credenciais.

Não use reinício, limpeza de volumes, desativação de controles ou alteração de firewall como teste inicial. Quando uma correção for necessária, indique a evidência, o efeito esperado, o alcance e como reverter; execute somente dentro da autorização existente.

Após corrigir, verifique saúde técnica e uma operação que represente o uso real do serviço. Registre causa confirmada ou hipótese restante, ações, resultado e prevenção pertinente. Se não houver acesso, forneça comandos específicos ao ambiente identificado e peça as saídas mínimas necessárias.
