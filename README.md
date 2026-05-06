# Sistema web institucional, area restrita e painel administrativo

Portfolio tecnico de um sistema web completo, com site publico, area restrita, painel administrativo, backend PHP, modulo Java e preocupacao com LGPD desde a publicacao.

> Esta versao publica e demonstrativa. Ela nao contem dados reais, credenciais, documentos emitidos, boletos, recibos, certidoes, dumps de banco ou arquivos internos da empresa.

## Visao geral

O projeto representa uma plataforma institucional com operacoes internas e area autenticada. A proposta e demonstrar dominio de ponta a ponta: interface, rotas, integracao com backend, emissao documental, organizacao administrativa e planejamento de seguranca.

## Stack principal

| Camada | Tecnologias |
| --- | --- |
| Frontend | React 17, React Router, Axios |
| Backend legado/operacional | PHP, Template Power, FPDF |
| Backend de servicos | Java |
| Banco de dados | MySQL |
| Documentos | Geracao demonstrativa de boleto, recibo e certidao |
| Seguranca | Separacao de ambiente, `.env.example`, checklist LGPD, roadmap de hardening |

## Destaques tecnicos

- Site publico responsivo com conteudo institucional, noticias, eventos, galeria, videos e links uteis.
- Area restrita para associados/tabelionatos com rotas protegidas e fluxo operacional.
- Painel administrativo para gestao de conteudos, consultas e documentos.
- Fluxo de busca documental/testamento com preenchimento guiado.
- Geracao demonstrativa de boleto, recibo e certidao.
- Backend PHP para rotinas administrativas, templates, endpoints e PDFs.
- Modulo Java planejado/usado como camada de servicos para area restrita, financeiro e integracoes.
- Documentacao de seguranca com foco em LGPD e publicacao segura no GitHub.

## Arquitetura resumida

```text
Usuario publico
      |
      v
Site React --------------+
                         |
Area restrita React -----+----> APIs PHP ----> MySQL
                         |         |
Painel administrativo ---+         +----> PDFs / boletos / recibos / certidoes
                         |
                         +----> APIs Java ----> servicos de associado, financeiro e integracoes
```

## Modulos do sistema

### Site publico

Home institucional, paginas de conteudo, noticias, eventos, galeria, videos, contato, links uteis e acesso para usuarios autenticados.

### Area restrita

Ambiente autenticado para associados/tabelionatos, com dados cadastrais, consultas, financeiro e fluxo de busca documental.

### Painel administrativo

Gestao interna para administradores e operadores, com controle de conteudo, consultas, documentos e emissao de arquivos PDF.

### Busca documental

Fluxo demonstrativo no qual o usuario preenche os dados da busca, confirma responsabilidade, gera boleto e, quando autorizado, visualiza recibo e certidao.

### Backend PHP

Responsavel por rotinas existentes do sistema, endpoints web, templates administrativos, comunicacao com MySQL e geracao de documentos em PDF.

### Modulo Java

Camada de servicos para evoluir regras de negocio, APIs de associado, financeiro e integracoes. Em producao, essa camada pode receber validacoes, DTOs, Swagger/OpenAPI, testes e health checks.

## Seguranca e LGPD

A versao publica foi preparada para demonstrar o projeto sem expor informacoes sensiveis. A estrategia adotada:

- dados reais removidos;
- arquivos `.env` reais fora do repositorio;
- `.env.example` apenas com valores ficticios;
- `.gitignore` bloqueando builds, documentos, backups, logs e credenciais;
- documentacao explicando o que nao deve ser publicado;
- roadmap de melhorias para ambiente de producao.

Documentos:

- [Seguranca e LGPD](docs/SEGURANCA_LGPD.md)
- [Checklist de publicacao no GitHub](docs/CHECKLIST_PUBLICACAO_GITHUB.md)
- [Roadmap de producao](docs/ROADMAP_PRODUCAO.md)

## O que falta para producao

- Revisao completa de autenticacao, sessoes e permissoes.
- CSRF, rate limit e validacoes centralizadas.
- Logs de auditoria para acoes sensiveis.
- Testes automatizados para fluxos criticos.
- Documentacao formal das APIs Java com Swagger/OpenAPI.
- Separacao de ambientes de desenvolvimento, homologacao e producao.
- Deploy automatizado sem copiar arquivos sensiveis.
- Politica de backup, retencao e descarte de documentos.

## Como rodar a parte React

```bash
npm install
npm start
```

## Como rodar a parte PHP

Use um ambiente local com Apache/PHP, como XAMPP, e configure as variaveis de ambiente usando `.env.example` como base.

## Como rodar a parte Java

O modulo Java deve ser configurado em ambiente separado, com variaveis de ambiente proprias para banco, portas e integracoes. Nesta versao publica, a documentacao descreve a arquitetura sem publicar credenciais, dados reais ou endpoints sensiveis.

## Observacao

Este repositorio foi montado como portfolio publico. O objetivo e mostrar arquitetura, escopo funcional, criterios de seguranca e maturidade de desenvolvimento sem comprometer dados protegidos por LGPD.

