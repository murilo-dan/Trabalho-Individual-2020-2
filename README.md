[![Actions Status](https://github.com/murilo-dan/Trabalho-Individual-2020-2/actions/workflows/main.yml/badge.svg)](https://github.com/murilo-dan/Trabalho-Individual-2020-2/actions)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=murilo-dan_Trabalho-Individual-2020-2&metric=alert_status)](https://sonarcloud.io/dashboard?id=murilo-dan_Trabalho-Individual-2020-2)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=murilo-dan_Trabalho-Individual-2020-2&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=murilo-dan_Trabalho-Individual-2020-2)
[![codecov](https://codecov.io/gh/murilo-dan/Trabalho-Individual-2020-2/branch/master/graph/badge.svg?token=NKEF3FNSRO)](https://codecov.io/gh/murilo-dan/Trabalho-Individual-2020-2)

# Trabalho Individual 2020.2

| Aluno | Matrícula |
| --- | --- |
| Murilo Loiola Dantas | 17/0163571 |

## 1. Containerização

A contaneirização da aplicação foi implementada através dois arquivos Dockerfile e um arquivo docker-compose.yml, para a orquestração.

Para rodar a aplicação, execute o seguinte comando:
```bash
docker-compose up --build
```

Espere a finalização da build (uma mensagem avisando que o projeto está rodando na porta 8000).

Acesse <code>localhost:8000</code> para visualizar o projeto.

## 2. Integração Contínua e Coverage

A integração contínua foi feita através de um pipeline usando o GitHub Actions. O pipeline é responsável por testar a build completa da aplicação, executar os testes e fazer as verificações de folhas de estilo e linter. Além disso, o pipeline faz comunicação com o SonarCloud e o CodeCov para escanear as métricas de código e a cobertura de testes do repositório, respectivamente.

Todo esse processo é realizado através de jobs definidos no pipeline. É possível observar a execução de cada job paralelamente na aba do GitHub Actions.

Clicar nas badges que aparecem no começo desse README redirecionará para os sites utilizados na coleta de métricas.