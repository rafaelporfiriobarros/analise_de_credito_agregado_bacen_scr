# SCR.data - Dados Agregados de Crédito do Banco Central

![Banco Central do Brasil](https://ww2.gestaoni.com.br/painel/storage/031220165128c47532bbb1e2883c902071591ae1ec9b/img_site/g/73f6914fd787c369ac5f8bdda6c72904.jpg)

Repositório de documentação e apoio ao uso dos dados agregados disponibilizados pelo **Banco Central do Brasil** por meio do sistema **SCR.data** (Sistema de Informações de Crédito). Este material é útil para análises estatísticas, estudos econômicos, construção de dashboards e desenvolvimento de modelos relacionados ao mercado de crédito.

---

## Introdução

O **Banco Central do Brasil** divulga mensalmente dados agregados de operações de crédito recebidas através do documento 3040 do Sistema de Informações de Crédito – **SCR**. As informações são atualizadas no último dia útil do mês, com dados referentes a até 60 dias antes da data de publicação.

### Disponibilizações:
- Carteira Ativa
- Inadimplência
- Ativo Problemático

Com detalhamento por:
- Tipo de cliente (PF/PJ)
- Modalidade de crédito
- Unidade da federação
- CNAE (PJ) ou natureza da ocupação (PF)
- Porte/rendimento
- Origem de recursos
- Indexador da operação

Período: **Junho de 2012 até a atualidade**

**Observação:** Os dados do SCR podem divergir de outras fontes do BCB, como o SGS e notas para imprensa. A razão principal está na granularidade e origem das informações.

---

## Conceitos

### Escopo
Abrange operações de crédito acima de R$1.000 (até mai/2016) ou acima de R$200 (a partir de jun/2016), cursadas no Brasil, reportadas por instituições obrigadas a enviar o documento 3040.

### Carteira
Soma dos valores a vencer e vencidos (modalidades 01 a 13).

### Inadimplência
Proporção de operações com parcelas vencidas há mais de 90 dias sobre o total da carteira.

### Ativo Problemático
Operações com atraso > 90 dias ou com indícios de não pagamento (ex: reestruturação com classificação de risco E a H).

---

## Gráficos Interativos (BCB)

Disponibilizados no [portal oficial do SCR.data](https://www3.bcb.gov.br/ifdata/), os gráficos permitem segmentações por:

- **Período**
- **Tipo de cliente**: PF / PJ
- **Modalidade**: Cartão, Consignado, Capital de Giro, Investimento, etc.
- **UF**
- **CNAE (PJ)** ou **Natureza de ocupação (PF)**
- **Porte dos clientes**
- **Origem dos recursos**
- **Indexador da operação**

> 📌 Para equivalência entre as modalidades do relatório e o layout oficial do SCR, acesse:  
> [Equivalência de Modalidades - SCR vs SCR.data](https://www.bcb.gov.br/content/estabilidadefinanceira/Leiaute_de_documentos/scrdoc3040/Equivalencia_Modalidades.xlsx)

---

## Campos Disponíveis no Portal de Dados Abertos

O Banco Central também fornece os dados em formato tabular (CSV), permitindo análises mais robustas e automatizadas. Os campos incluem:

### Tipo de Consolidado Bancário (TCB)
- Bancário
- Não bancário
- Cooperativas

### Segmento (Resolução nº 4.553/2017)
- S1 a S5 (por porte e tipo de instituição)

### Tipo de Cliente
- Pessoas Físicas
- Pessoas Jurídicas

### Modalidade de Crédito
- Ex: PF - Cartão de Crédito, PJ - Capital de Giro, PJ - Comércio Exterior etc.

### UF
- Total nacional + 27 unidades da federação (base: CEP da residência/sede)

### 👷 Natureza da Ocupação (PF)
- Servidor público, Autônomo, Empresário, MEI, etc.

### 🏭 CNAE (PJ)
- Disponível até o nível de **subclasse (7 dígitos)**

### 💼 Porte dos Clientes
#### PF:
- Faixas de salários mínimos (de "sem rendimento" até "acima de 20 SM")

#### PJ:
- Micro, Pequeno, Médio, Grande

### Origem dos Recursos
- Com ou sem destinação específica

### Indexador da Operação
- Prefixado, Pós-fixado, Índices de preços, TRFC/TCR, etc.

---

## 🔗 Links úteis

- 📄 [Leiaute do SCR (documento 3040)](https://www.bcb.gov.br/estabilidadefinanceira/scrdoc3040)
- 📊 [Portal IF.data](https://www3.bcb.gov.br/ifdata/)
- 📂 [Portal de Dados Abertos - BCB](https://dadosabertos.bcb.gov.br/)
- 🗂️ [Equivalência Modalidades SCR.data vs SCR](https://www.bcb.gov.br/content/estabilidadefinanceira/Leiaute_de_documentos/scrdoc3040/Equivalencia_Modalidades.xlsx)

---

## Possibilidades de uso

- Estudos de inadimplência
- Modelagem de crédito
- Análises de carteira ativa por região
- Segmentação por perfil de cliente
- Avaliação de impacto de políticas públicas no crédito
- Monitoramento do sistema financeiro nacional

---

## Licença

Os dados utilizados neste repositório são de domínio público, conforme disponibilização oficial do Banco Central do Brasil. Este projeto é livre para fins educacionais e analíticos.

---

