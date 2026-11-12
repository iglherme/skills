---
name: revisar-alteracoes
description: Revisar diffs e mudanças de projetos pessoais procurando bugs, regressões e lacunas de validação. Use para revisão de código ou preparação de uma entrega, sem presumir autorização para publicar.
---

Determine o diff solicitado e leia o contexto dos trechos alterados, seus consumidores e testes relevantes. Diferencie problemas introduzidos pela mudança de problemas antigos.

Priorize falhas demonstráveis: comportamento incorreto, perda de dados, permissões, compatibilidade e migrações. Não transforme preferências de estilo em defeitos. Para cada achado, informe arquivo e linha, condição que dispara o problema, impacto e evidência; sinalize incerteza quando depender de uma hipótese.

Execute verificações focadas se disponíveis e proporcionais. Em revisões puras, apresente achados antes de alterar código. Se o usuário pedir correções, implemente-as no escopo autorizado e valide novamente o comportamento afetado.

Se não houver achados, diga isso e descreva os limites da revisão. Não confunda testes passando com garantia de ausência de defeitos.
