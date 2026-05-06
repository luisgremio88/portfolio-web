# Roadmap para deixar completo e mais seguro

## Prioridade 1 - Segurança básica

- Centralizar configurações em variáveis de ambiente.
- Remover credenciais hardcoded.
- Criar perfis de acesso com permissões claras.
- Revisar login, sessão e recuperação de senha.
- Adicionar CSRF em formulários.
- Validar entradas no backend.
- Garantir HTTPS em produção.

## Prioridade 2 - Auditoria e LGPD

- Registrar logs de acesso e ações administrativas.
- Criar política de retenção de documentos.
- Criar rotina de descarte seguro.
- Mapear quais dados pessoais são tratados.
- Documentar finalidade, base legal e prazo de guarda.
- Criar termo de uso e política de privacidade.

## Prioridade 3 - Infraestrutura

- Separar ambientes: desenvolvimento, homologação e produção.
- Automatizar deploy sem copiar arquivos sensíveis.
- Configurar backups criptografados.
- Monitorar erros e disponibilidade.
- Criar rotina de atualização de dependências.

## Prioridade 4 - Qualidade

- Criar testes para fluxos críticos.
- Testar emissão de boleto, recibo e certidão.
- Testar permissões por perfil.
- Testar responsividade.
- Revisar acessibilidade.

## Prioridade 5 - Integrações reais

- Integrar provedor bancário real.
- Integrar comunicação com bases externas quando autorizado.
- Registrar falhas de integração.
- Criar modo de contingência quando serviços externos estiverem indisponíveis.

