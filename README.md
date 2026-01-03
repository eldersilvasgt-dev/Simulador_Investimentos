# 📊 Simulador de Investimentos – Planilha Financeira

Este projeto é uma planilha de simulação de investimentos desenvolvida para auxiliar usuários na análise e tomada de decisão financeira, por meio da projeção do crescimento patrimonial mês a mês a partir de aportes e rentabilidade.

---

## Índice
- [Objetivo](#objetivo)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Parâmetros (Entrada)](#parâmetros-entrada)
- [Projeção (Cálculos)](#projeção-cálculos)
- [Resumo (Indicadores)](#resumo-indicadores)
- [Fórmulas Utilizadas (Visão Geral)](#fórmulas-utilizadas-visão-geral)
- [Compatibilidade](#compatibilidade)
- [Limitações](#limitações)
- [Evoluções Possíveis](#evoluções-possíveis)
- [Exemplo Rápido](#exemplo-rápido)
- [Contribuição e Licença](#contribuição-e-licença)

---

## 🎯 Objetivo

Fornecer uma ferramenta simples, clara e estruturada que permita:
- Simular diferentes cenários de investimento;
- Avaliar o impacto de aportes regulares;
- Estimar o crescimento patrimonial ao longo do tempo;
- Visualizar geração de renda passiva (dividendos).

A planilha automatiza cálculos financeiros recorrentes, reduzindo erros manuais e melhorando a confiabilidade da análise.

---

## 🗂️ Estrutura do Projeto

A planilha contém três abas principais:

### 1️⃣ Parâmetros (entrada)
Aba destinada exclusivamente à entrada de dados do usuário.

Campos recomendados:
- Patrimônio Inicial (valor monetário)
- Aporte Mensal (valor monetário)
- Taxa de Retorno Mensal (%) — taxa média de valorização mensal
- Dividend Yield Mensal (%) — rendimento por dividendos em % ao mês
- Meses de Simulação (inteiro)

Observação: mantenha apenas esta aba para alterar cenários; as demais abas usam referências para recalcular automaticamente.

---

### 2️⃣ Projeção
Aba que realiza a simulação mês a mês com as colunas típicas:
- Mês / Período
- Saldo Inicial do mês
- Aporte Mensal
- Rendimentos (juros/valorização)
- Dividendos
- Saldo Final do mês
- Total Investido acumulado

As fórmulas devem ser arrastadas/estendidas para cobrir o número de meses desejado.

---

### 3️⃣ Resumo
Aba consolidada com os principais indicadores:
- Total investido no período
- Patrimônio final estimado
- Dividendos médios mensais
- Rentabilidade média do período

Útil para comparar cenários e para relatórios rápidos.

---

## 📐 Fórmulas Utilizadas (Visão Geral)

As fórmulas abaixo assumem que as percentagens estão no formato porcentagem mensal (ex.: 1% = 1.0).

- Rendimento Mensal:
  - rendimento = saldo_inicial * (taxa_retorno_mensal / 100)

- Dividendos Mensais:
  - dividendos = saldo_inicial * (dividend_yield_mensal / 100)

- Saldo Final do Mês:
  - saldo_final = saldo_inicial + aporte_mensal + rendimento + dividendos

- Saldo Inicial do Próximo Mês:
  - saldo_inicial_prox = saldo_final

- Total Investido (acumulado):
  - total_investido = patrimonio_inicial + aporte_mensal * número_de_meses_realizados

Observações:
- Se desejar que dividendos sejam reinvestidos, ajuste a ordem (somar dividendos ao saldo antes do cálculo do rendimento do mês seguinte ou reinvestir imediatamente no aporte).
- Se taxas foram informadas em termos anuais, converta para mensal: taxa_mensal ≈ (1 + taxa_anual)^(1/12) - 1.

---

## 🧩 Compatibilidade

- Microsoft Excel (PT‑BR e EN‑US)
- Google Sheets
- LibreOffice Calc

Funções utilizadas (exemplos): `MAX`, `AVERAGE`, operações aritméticas e referências relativas/absolutas.

---

## ⚠️ Limitações

- Não considera inflação;
- Não considera impostos (IR) ou taxas de corretagem/gestão;
- Assume taxas constantes ao longo do período (sem volatilidade);
- Dividendos não são reinvestidos por padrão (a menos que ajuste na planilha seja feito);
- Não há tratamento automático de fechamento de mercado, dividendos extraordinários ou eventos corporativos.

---

## 🚀 Possíveis Evoluções

- Inclusão de inflação e tributação (simulação de IR sobre ganhos e dividendos);
- Reinvestimento automático de dividendos (opção ON/OFF);
- Comparação entre múltiplos cenários lado a lado;
- Gráficos automáticos de evolução patrimonial e rendimento;
- Conversão cambial (ex.: ativos em dólar);
- Simulação com séries históricas de rentabilidade (volatilidade) para Monte Carlo.

---

## 🧪 Exemplo Rápido

Parâmetros:
- Patrimônio Inicial: R$ 10.000,00  
- Aporte Mensal: R$ 500,00  
- Taxa de Retorno Mensal: 1,0 (%)  
- Dividend Yield Mensal: 0,3 (%)  
- Meses: 12

Cálculo do primeiro mês (exemplo):
- rendimento = 10.000 * 0,01 = 100,00  
- dividendos = 10.000 * 0,003 = 30,00  
- saldo final = 10.000 + 500 + 100 + 30 = 10.630,00

---

## 🤝 Contribuição e Licença

Contribuições são bem‑vindas — abra uma issue para discutir mudanças ou um pull request com a melhoria. Inclua exemplos e screenshots quando possível.

Sugestão: adicionar um arquivo LICENSE (ex.: MIT) e um CONTRIBUTING.md com orientações de como colaborar.

---

## Contato

Se precisar de ajuda para adaptar a planilha ao seu caso (reinvestimento, impostos ou simulações avançadas), abra uma issue ou me envie uma mensagem pelo repositório.

---
