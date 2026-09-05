# Padrões de Repositórios da Alphavision®

Este documento estabelece os padrões gerais utilizados nos repositórios públicos mantidos pela organização Alphavision® no GitHub.

As características específicas de cada projeto poderão exigir adaptações, desde que sejam documentadas no próprio repositório.

## Nomenclatura

Os nomes dos repositórios devem utilizar letras minúsculas e palavras separadas por hífen.

Exemplos:

- `whmcs-auto-login`
- `whmcs-consulta-cnpj`
- `wordpress-last-modified`
- `whmcs-pt-br`
- `lagom-pt-br`
- `vscode-config`

Não é necessário utilizar `alphavision-` como prefixo nos nomes dos repositórios, pois os projetos já estão identificados pela organização `alphavisionbr`.

## Idiomas

O idioma principal da documentação é Português do Brasil (pt-BR).

Sempre que possível, projetos destinados também à comunidade internacional deverão possuir documentação em inglês.

O padrão para os arquivos principais é:

```text
README.md
README.en.md
```

Para documentações maiores, poderá ser utilizada a estrutura:

```text
docs/
├── pt-BR/
└── en/
```

Issues e Pull Requests poderão ser enviados em português ou inglês.

## Estrutura básica

Sempre que aplicável, os repositórios deverão utilizar a seguinte estrutura:

```text
projeto/
├── docs/
├── .gitignore
├── CHANGELOG.md
├── LICENSE
├── README.md
└── README.en.md
```

Arquivos e diretórios adicionais deverão ser incluídos conforme as necessidades específicas de cada projeto.

## Licenciamento

Cada repositório deverá possuir sua própria licença.

Não existe uma licença única obrigatória para todos os projetos da Alphavision®.

Como orientação geral:

- Plugins para WordPress: GPL-2.0-or-later
- Bibliotecas, ferramentas e utilitários PHP: MIT, quando apropriado
- Módulos open source para WHMCS: licença definida individualmente conforme as características do projeto
- Configurações, snippets e exemplos: MIT, quando apropriado
- Documentação produzida pela Alphavision®: licença definida conforme a finalidade do material

Projetos que não devam permitir redistribuição, modificação ou reutilização não deverão ser publicados como projetos open source sem uma análise específica de licenciamento.

Dependências, traduções e materiais relacionados a softwares de terceiros deverão respeitar as respectivas licenças e direitos dos projetos originais.

## Versionamento

Os projetos deverão utilizar Semantic Versioning sempre que aplicável.

Formato:

```text
MAJOR.MINOR.PATCH
```

Exemplos:

```text
1.0.0
1.0.5
2.0.0
2.1.3
```

Versões de desenvolvimento poderão utilizar identificadores como:

```text
1.0.5-rc.1
1.0.5-rc.2
2.0.0-beta.1
```

## Tags

As tags de versões deverão utilizar o prefixo `v`.

Exemplos:

```text
v1.0.0
v2.1.3
```

## Releases

Versões estáveis deverão ser publicadas como releases normais.

Versões beta, RC ou outras versões de teste deverão ser identificadas como pre-release.

Quando aplicável, o arquivo instalável do projeto deverá ser disponibilizado como asset da release.

Exemplo de título:

```text
Alphavision® WHMCS Auto Login v2.1.3
```

## Changelog

Projetos versionados deverão utilizar `CHANGELOG.md` sempre que o histórico de alterações for relevante.

O changelog será mantido prioritariamente em Português do Brasil.

Estrutura recomendada:

```markdown
## [2.1.3] - 2026-07-21

### Adicionado

- Nova configuração para escolha da rota utilizada pelo Auto Login.

### Alterado

- Ajustado o contraste dos títulos da página de configuração.

### Corrigido

- Ajustes relacionados à geração das URLs de acesso.
```

Não é obrigatória a criação de um `CHANGELOG.en.md` para todos os projetos.

## Topics

Os GitHub Topics deverão ser utilizados para facilitar a classificação e descoberta dos projetos.

Exemplos:

```text
wordpress
woocommerce
whmcs
plesk
php
linux
translation
developer-tools
open-source
```

Os Topics deverão ser escolhidos de acordo com o conteúdo de cada repositório.

## Arquivos comunitários

Os repositórios deverão utilizar, sempre que aplicável, os arquivos comunitários definidos no repositório `.github` da organização, incluindo:

- Código de Conduta
- Diretrizes de Contribuição
- Política de Segurança
- Templates de Issues
- Template de Pull Request

Quando um projeto necessitar de regras específicas, poderá possuir seus próprios arquivos, substituindo os padrões da organização.

## Segurança

Vulnerabilidades de segurança não deverão ser relatadas por meio de Issues públicas.

Os projetos deverão seguir a Política de Segurança publicada pela organização Alphavision®.

## Alphavision®

Estes padrões são mantidos pela **Alphavision®** para seus projetos públicos e open source no GitHub.

**Site:** https://alphavision.com.br  
**Contato:** contato@alphavision.com.br
