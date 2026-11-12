---
name: homelab-mudanca
description: Preparar e executar mudanças autorizadas de configuração, atualizações e deploys no homelab. Use quando uma alteração de infraestrutura precisar de validação, sequência e reversão.
---

Localize a fonte de configuração e a ferramenta usada pelo ambiente. Confirme destino e escopo a partir do pedido e das evidências; não trate exemplos de documentação como alvos reais.

Inspecione diferenças, dependências, versões atuais e persistência. Para atualização, consulte documentação oficial da versão alvo quando necessária para compatibilidade e migrações. Defina validação antes da mudança, efeito esperado e reversão específica; migrações de dados podem exigir restauração em vez de simples retorno de imagem.

Prepare a alteração em arquivos versionados e use validação estática, renderização ou dry-run quando disponíveis. Inspecione saídas que possam conter segredos. Não substitua gerenciamento declarativo por edições manuais sem justificar a necessidade.

Execute no destino somente quando autorizado, na menor unidade que permita observar o resultado. Se falhar, interrompa a sequência, examine a causa e use a reversão prevista quando autorizada; não repita mutações indefinidamente.

Verifique o serviço e suas dependências após aplicar. Relate o que foi preparado, aplicado e efetivamente validado, incluindo indisponibilidade ou pendências. Não amplie para outros hosts ou serviços por conveniência.
