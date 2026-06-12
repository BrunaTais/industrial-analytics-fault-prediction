# 🏭 Analytics para Manutenção Industrial e Falhas Elétricas

## 🎯 Contexto e Objetivos do Caderno de Estudos
O objetivo deste projeto, desenvolvido para o desafio da DIO, é aplicar a Inteligência Artificial (NotebookLM) como uma ferramenta de aprendizagem ativa para acelerar minha transição de carreira para a área de Dados. 

Como meu background é em Engenharia Elétrica e Planejamento Industrial (PPCM), escolhi o tema **Analytics Industrial focado em Previsão de Falhas Elétricas**. O objetivo do caderno é mapear como transformar dados brutos de sensores e logs de chão de fábrica em insights estratégicos de negócios, unindo minha experiência técnica anterior com as novas habilidades em dados.

---

## 📚 Curadoria de Fontes Selecionadas
Para alimentar a inteligência do meu caderno de estudos, selecionei as seguintes referências e conceitos de mercado:
1. **Os 5 Domínios da Transformação Digital (David Rogers):** Adaptados para o cenário de manutenção (Clientes, Competição, Dados, Inovação e Valor).
2. **Metodologia DB-SMigra & ISO 31000:** Focadas em governança, qualidade de dados e mitigação de riscos na migração de dados industriais legados.
3. **Guias Práticos de SQL e Python para EDA (Análise Exploratória de Dados):** Focados no tratamento de inconsistências e desduplicação de registros de telemetria de sensores.

---

## 🧠 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Durante as interações com a IA para estruturar este plano de analytics, documentei os testes de abordagens:

### ❌ Prompt Fraco (Tentativa Inicial)
*   **Comando:** *"Me dê ideias de projetos de dados para quem é engenheiro."*
*   **Resultado:** A IA trouxe exemplos genéricos (previsão de preço de casas, análise de vendas de mercado) que não aproveitavam minha senioridade.

###  Prompt Forte (Abordagem Especialista)
*   **Comando:** *"Atue como um Especialista Sênior em Analytics Industrial. Crie um roteiro de projeto de portfólio que utilize SQL, Python e Power BI para resolver o problema de paradas não planejadas por falhas elétricas, aplicando o workflow DB-SMigra e os princípios de gestão de riscos da ISO 31000."*
*   **Resultado:** Excelente. A IA estruturou um roteiro rigoroso dividindo as fases em Engenharia (SQL), Processamento (Python) e Storytelling de Negócio (Power BI), que é o que utilizarei como guia de portfólio.

---

## 📖 Miniguia de Estudo e Execução do Protótipo (Entrega Final)

### 1. Resumo Estruturado das Etapas Técnicas
*   **SQL (Ingestão):** O foco é garantir a integridade. Usarei consultas com `COUNT(*)` para validar tuplas entre sistemas e `LEFT JOIN` para rastrear registros órfãos em logs de falhas.
*   **Python (Limpeza):** Tratamento de ruídos e dados nulos de sensores utilizando Pandas, validando se picos de corrente elétrica coincidem com os logs reais de erro.
*   **Power BI (Visualização):** Criação de um dashboard com duas camadas (Executiva para métricas de negócio como MTBF e Técnica para drill-down de sensores).

### 2. Glossário de Conceitos Aprendidos

| Termo Técnico | Significado no Contexto Industrial |
| :--- | :--- |
| **MTBF (Mean Time Between Failures)** | Tempo Médio Entre Falhas. Métrica crítica para medir a confiabilidade do ativo. |
| **Workflow DB-SMigra** | Processo estruturado para migração e garantia de qualidade de dados entre bancos. |
| **Registros Órfãos** | Dados de falhas ou eventos que perderam a referência do ativo correspondente no sistema. |
| **EDA (Exploratory Data Analysis)** | Análise Exploratória de Dados. Fase no Python para descobrir padrões de falhas elétricas. |

### 3. Prompts Reutilizáveis para Próximas Fases
*   *“Gere uma tabela de dados fictícios em formato CSV simulando 100 linhas de leituras de sensores de corrente e temperatura com algumas falhas para eu treinar no Python.”*
*   *“Escreva uma query em PostgreSQL para calcular o MTBF de um grupo de motores elétricos com base em uma tabela de eventos.”*
