# Sistema institucional e administrativo - Portfolio

Este repositório apresenta uma versão demonstrativa de um sistema institucional completo, com site público, área restrita, painel administrativo e fluxo de busca documental com geração de boleto, recibo e certidão em modo de demonstração.

> Importante: este projeto de portfolio não contém dados reais de empresa, clientes, tabelionatos, documentos, boletos, recibos, certidões, chaves de API ou credenciais. Os nomes e fluxos descritos aqui são demonstrativos.

## Objetivo

Mostrar capacidade de desenvolver e organizar um sistema web completo, incluindo:

- home institucional moderna e responsiva;
- área restrita para usuários autenticados;
- painel administrativo;
- gestão de conteúdos institucionais;
- busca documental/testamento em fluxo guiado;
- geração demonstrativa de boleto, recibo e certidão;
- documentação técnica;
- preocupação com segurança, LGPD e separação de dados sensíveis.

## Tecnologias

- React 17
- React Router
- Axios
- PHP
- MySQL
- Template Power
- FPDF
- Integração preparada para APIs externas

## Principais áreas do sistema

### Site público

Interface institucional com páginas de conteúdo, notícias, eventos, galeria, vídeos, links úteis, contato e acesso à área restrita.

### Área restrita

Ambiente autenticado para associados/tabelionatos, com dados cadastrais, consultas, financeiro e fluxo de busca documental.

### Painel administrativo

Área de gestão interna para usuários administrativos, com controle de conteúdos, consultas, documentos e emissão de arquivos em PDF.

### Busca documental

Fluxo demonstrativo onde o usuário preenche dados da busca, confirma responsabilidade, gera boleto e, quando permitido, visualiza recibo e certidão.

## Segurança e LGPD

Esta versão foi pensada para portfolio, por isso não inclui dados reais. A estratégia de publicação segura está documentada em:

- [docs/SEGURANCA_LGPD.md](docs/SEGURANCA_LGPD.md)
- [docs/CHECKLIST_PUBLICACAO_GITHUB.md](docs/CHECKLIST_PUBLICACAO_GITHUB.md)
- [docs/ROADMAP_PRODUCAO.md](docs/ROADMAP_PRODUCAO.md)

## Como rodar a parte React

```bash
npm install
npm start
```

## Como rodar a parte PHP

Coloque o projeto em um ambiente local com Apache/PHP, como XAMPP, e configure as variáveis de ambiente usando `.env.example` como base.

## Status do projeto

Projeto em evolução para demonstração profissional. A versão de produção exigiria reforços adicionais de segurança, auditoria, logs, controle de permissões e integração real com provedores externos.

