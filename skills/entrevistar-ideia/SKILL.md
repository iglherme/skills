---
name: entrevistar-ideia
description: Questionar uma ideia, plano ou decisão para expor premissas frágeis e esclarecer escolhas antes da implementação. Use quando o usuário pedir uma entrevista crítica, grill-me ou para testar seu raciocínio.
---

Identifique a decisão que o usuário quer amadurecer e os limites do pedido. Leia o contexto disponível antes de perguntar: fatos sobre código, ferramentas e configuração devem ser investigados com as ferramentas disponíveis; preferências, objetivos e escolhas pertencem ao usuário.

Organize mentalmente as decisões por dependência. Comece pelas que podem ser resolvidas agora sem presumir respostas a questões abertas. Faça rodadas curtas em português, salvo preferência diferente do usuário, agrupando apenas perguntas independentes. Use a interface de perguntas quando disponível e adequada; caso contrário, apresente perguntas numeradas na conversa.

Para cada pergunta, explique a escolha concreta e seu efeito, apresente alternativas plausíveis e dê uma recomendação justificada quando houver evidência suficiente. Explicite as hipóteses dessa recomendação. Deixe espaço para uma resposta diferente das opções sugeridas. Aguarde as respostas antes de avançar nas questões dependentes.

Teste premissas com cenários concretos e proporcionais ao projeto: um requisito pode conflitar com o tempo disponível, uma solução com a capacidade de manutenção, ou uma decisão de infraestrutura com a recuperação esperada. Questione essas relações sem transformar a entrevista em discussão de requisitos adjacentes ou problemas hipotéticos sem relevância.

Após cada rodada, incorpore as respostas e reavalie o que ainda muda a decisão. Se o usuário não souber responder, exponha a incerteza e proponha uma pesquisa ou experimento delimitado; diferencie uma hipótese provisória de uma escolha aceita. Não repita perguntas já respondidas nem prolongue a entrevista para preencher um roteiro.

Encerre quando houver entendimento suficiente para a decisão pedida, ou quando o usuário pedir para parar. Resuma objetivo, escolhas, motivos, trade-offs e incertezas restantes. A entrevista não autoriza implementar, publicar ou alterar infraestrutura; continue essas ações somente quando fizerem parte do escopo já autorizado.

Se o usuário também pedir documentação, use [registrar-decisoes](../registrar-decisoes/SKILL.md) para registrar termos acordados e decisões que mereçam ADR. Se essa skill não estiver instalada junto, consulte a documentação existente do projeto e registre contexto, alternativas, decisão, estado e consequências no formato local. Sem pedido de documentação, mantenha o resumo na conversa. Propostas ainda não aceitas devem permanecer identificadas como propostas.
