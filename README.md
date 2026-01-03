# 📊 Simulador de Investimentos – Planilha Financeira

Este projeto consiste em uma **planilha de simulação de investimentos** desenvolvida para auxiliar usuários na **análise e tomada de decisão financeira**, por meio da projeção do crescimento patrimonial ao longo do tempo com aportes recorrentes, rendimentos e dividendos.

---

## 🎯 Objetivo

Fornecer uma ferramenta simples, clara e estruturada que permita:
- Simular diferentes cenários de investimento;
- Avaliar o impacto de aportes mensais;
- Estimar crescimento patrimonial;
- Visualizar a geração de renda passiva (dividendos).

A planilha automatiza cálculos financeiros recorrentes, reduzindo erros manuais e aumentando a confiabilidade da análise.

---

## 🗂️ Estrutura do Projeto

A planilha é composta por **três abas principais**, cada uma com uma função específica:

### 1️⃣ Parametros
Aba destinada exclusivamente à **entrada de dados do usuário**.

**Campos disponíveis:**
- Patrimônio Inicial  
- Aporte Mensal  
- Taxa de Retorno Mensal (%)  
- Dividend Yield Mensal (%)  
- Meses de Simulação  

> ⚠️ Recomenda-se alterar apenas esta aba para simular novos cenários.

---

### 2️⃣ Projecao
Aba responsável pela **simulação financeira mês a mês**.

**Principais informações calculadas:**
- Saldo inicial de cada mês
- Aportes mensais
- Rendimentos
- Dividendos
- Saldo final acumulado
- Total investido ao longo do tempo

As fórmulas são automaticamente ajustadas ao se estender a simulação para novos meses.

---

### 3️⃣ Resumo
Aba de **consolidação gerencial**, voltada para análise rápida.

**Indicadores apresentados:**
- Total investido no período
- Patrimônio final estimado
- Dividendos médios mensais

Ideal para comparação entre cenários e avaliação estratégica.

---

## ⚙️ Funcionamento do Modelo

1. O usuário informa os dados na aba **Parametros**  
2. A aba **Projecao** realiza automaticamente os cálculos mensais  
3. A aba **Resumo** consolida os principais resultados  
4. Alterações nos parâmetros recalculam toda a simulação em tempo real  

---

## 📐 Fórmulas Utilizadas (Visão Geral)

- **Rendimento Mensal**
- 
- **Dividendos Mensais**  

- **Saldo Final**  

- **Total Investido**  

---

## 🧩 Compatibilidade

- Microsoft Excel (PT-BR e EN-US)
- Google Sheets
- LibreOffice Calc

> Funções utilizadas: `MAX`, `AVERAGE`

---

## ⚠️ Limitações

- Não considera inflação
- Não considera impostos ou taxas
- Assume taxas constantes ao longo do período
- Dividendos não são reinvestidos automaticamente

---

## 🚀 Possíveis Evoluções

- Inclusão de inflação e tributação
- Reinvestimento automático de dividendos
- Comparação entre múltiplos cenários
- Gráficos automáticos de evolução patrimonial
- Conversão cambial (ex.: dólar)

---

## 👤 Público-Alvo

- Investidores iniciantes e intermediários
- Estudantes de finanças e economia
- Planejamento financeiro pessoal
- Uso acadêmico ou corporativo


---

## 📌 Conclusão

Esta planilha oferece uma solução prática e eficiente para simular investimentos, permitindo ao usuário compreender como aportes, tempo e rentabilidade impactam o crescimento patrimonial e a geração de renda passiva.

---

