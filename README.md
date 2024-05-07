# PyKitInicial

PyKitInicial é um modelo de projeto Python para ajudá-lo a começar rapidamente com seus novos projetos Python. Ele inclui componentes essenciais como configuração de testes, linting, formatação e muito mais.

## Recursos

- **Gerenciamento de Versão Python**: Gerenciado com Pyenv.
- **Gerenciamento de Dependências**: Gerenciado com Poetry.
- **Formatação de Código**: A formatação de código é configurada com Black.
- **Linting**: O linting é configurado com Flake8.
- **Testes**: Os testes unitários são configurados com Pytest.
- **Hooks de pré-commit**: Os hooks de pré-commit são configurados com Pre-commit.

## Pré-requisitos

Antes de poder usar este modelo, você precisa ter as seguintes ferramentas instaladas em sua máquina:

- Python: Você pode baixá-lo do [site oficial](https://www.python.org/downloads/).
- Pyenv: Você pode instalá-lo usando as instruções no [repositório GitHub do Pyenv](https://github.com/pyenv/pyenv#installation).
- Poetry: Você pode instalá-lo usando as instruções no [site do Poetry](https://python-poetry.org/docs/#installation).
- Pre-commit: Você pode instalá-lo usando as instruções no [site do Pre-commit](https://pre-commit.com/#install).

Depois de ter essas ferramentas instaladas, você pode seguir as instruções na seção "Iniciando" para configurar seu projeto.

## Começando

Aqui estão os passos para criar um novo projeto a partir deste modelo:

1. Clique no botão "Use este modelo" para criar um novo repositório a partir deste modelo.
2. Clone o novo repositório para sua máquina local.
3. Defina a versão do Python para o seu projeto com Pyenv executando `pyenv local 3.x.x` (substitua 3.x.x pela versão do Python desejada).
4. Instale as dependências com Poetry executando `poetry install`.
5. Instale os hooks de pré-commit com `pre-commit install`.
6. Renomeie o projeto e ajuste as configurações de acordo com suas necessidades.

## Uso

Aqui está como você pode usar os diferentes recursos deste modelo:

- **Gerenciamento de Versão Python**: Você pode definir a versão do Python para o seu projeto com o comando `pyenv local 3.x.x`.
- **Executando Testes**: Você pode executar testes usando o comando `pytest`.
- **Linting**: Você pode lintar seu código usando o comando `flake8`.
- **Formatação**: Você pode formatar seu código usando o comando `black`.
- **Hooks de pré-commit**: Pre-commit verificará automaticamente seu código para erros de formatação e linting antes de cada commit.

Lembre-se, para entrar no shell do Poetry, use o comando `poetry shell`. Isso garante que o ambiente Python correto e as dependências sejam usados.

Para usar `black` e `flake8` dentro de um shell `poetry`, primeiro ative o shell com `poetry shell`, então você pode executar `black` e `flake8` como de costume.

## Personalizando o Projeto

### Atualize as Informações do Autor

O arquivo pyproject.toml contém um espaço reservado para as informações do autor. Para atualizá-lo:

1. Abra pyproject.toml em seu editor de texto.
2. Encontre o campo authors em [tool.poetry].
3. Substitua "Seu Nome <seu.email.email@example.com>" pelo seu nome e endereço de e-mail, assim:

```toml
authors = ["Seu nome de verdade <seu.email.de.verdade@example.com>"]
```

4. Salve e feche o arquivo


## Gerenciando Dependências com Poetry

Poetry é uma ferramenta para gerenciamento de dependências e empacotamento em Python. Ele permite que você declare as bibliotecas das quais seu projeto depende e ele irá gerenciá-las (instalar/atualizar) para você.

### Adicionando Dependências

Para adicionar uma nova dependência ao seu projeto, use o comando `poetry add` seguido pelo nome do pacote que você deseja adicionar:

```bash
poetry add nome-pacote
```

Isso adicionará o pacote ao seu arquivo pyproject.toml e o instalará em seu ambiente virtual.

### Atualizando Dependências

Para atualizar uma dependência para a versão mais recente, use o comando poetry update seguido pelo nome do pacote:

```bash
poetry update nome-pacote
```

Isso atualizará o pacote em seu ambiente virtual e atualizará o arquivo poetry.lock

### Executando arquivos

Para executar um arquivo Python em seu projeto, use o comando poetry run seguido pelo comando python e o caminho para o arquivo:

```bash
poetry run python caminho/do/arquivo.py
```

Isso garantirá que o arquivo seja executado no ambiente virtual com acesso às dependências especificadas em seu arquivo pyproject.toml.

Nota: Se você estiver usando uma sessão `poetry shell`, você pode executar scripts Python diretamente com o comando `python`, sem a necessidade de prefixá-lo com `poetry run`.

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para enviar um Pull Request.

## Licença

Este projeto está licenciado sob os termos da licença MIT.
