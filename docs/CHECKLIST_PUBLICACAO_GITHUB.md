# Checklist para publicar no GitHub

Antes de publicar qualquer versão pública:

- [ ] Criar uma pasta ou repositório separado da versão real.
- [ ] Remover `.env`, `.env.development`, certificados e credenciais.
- [ ] Remover PDFs reais de buscas, boletos, recibos e certidões.
- [ ] Remover arquivos CNAB, remessa e retorno bancário.
- [ ] Remover banco de dados, dumps SQL e backups.
- [ ] Remover logs e arquivos temporários.
- [ ] Trocar dados reais por dados fictícios.
- [ ] Verificar imagens e documentos que possam identificar dados internos.
- [ ] Conferir `.gitignore`.
- [ ] Rodar uma busca por termos sensíveis como senha, token, secret, password, api_key, cpf, cnpj.
- [ ] Criar `.env.example` somente com valores falsos.
- [ ] Ativar Secret Scanning e Push Protection no GitHub.
- [ ] Publicar primeiro como repositório privado para revisão.
- [ ] Só transformar em público depois da revisão final.

## Comandos úteis

```bash
git status
git init
git add README.md docs .gitignore .env.example
git commit -m "docs: add portfolio security documentation"
```

## Busca local recomendada

```bash
git grep -n "senha\|password\|token\|secret\|api_key\|cpf\|cnpj"
```

Se algum dado sensível já foi enviado para o GitHub, apagar o arquivo no commit seguinte não é suficiente. É necessário limpar o histórico ou criar um repositório novo sem esse histórico.

