# Sistema institucional e administrativo - Portfolio

Este repositorio apresenta uma versao demonstrativa de um sistema institucional completo, com site publico, area restrita, painel administrativo, backend PHP e modulo Java preparado para servicos e integracoes.

> Importante: este projeto de portfolio nao contem dados reais de empresa, clientes, tabelionatos, documentos, boletos, recibos, certidoes, chaves de API ou credenciais. Os nomes e fluxos descritos aqui sao demonstrativos.

## Objetivo

Mostrar capacidade de desenvolver e organizar um sistema web completo, incluindo:

- home institucional moderna e responsiva;
- area restrita para usuarios autenticados;
- painel administrativo;
- backend PHP para rotinas administrativas e emissao de documentos;
- modulo Java para APIs, servicos de associado e integracoes;
- gestao de conteudos institucionais;
- busca documental/testamento em fluxo guiado;
- geracao demonstrativa de boleto, recibo e certidao;
- documentacao tecnica;
- preocupacao com seguranca, LGPD e separacao de dados sensiveis.

## Tecnologias

- React 17
- React Router
- Axios
- PHP
- Java
- MySQL
- Template Power
- FPDF
- Integracao preparada para APIs externas

## Arquitetura resumida

```text
Site publico / Area restrita
        |
        v
React + Axios
        |
        +--> APIs PHP: autenticacao, conteudo, busca documental, PDFs
        |
        +--> APIs Java: servicos de associado, financeiro e integracoes futuras
        |
        v
MySQL / provedores externos em ambiente de producao
```

## Principais areas do sistema

### Site publico

Interface institucional com paginas de conteudo, noticias, eventos, galeria, videos, links uteis, contato e acesso a area restrita.

### Area restrita

Ambiente autenticado para associados/tabelionatos, com dados cadastrais, consultas, financeiro e fluxo de busca documental.

### Painel administrativo

Area de gestao interna para usuarios administrativos, com controle de conteudos, consultas, documentos e emissao de arquivos em PDF.

### Backend PHP

Responsavel por rotinas existentes do sistema, templates administrativos, endpoints web, emissao de PDFs, recibos, certidoes e comunicacao com banco de dados.

### Modulo Java

Camada preparada para evoluir servicos de associado, financeiro, consultas e integracoes. A ideia e separar regras de negocio mais novas em APIs, facilitando manutencao, escalabilidade e testes.

### Busca documental

Fluxo demonstrativo onde o usuario preenche dados da busca, confirma responsabilidade, gera boleto e, quando permitido, visualiza recibo e certidao.

## Seguranca e LGPD

Esta versao foi pensada para portfolio, por isso nao inclui dados reais. A estrategia de publicacao segura esta documentada em:

- [docs/SEGURANCA_LGPD.md](docs/SEGURANCA_LGPD.md)
- [docs/CHECKLIST_PUBLICACAO_GITHUB.md](docs/CHECKLIST_PUBLICACAO_GITHUB.md)
- [docs/ROADMAP_PRODUCAO.md](docs/ROADMAP_PRODUCAO.md)

## Como rodar a parte React

```bash
npm install
npm start
```

## Como rodar a parte PHP

Coloque o projeto em um ambiente local com Apache/PHP, como XAMPP, e configure as variaveis de ambiente usando `.env.example` como base.

## Como rodar a parte Java

O modulo Java deve ser configurado em ambiente separado, com variaveis de ambiente proprias para banco, portas e integracoes. Nesta versao publica, a documentacao descreve a arquitetura sem publicar credenciais, dados reais ou endpoints sensiveis.

## Status do projeto

Projeto em evolucao para demonstracao profissional. A versao de producao exigiria reforcos adicionais de seguranca, auditoria, logs, controle de permissoes, testes automatizados e integracao real com provedores externos.

