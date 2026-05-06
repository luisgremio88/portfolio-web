# Segurança e LGPD

## Postura adotada para o portfolio

Este portfolio segue o princípio de minimização: somente informações necessárias para demonstrar o projeto devem ser publicadas. Dados reais, documentos gerados, credenciais, backups e integrações sensíveis ficam fora do repositório público.

## O que não deve ir para o GitHub público

- Arquivos `.env` reais.
- Senhas, tokens, chaves de API, certificados e credenciais bancárias.
- Dados de clientes, usuários, tabelionatos ou colaboradores.
- PDFs reais de boleto, recibo, certidão ou busca.
- Arquivos CNAB, retorno bancário ou remessa.
- Dumps de banco de dados.
- Backups, logs e arquivos temporários.
- Documentos internos da empresa.

## Medidas já previstas

- Separação entre versão real e versão demonstrativa.
- Uso de `.env.example` sem segredos.
- `.gitignore` bloqueando arquivos sensíveis e gerados.
- Dados fictícios para demonstração.
- Documentação clara sobre limites do portfolio.
- Fluxo de boleto, recibo e certidão tratado como modo demo.

## O que precisa para produção

- Autenticação com senha forte e hash seguro.
- Controle de sessão com expiração e renovação segura.
- Proteção contra CSRF em formulários administrativos.
- Validação e sanitização de entrada no backend.
- Controle de permissões por perfil.
- Logs de auditoria para ações sensíveis.
- Rate limit em login, recuperação de senha e APIs públicas.
- HTTPS obrigatório.
- Política de backup criptografado.
- Rotação de credenciais.
- Secret scanning no GitHub.
- Pipeline de deploy sem copiar arquivos sensíveis.
- Revisão jurídica/privacidade para base legal, retenção e descarte de dados.

## Perfis de acesso sugeridos

- Administrador: acesso total à gestão do sistema.
- Operador: acesso às rotinas administrativas permitidas.
- Financeiro: acesso a boletos, pagamentos e relatórios financeiros.
- Associado/Tabelionato: acesso restrito aos próprios dados e solicitações.
- Visitante: acesso apenas ao conteúdo público.

## Observação sobre LGPD

O objetivo desta versão pública é demonstrar competência técnica sem expor dados pessoais. Em produção, o sistema deve aplicar os princípios de segurança, prevenção, necessidade, transparência e responsabilização.

