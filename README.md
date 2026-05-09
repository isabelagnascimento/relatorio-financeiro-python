# 📊 Automação de Relatório Financeiro Corporativo

## 📝 Descrição do Projeto
Este projeto consiste em uma automação em Python para a geração de relatórios financeiros corporativos. O objetivo principal é otimizar rotinas administrativas extraindo dados reais da bolsa de valores e estruturando-os automaticamente.

Desenvolvido como parte de um estudo prático de programação e finanças, o sistema coleta o histórico de preços da ação da Petrobras (PETR4.SA), simula aportes mensais de investimentos e exporta uma planilha Excel pronta para uso. A grande vantagem é que a planilha já sai do código com dados tabelados e gráficos nativos embutidos.

<img width="626" height="308" alt="Captura de tela 2026-05-09 192023" src="https://github.com/user-attachments/assets/6df393d7-156f-4150-95fa-3d8f30ec0f40" />
*Figura 1: Gráfico do "Preço do Ativo" gerado automaticamente no Excel. Ele plota o histórico de preços reais baixado via API, permitindo visualizar a tendência do mercado no período analisado.*

<img width="625" height="307" alt="Captura de tela 2026-05-09 192009" src="https://github.com/user-attachments/assets/ce0bdb22-569a-4b0c-b9db-26620219c02b" />
Figura 2: Gráfico da "Evolução da Carteira". Note o padrão em "degraus" da linha: cada salto vertical representa visualmente o momento exato em que o algoritmo simulou um novo aporte financeiro (a cada 21 dias úteis), somado à valorização contínua do ativo.

## 🚀 Tecnologias Utilizadas
* ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) **Linguagem:** Python
* ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) **Manipulação de Dados:** Pandas, YFinance
* ![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white) **Geração de Relatórios:** OpenPyXL
* **Ambiente:** Google Colab / Jupyter Notebook

## 📊 Resultados e Aprendizados
O projeto demonstra a capacidade de integrar APIs externas de dados (Yahoo Finance) com a manipulação automatizada de arquivos de escritório.
* **Automação de Tarefas:** Aprendi a eliminar o trabalho manual de atualização diária ou mensal de planilhas de controle.
* **Tratamento de Dados:** Prática na limpeza de dados financeiros, como a remoção de índices duplos (MultiIndex) utilizando a biblioteca Pandas.
* **Integração com Excel via Código:** Geração de gráficos de linha nativos do Excel diretamente via script Python, uma habilidade muito valorizada no mercado corporativo.

## 🔧 Como Executar
1. Clone o repositório ou baixe o arquivo `.ipynb`.
2. Em um ambiente Python (como o Google Colab), instale as dependências: `!pip install pandas openpyxl yfinance`.
3. Execute o código completo.
4. O arquivo `relatorio_financeiro.xlsx` será gerado e baixado automaticamente com os dados atualizados.
