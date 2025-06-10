# Organizador de Declaração de Imposto de Renda 🦁

## 📝 Descrição do Projeto

Este projeto, desenvolvido como parte de um desafio da DIO, consiste em uma ferramenta criada em Excel para agregar e organizar de forma eficiente as informações essenciais para a declaração de imposto de renda (IRPF).

A solução funciona como um centralizador de dados, permitindo ao usuário controlar suas movimentações financeiras e de investimentos de maneira prática e validada. A planilha possui uma interface amigável, com menus de navegação, validações automáticas e funcionalidades extras para otimizar o processo de preparação para a declaração anual.

![app_interface]()

## 🎯 Objetivos

O principal objetivo é simplificar a organização de dados fiscais, oferecendo uma ferramenta robusta e prática que pode ser um excelente diferencial no portfólio. Ao utilizar esta planilha, o usuário poderá:

-   Centralizar informações de diferentes fontes (Informes de Rendimentos, Notas de Corretagem).
-   Manter um registro claro e organizado das operações financeiras.
-   Facilitar a consulta de dados na hora de preencher a declaração oficial.
-   Reduzir a chance de erros e omissões.

## ✨ Funcionalidades Principais

-   **Navegação Facilitada:** Menus e links rápidos que permitem ao usuário navegar entre as diferentes seções da planilha com apenas um clique.
-   **Validação de Dados:** Campos com listas suspensas e validações automáticas para garantir a integridade e a padronização das informações inseridas (Ex: Lista de Bancos, Tickers da B3).
-   **Cadastro de Informações do Titular:** Seção para registrar os dados pessoais e bancários do declarante.
-   **Lançamento de Informes de Rendimentos:** Aba dedicada para registrar os valores recebidos de fontes pagadoras, como salários e outros rendimentos tributáveis.
-   **Controle de Operações em Renda Variável:** Módulo para lançamento de notas de corretagem, detalhando operações de compra e venda de ativos na bolsa de valores.

---

## 📂 Estrutura da Planilha

A ferramenta é dividida em abas (planilhas) principais, cada uma com uma finalidade específica.

### 👤 **TITULAR**

Nesta aba, o usuário insere suas informações cadastrais básicas. É o ponto de partida para a organização.

| Coluna  | Descrição                                 |
| :------ | :---------------------------------------- |
| `NOME`  | Nome completo do titular da declaração.   |
| `CPF`   | CPF do titular.                           |
| `BANCO` | Banco principal para referência.          |
| `AG`    | Agência bancária.                         |
| `CONTA` | Número da conta corrente.                 |

<br/>

### 📄 **INFORMES**

Destinada ao registro dos dados contidos nos **Informes de Rendimentos** fornecidos pelas fontes pagadoras.

| Coluna             | Descrição                                                 |
| :----------------- | :-------------------------------------------------------- |
| `CPF/CNPJ FONTE`   | CPF ou CNPJ da fonte pagadora.                            |
| `NOME FONTE`       | Nome da empresa ou pessoa que realizou o pagamento.       |
| `REND. TRIBUTÁVEL` | Total de rendimentos tributáveis recebidos.               |
| `IMPOSTO RETIDO`   | Valor do imposto de renda retido na fonte (IRRF).         |
| `13° SALÁRIO`      | Valor recebido a título de 13º salário.                   |
| `IRRF s/ 13°`      | Imposto de renda retido na fonte sobre o 13º salário.     |

<br/>

### 📈 **NOTAS**

Essencial para quem investe em renda variável. Aqui são lançadas as informações das **Notas de Corretagem**.

| Coluna      | Descrição                                                 |
| :---------- | :-------------------------------------------------------- |
| `DATA`      | Data em que a operação foi realizada (formato `DD/MM/AAAA`).|
| `NOTA`      | Número da nota de corretagem.                             |
| `OPERAÇÃO`  | Tipo de operação: `COMPRA` ou `VENDA`.                    |
| `TICKER`    | Código do ativo negociado (ex: `PETR4`, `ITUB3`).         |
| `QUANTIDADE`| Quantidade de ativos negociados.                          |
| `PREÇO`     | Preço unitário do ativo na operação.                      |
| `CUSTOS`    | Custos operacionais (taxas de corretagem, emolumentos, etc.).|
| `TOTAL`     | Valor total da operação (`Quantidade * Preço +/- Custos`).|

<br/>

### 🗂️ **TABELAS**

Esta é uma aba de apoio que serve como "banco de dados" para as demais. Ela contém listas utilizadas para as funções de validação de dados, garantindo consistência e agilidade no preenchimento.
* `LISTA DE BANCOS`
* `TICKERS B3`
* `CORRETORAS`

---

## 🚀 Como Utilizar

1.  **Faça o download** do arquivo `lion_app_irpf.xlsx`.
2.  **Abra** o arquivo no Microsoft Excel.
3.  **Comece pela aba `TITULAR`** e preencha suas informações pessoais.
4.  **Navegue para a aba `INFORMES`** para cadastrar os rendimentos recebidos ao longo do ano-base.
5.  **Utilize a aba `NOTAS`** para registrar todas as suas operações na bolsa de valores, com base nas notas de corretagem.
6.  Ao final do período, utilize os dados consolidados na planilha como guia para preencher sua declaração oficial no programa da Receita Federal.

## 🛠️ Tecnologias e Ferramentas

-   **Microsoft Excel:**
    -   Fórmulas (`SOMA`, `SE`, etc.)
    -   Validação de Dados
    -   Formatação Condicional
    -   Hiperlinks para navegação

## 🎓 Objetivos de Aprendizagem Alcançados

-   Aplicação de conceitos de organização de dados em um ambiente prático e de relevância real.
-   Criação de documentação técnica clara e estruturada para um projeto.
-   Utilização do GitHub para compartilhar e documentar a evolução do projeto.