# CS2 Match Analytics: De CSVs Brutos a Insights Estratégicos


Neste projeto, aceitei o desafio de construir um pipeline de dados completo "end-to-end", desde a ingestão de arquivos brutos até a entrega de um dashboard de alta fidelidade. Utilizei um dataset do Kaggle contendo o histórico de partidas profissionais do portal HLTV.org, unindo minha paixão por análise de dados ao cenário competitivo de Counter-Strike.


# 🛠️ Stack Tecnológica Linguagem: Python (Pandas) para ETL e automação.

Banco de Dados: SQLite (Modelo Relacional) para persistência e integridade.

Visualização: Power BI (DAX & Power Query).

Integração: Driver ODBC para conectividade de banco de dados.


# 🏗️ Arquitetura do Projeto Fase 1: ETL e Higienização de Dados (Python) Ao iniciar, identifiquei desafios comuns em dados reais: registros despadronizados, informações redundantes e inconsistências de tipos.

Ação: Desenvolvi scripts em Python para realizar a limpeza pesada, filtragem de colunas irrelevantes e padronização de nomenclaturas.

Refinamento: Utilize o Power Query para transformações granulares de última milha, garantindo que o dataset estivesse pronto para modelagem.


# Fase 2: Modelagem e Integração SQL Para garantir a escalabilidade e integridade, migrei os dados dos CSVs para um banco de dados SQL relacional.

Relacionamentos: Estruturei as tabelas de Resultados e Picks/Bans conectadas via match_id.

Conectividade: Implementei a integração entre o banco de dados e o Power BI utilizando o protocolo ODBC, superando o desafio de importar dados de fontes relacionais locais.


# Fase 3: Analytics e Visualização (DAX & UI) O foco final foi transformar dados em decisões estratégicas.

Cálculos Avançados: Desenvolvi fórmulas DAX complexas para calcular a eficácia de vitórias em mapas escolhidos (Picks) e identificar o "Fator Zebra" (correlação entre Rank e resultado).

UI/UX: Elaborei um design customizado com o tema "Dark & Orange", utilizando as cores paleta oficial do CS para proporcionar uma experiência imersiva e profissional.

# 🧠 Troubleshooting & Lições Aprendidas Desafio: Conflito de tipos de dados (Texto vs Inteiro) na comparação de vencedores durante o cálculo de performance.

Solução: Implementação das funções FORMAT e VALUE no DAX para padronização de tipos em tempo de execução, garantindo a precisão das colunas calculadas e evitando erros de processamento no modelo.

📊 Visualização do Projeto

![Demonstração do Dashboard](C:\databases\csgo_proMatches\visuals\FinalProjeto.png)
