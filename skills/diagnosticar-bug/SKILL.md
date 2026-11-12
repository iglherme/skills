---
name: diagnosticar-bug
description: Investigar bugs difíceis e regressões de desempenho no código com reprodução mínima e testes de hipóteses. Use para defeitos de software; falhas operacionais do homelab pertencem a homelab-diagnostico.
---

Use o relato e as evidências fornecidas como ponto de partida. Identifique o sintoma exato e procure um sinal observável capaz de distinguir esse defeito de uma falha próxima: teste, comando com fixture, requisição local ou medição de desempenho.

Construa uma reprodução curta e reduza entradas ou dependências uma por vez, mantendo o sintoma. Aproveite evidência existente; novas execuções devem reduzir incerteza ou verificar a correção. Para intermitência, registre frequência e condições, limite repetições e aplique estresse apenas em ambiente isolado autorizado.

Se não for possível reproduzir, explicite o limite e investigue por inspeção ou evidência disponível, identificando hipóteses como hipóteses. Não invente um teste passando ou bloqueie toda análise por ausência de reprodução.

Liste hipóteses plausíveis com previsões verificáveis e escolha consultas que as distingam. Altere uma variável por vez. Para lentidão, obtenha uma medida comparável antes e depois; use profiler ou plano de consulta quando isso trouxer mais informação que logs.

Corrija a causa sustentada pelas evidências. Quando houver uma interface adequada, transforme a reprodução em teste de regressão, observando falha antes e sucesso depois da correção. Verifique também o cenário original. Remova instrumentação temporária criada na tarefa, preserve evidências úteis sem segredos e relate causa, validação e incertezas restantes.

Bisseção e experimentos que alteram código devem preservar o trabalho existente e usar um checkout apropriado. Diagnóstico não autoriza executar cargas, instrumentar ou modificar produção.
