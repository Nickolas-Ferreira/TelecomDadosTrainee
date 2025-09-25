# Gerador de Dados Fictícios – Telecom

Este repositório fornece uma solução em Python que gera dados fictícios para simular dados de uma **empresa de Telecomunicações** (clientes, assinaturas, chamadas, faturas e tickets de suporte), especialmente desenvolvido para ser usado em uma demonstração para a turma da Residência de Dados Serratec 2025, utilizando o Databricks e processando dados em sua arquitetura Medalhão (Bronze-Silver-Gold).

## Estrutura

- `GeradorDadosFakeTelecom` (classe principal)
  - `gerar_clientes`: Cria o cadastro inicial de clientes.
  - `gerar_assinaturas`: Gera planos contratados (voz, dados, internet).
  - `gerar_chamadas`: Produz registros de chamadas e consumo de dados (CDRs).
  - `gerar_faturas`: Cria cobranças mensais vinculadas às assinaturas.
  - `gerar_tickets`: Simula chamados de suporte técnico e reclamações.
  - `carga_inicial`: Inicializa diretórios e gera a primeira carga de dados.
  - `gerar_incremental`: Produz cargas incrementais (novos clientes, CDRs, tickets).
  - `verificar_e_gerar_dados`: Verifica existência de dados e gera carga inicial ou incremental automaticamente.
  - `stream`: Simula streaming de dados gerando lotes incrementais em intervalos definidos.

## Pré-requisitos

- Acesso ao Databricks (Unity Catalog e Volumes)

## Instalação

Clone este repositório ou importe o arquivo diretamente em um notebook Databricks:

```bash
git clone https://github.com/SeuRepo/Residencia-Dados-Telecom.git
