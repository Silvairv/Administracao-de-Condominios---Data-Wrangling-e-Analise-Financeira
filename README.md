# Administracao-de-Condomnios---Data-Wrangling-e-Analise-Financeira
Este projeto foca na aplicação de técnicas avançadas de Data Wrangling com a biblioteca Pandas para transformar dados imobiliários brutos e não estruturados em uma base de dados limpa e pronta para análises financeiras de inadimplência.

📌 Contexto do Projeto
O objetivo principal foi processar um ficheiro JSON complexo contendo informações de alugueres de um condomínio. O desafio consistiu em normalizar dados aninhados, tratar listas dentro de células e padronizar formatos de moeda e data para análise de métricas de pagamento.

🛠️ Tecnologias e Ferramentas
Linguagem: Python

Biblioteca Principal: Pandas (manipulação e transformação de dados)

Formatos de Dados: JSON e DataFrames estruturados

📈 Etapas do Pipeline de Dados
1. Extração e Normalização (ETL)
Carregamento de dados estruturados em JSON.

Utilização de json_normalize para transformar estruturas de dicionários aninhados em colunas de um DataFrame.

2. Tratamento de Estruturas Complexas
Implementação do método explode para desmembrar listas de datas e valores que estavam agrupadas em linhas únicas, garantindo que cada registo representasse um único evento de pagamento.

Reset de índices para garantir a integridade da navegação nos dados.

3. Limpeza e Tipagem de Dados (Data Cleaning)
Tratamento de Strings: Remoção de carateres especiais (como "$" e "reais") e substituição de vírgulas por pontos para conversão numérica.

Conversão de Tipos: Transformação de colunas de texto para float (valores financeiros) e datetime (datas de pagamento).

4. Análise de Inadimplência
Criação de métricas para identificar o atraso nos pagamentos comparando as datas combinadas com as datas efetivas.

Agrupamento de dados por unidade (apartamento) para identificar padrões de comportamento financeiro.

🚀 Como Executar o Projeto
Clone o repositório.

Certifique-se de ter o Python e a biblioteca Pandas instalados.

Execute o ficheiro Jupyter Notebook Projeto_Administracao_De_Condominios.ipynb.

🎯 Conclusão
Este projeto demonstra a capacidade de lidar com a etapa mais crítica da ciência de dados: a preparação de dados. A transformação de um JSON "sujo" numa tabela estruturada permite que a administração do condomínio tenha uma visão clara sobre o fluxo de caixa e a pontualidade dos inquilinos.

Desenvolvido por Gabriel Rodrigues (https://www.linkedin.com/in/gabriel-rodrigues5955/)
