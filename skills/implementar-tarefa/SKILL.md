---
name: implementar-tarefa
description: Implementar funcionalidades e corrigir bugs em projetos pessoais a partir de uma tarefa definida. Use quando houver código ou comportamento a alterar; planejamento amplo pertence a planejar-projeto.
---

Leia as instruções locais, o estado do Git e os pontos de entrada relacionados à tarefa. Preserve alterações do usuário e identifique como o projeto é executado e validado antes de editar.

Para bugs, procure uma reprodução ou evidência que diferencie a causa de um sintoma. Para funcionalidades, derive o comportamento esperado do pedido e das convenções existentes. Faça a menor alteração coerente com esse comportamento, sem incluir refatorações independentes.

Valide o caminho alterado com os testes e verificações pertinentes disponíveis. Use teste de regressão quando ele provar um comportamento relevante; não introduza infraestrutura de testes apenas para uma edição trivial. Se uma verificação não puder rodar, relate a limitação sem afirmar sucesso.

Atualize documentação ou exemplos afetados. Entregue um resumo do comportamento, validação realizada e limitações. Commit, push, publicação e deploy seguem o escopo autorizado pelo usuário.
