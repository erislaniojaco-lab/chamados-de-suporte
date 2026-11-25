# chamados-de-suporte
# API de Chamados de Suporte

**Estudante:** Erislânio Jacó da Silva

## 1. Objetivo do Projeto

Desenvolver a estrutura inicial de uma API de chamados de suporte utilizando Python e Flask.

Nesta primeira etapa, foi implementada a rota inicial (`GET /`), responsável por verificar o funcionamento da API e retornar uma mensagem em formato JSON.

## 2. Tecnologias Utilizadas

- Python
- Flask
- uv (gerenciador de ambiente e dependências)

## 3. Instalação das Dependências

Após clonar o repositório, acesse a pasta do projeto e execute o comando:

```bash
uv sync --locked
```

Esse comando instala as dependências do projeto conforme as versões definidas no arquivo `uv.lock`.

## 4. Como Executar a Aplicação

No terminal, execute:

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

Após iniciar, a API estará disponível na porta 5000.

## 5. Acessando a Rota Inicial

Acesse pelo navegador:

```text
http://localhost:5000/
```

Ou faça uma requisição pelo terminal:

```bash
curl -i http://localhost:5000/
```

## 6. Resposta Esperada

A rota `GET /` deverá retornar o código HTTP `200 OK`, com o seguinte objeto JSON:

```json
{
  "mensagem": "API de chamados em funcionamento"
}
```

O cabeçalho da resposta deverá indicar:

```text
Content-Type: application/json
```

## 7. Estrutura do Projeto

```text
chamados-de-suporte/
├── app.py
├── pyproject.toml
├── uv.lock
├── .gitignore
├── README.md
└── .venv/
```