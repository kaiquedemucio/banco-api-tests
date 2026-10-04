# banco-api-tests

## Objetivo

Este projeto realiza testes automatizados na API REST do
[banco-api](https://github.com/kaiquedemucio/banco-api-tests), validando suas
funcionalidades e contribuindo a qualidade de suas operações.

## Stack utilizada

-   **Linguagem:** JavaScript (Node.js)
-   **Framework de testes:** [Mocha](https://mochajs.org/)
-   **Biblioteca de requisições HTTP:**
    [Supertest](https://www.npmjs.com/package/supertest)
-   **Biblioteca de asserções:** [Chai](https://www.chaijs.com/)
-   **Relatórios de testes:**
    [Mochawesome](https://www.npmjs.com/package/mochawesome)
-   **Gerenciamento de variáveis de ambiente:**
    [dotenv](https://www.npmjs.com/package/dotenv)

## Estrutura de diretórios

``` bash
banco-api-tests/
├── test/                  # Testes organizados por funcionalidades
│   ├── login.test.js
│   └── transferencias.test.js
├── mochawesome-report/    # Diretório gerado automaticamente com o relatório HTML dos testes
├── .env                   # Arquivo para configuração da variável BASE_URL
├── .gitignore
├── package.json
└── README.md
```

## Formato do arquivo `.env`

Antes de rodar os testes, crie um arquivo chamado `.env` na raiz do
projeto com o seguinte conteúdo:

``` ini
BASE_URL=http://localhost:3000
```

Substitua `http://localhost:3000` pela URL onde a API
[banco-api](https://github.com/kaiquedemucio/banco-api) está rodando.

## Comandos para execução

Instale as dependências:

``` bash
npm install
```

Execute todos os testes:

``` bash
npm test
```

### Gerar o relatório HTML

O **Mochawesome** já está integrado ao projeto e o relatório será gerado
automaticamente após a execução dos testes, dentro da pasta:

``` text
mochawesome-report/
```

Se quiser executar os testes e abrir automaticamente o relatório após os
testes, você pode adicionar um script extra no `package.json`, como, por
exemplo:

``` json
"scripts": {
  "test:report": "npm test && open mochawesome-report/mochawesome.html"
}
```

> **Windows:** você pode usar `start` ao invés de `open`.

## Dependências utilizadas e suas documentações

-   [Mocha](https://mochajs.org/) - Framework de execução de testes
-   [Supertest](https://www.npmjs.com/package/supertest) - Biblioteca
    para chamadas HTTP
-   [Chai](https://www.chaijs.com/) - Biblioteca de asserções
-   [Mochawesome](https://www.npmjs.com/package/mochawesome) - Geração
    de relatórios em HTML
-   [dotenv](https://www.npmjs.com/package/dotenv) - Gerenciamento de
    variáveis de ambiente

## 👨‍💻 Autor

**Kaique Demucio**

- GitHub: [https://github.com/kaiquedemucio](https://github.com/kaiquedemucio)
- LinkedIn: [https://www.linkedin.com/in/kaiquedemucio/](https://www.linkedin.com/in/kaiquedemucio/)
- Portfólio: [https://kaiquedemucio.github.io/](https://kaiquedemucio.github.io/)

