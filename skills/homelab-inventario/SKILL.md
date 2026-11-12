---
name: homelab-inventario
description: Mapear e documentar hosts, serviços, redes, armazenamento e dependências do homelab. Use para criar ou atualizar inventário e runbooks a partir de arquivos e consultas autorizadas.
---

Comece pelas fontes existentes: documentação, manifests, Compose, inventário de automação e configurações versionadas. Não presuma Proxmox, Kubernetes, Docker ou qualquer provedor específico.

Registre para cada componente conhecido: função, host, forma de acesso, dependências, dados persistentes, configuração de origem e procedimento operacional disponível. Relacione serviços com DNS, proxy, rede e armazenamento quando houver evidência. Marque desconhecidos e registre a origem e a data das observações.

Diferencie configuração declarada de estado observado. Use consultas de leitura apenas nos destinos autorizados; não faça varredura de rede por inferência. Não registre senhas, tokens, chaves privadas ou conteúdo de arquivos de segredo. Registre somente a referência ao mecanismo de segredos.

Atualize a documentação no formato já usado pelo repositório. Sem convenção, proponha um inventário Markdown e runbooks por serviço quando necessários. Não invente endereços, nomes ou procedimentos de recuperação.
