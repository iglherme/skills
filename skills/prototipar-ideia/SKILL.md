---
name: prototipar-ideia
description: Construir um experimento descartável para responder uma dúvida de interface, lógica ou modelo de estados. Use para explorar uma ideia antes de implementar a solução definitiva.
---

Declare uma pergunta concreta e o que precisa ser observado para respondê-la. Escolha o menor artefato executável: uma página interativa para estados ou interface, um script para lógica, ou um experimento isolado de persistência quando essa for a dúvida.

Para lógica e estados, exponha estado inicial, ações e transições; inclua um caminho normal e os casos difíceis que motivaram a pergunta. Para interface, compare alternativas que representem decisões reais e descreva o que cada uma explora.

Marque o artefato como protótipo. Use memória ou dados fictícios por padrão e isole qualquer persistência experimental. Reutilize ferramentas existentes quando isso simplificar a execução. Evite dependências, abstrações e acabamento que não ajudem a responder a pergunta.

Mantenha o experimento separado dos caminhos de produção, na convenção existente ou em `prototypes/<assunto>/`. Registre a pergunta, como executar, cenários observados, limitações e conclusão em `result.md` ao lado do artefato. Valide o experimento pelo modo real de uso; para interface, use navegador quando disponível e informe quando não tiver conseguido inspecioná-la.

Exploração não implica promoção automática para produção. Quando a implementação também estiver autorizada, transporte apenas a solução selecionada, com tratamento de erros e validação apropriados. Remova conexões temporárias introduzidas no código definitivo e preserve o trabalho do usuário.
