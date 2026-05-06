# Roadmap para deixar completo e mais seguro

## Prioridade 1 - Seguranca basica

- Centralizar configuracoes em variaveis de ambiente.
- Remover credenciais hardcoded.
- Criar perfis de acesso com permissoes claras.
- Revisar login, sessao e recuperacao de senha.
- Adicionar CSRF em formularios.
- Validar entradas no backend PHP e nas APIs Java.
- Garantir HTTPS em producao.

## Prioridade 2 - Backend Java

- Consolidar APIs Java para area restrita, financeiro e servicos de associado.
- Separar regras de negocio novas do legado PHP quando fizer sentido.
- Criar camada de DTOs e validacoes.
- Adicionar testes unitarios e de integracao.
- Documentar endpoints com Swagger/OpenAPI.
- Configurar logs estruturados.
- Criar health check para monitoramento.

## Prioridade 3 - Auditoria e LGPD

- Registrar logs de acesso e acoes administrativas.
- Criar politica de retencao de documentos.
- Criar rotina de descarte seguro.
- Mapear quais dados pessoais sao tratados.
- Documentar finalidade, base legal e prazo de guarda.
- Criar termo de uso e politica de privacidade.

## Prioridade 4 - Infraestrutura

- Separar ambientes: desenvolvimento, homologacao e producao.
- Automatizar deploy sem copiar arquivos sensiveis.
- Configurar backups criptografados.
- Monitorar erros e disponibilidade.
- Criar rotina de atualizacao de dependencias.
- Separar deploy do React, PHP e Java quando necessario.

## Prioridade 5 - Qualidade

- Criar testes para fluxos criticos.
- Testar emissao de boleto, recibo e certidao.
- Testar permissoes por perfil.
- Testar responsividade.
- Revisar acessibilidade.

## Prioridade 6 - Integracoes reais

- Integrar provedor bancario real.
- Integrar comunicacao com bases externas quando autorizado.
- Registrar falhas de integracao.
- Criar modo de contingencia quando servicos externos estiverem indisponiveis.

