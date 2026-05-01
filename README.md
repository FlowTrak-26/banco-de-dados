<img src="./imgs/backReadme.png" style="width:100%"> 
<div align="center">

# FlowTrak™ — Banco de Dados

**Modelagem e Scripts SQL do Sistema de Monitoramento de Fluxo**

</div>
<h1>Sobre o Repositório</h1>

Este repositório contém o diagrama e os scripts de criação de tabelas da **FlowTrak™**, incluindo:

- Modelo entidade-relacionamento (`.mwb`) criado no **MySQL Workbench**
- Script SQL de criação e população do banco (`script.sql`)
- Documentação visual da modelagem (pasta `imgs/`)

O banco de dados é responsável por armazenar todos os registros de fluxo de clientes capturados pelos sensores IoT distribuídos no supermercado (entradas, saídas, corredores e caixas), possibilitando análise histórica.


## Estrutura do Repositório

```
banco-de-dados/
├── modelagem-banco.mwb          # Arquivo do diagrama
├── script.sql                   # Script de criação das tabelas e dados
└── README.md
```

## Tecnologias Utilizadas

| Tecnologia | Finalidade |
|---|---|
| **MySQL** | Sistema gerenciador de banco de dados |
| **MySQL Workbench** | Utilizado para criação do diagrama|

## Contexto na Arquitetura FlowTrak

Os sensores instalados em pontos estratégicos do supermercado enviam dados via API para o banco, que os armazena de forma estruturada. A aplicação web consome essas informações para gerar gráficos, indicadores e alertas em tempo real.

## Como Utilizar

### Pré-requisitos

- MySQL Server instalado (local ou em nuvem)
- MySQL Workbench (para visualizar o nosso diagrama)

### Importando o banco de dados

1. Para clonar o repositório:
```terminal
git clone https://github.com/FlowTrak-26/banco-de-dados.git
```

### Visualizando a Modelagem

Dentro do arquivo `modelagem-banco.mwb` você consegue visualizar o diagrama com a modelagem do nosso sistema.
