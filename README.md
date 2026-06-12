# PINGO - Sistema Inteligente de Reuso e Tratamento de Águas Cinzas 

> Trabalho Prático desenvolvido para a disciplina de **Projeto Integrador I (PI1)** do curso de **Ciência da Computação**.  
> **Status do Projeto:** Em conformidade com os entregáveis da Unidade 4 (Mapeamento Analítico e Interface Funcional).

---

## 📌 Contextualização do Projeto

O ecossistema **PINGO** nasce com o objetivo de atenuar o desperdício de água potável no ecossistema residencial através do reaproveitamento estratégico de águas cinzas geradas por máquinas de lavar roupas. O projeto integra automação de hardware (válvulas solenoides e sensores de nível acoplados ao ecossistema Arduino/ESP32) com uma plataforma digital inteligente.

Este repositório armazena as soluções de interface web desenvolvidas para suprir as exigências de **Engenharia de Usabilidade (UX/UI)** e **Fundamentação Teórica de Dados (ETL Industrial)** mapeadas nas unidades anteriores.

---

## 📂 Estrutura de Arquivos e Componentes

O repositório está dividido em dois módulos principais de simulação e análise. Ambos foram construídos utilizando tecnologias web padrão para fácil portabilidade.

### 1. `app_dashboard.html` (Dashboard Simulador do Aplicativo)
* **Objetivo:** Demonstrar de forma prática e interativa a experiência do usuário final (**Persona**) concebida no estudo de caso de UX/UI.
* **Funcionalidades:**
  * Simulação em tempo real do volume acumulado de litros salvos.
  * Cálculo dinâmico do **ROI (Retorno sobre o Investimento)** financeiro baseado na configuração de reuso ativa.
  * Feedback imediato do status do hardware simulado (Válvula solenoide Aberta/Fechada, Nível da Boia e Contagem de fluxo de enxágue).
  * Regra de negócio integrada que filtra os fluxos, ignorando o 1º ciclo (alta sujidade de sabão).

### 2. `dashboard_etl.html` (Dashboard de Fundamentação Teórica e ETL)
* **Objetivo:** Fornecer à banca do projeto a validação empírica da necessidade da nossa solução baseada em dados nacionais reais.
* **Funcionalidades:**
  * Renderização robusta e dinâmica do **Top 10 Municípios Brasileiros com Maior Captação de Água Industrial** (Dados reais processados pelo nosso pipeline Python Pandas no script de ETL).
  * Utilização da biblioteca analítica **Chart.js** via CDN.
  * Filtro interativo por região geográfica (Ex: Isolar Polos do Sudeste vs Outras Regiões).
  * Gráfico de balanço volumétrico nacional, ilustrando o gap de água que é captada mas não retorna tratada, validando o modelo de mercado do PINGO.

---

## Como Executar os Projetos

Por serem aplicações puramente *Client-Side* estruturadas em HTML5, CSS3 e JavaScript Moderno, **não é necessário instalar nenhuma dependência ou servidor local**.

1. Faça o clone deste repositório para a sua máquina local:
   ```bash
   git clone [https://github.com/seu-usuario/pingo-projeto-integrador-1.git](https://github.com/seu-usuario/pingo-projeto-integrador-1.git)
