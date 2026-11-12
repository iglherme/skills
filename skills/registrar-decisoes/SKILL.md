---
name: registrar-decisoes
description: Esclarecer vocabulário de um projeto e registrar decisões arquiteturais com suas alternativas e consequências. Use para resolver termos ambíguos ou documentar escolhas duráveis.
---

Leia glossário, documentação e registros de decisão existentes antes de criar arquivos. Use exemplos concretos para distinguir termos ambíguos e compare a interpretação acordada com o comportamento do código. Trate divergências como questões a resolver, sem substituir silenciosamente a definição oficial.

Registre termos quando forem descobertos ou acordados. Um glossário descreve conceitos e relações, não detalhes de implementação nem requisitos futuros. Não crie divisão em múltiplos domínios sem uma necessidade observada.

Registre uma decisão arquitetural quando houver uma escolha real entre alternativas, custo relevante de reversão e um motivo que seria difícil reconstruir depois. Decisões triviais podem ficar na tarefa ou na documentação corrente.

Use o formato e o local existentes. Sem convenção, use `docs/GLOSSARY.md` para termos e `docs/adr/NNNN-assunto.md` para decisões. Um ADR deve conter título, data, estado, contexto, alternativas consideradas, decisão, motivos e consequências. Marque propostas como propostas; não invente aceitação do usuário.

Preserve histórico: quando uma decisão mudar, registre a nova decisão e a relação com a anterior. Inclua referências às evidências ou restrições relevantes e mantenha credenciais fora dos documentos.
