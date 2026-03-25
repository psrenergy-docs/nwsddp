---
title: Release Notes (pt-BR)
nav_order: 2
---

# Versão 3.7.20

🔗 [Download](https://www.psr-inc.com/app/link/?t=d&f=nwsddp-3.7.20-setup.exe)


## Atualizações

- Adiciona MDC para PMO 2026/02+.

- Converte dados do ADTERM - termicas must-run criadas para representar periodo de lag com geração forçada.

## Correções

- Corrige conversão das restrições elétricas (restricoes-eletricas.csv):

  - Considera a duração dos patamares no cálculo do limite.


# Versão 3.7.19

🔗 [Download](https://www.psr-inc.com/app/link/?t=d&f=nwsddp-3.7.19-setup.exe)

## Correções


- Corrige conversão das restrições elétricas (restricoes-eletricas.csv):

  - Considera o sentido da interconexão ao definir os coeficientes da restrição genérica;

  - Considera o valor médio dos patamares na definição dos limites.



# Versão 3.7.17

🔗 [Download](https://www.psr-inc.com/app/link/?t=d&f=nwsddp-3.7.17-setup.exe)

## Correções

- Corrige conversão de dados de irrigação e consideração da irrigação definida no arquivos de modificação de cadastro.


# Versão 3.7.15

## Atualizações

- Opção de corrigir vazões incrementais negativas utilizando o histórico completo selecionada por padrão.


# Versão 3.7.14

## Correções

- Corrige conversão de dados de irrigação.
- Corrige leitura dos dados de irrigação do PDE34.

## Atualizações

- Opção de correção de vazões negativas considerando o histórico completo ativada por padrão.


# Versão 3.7.13

## Correções

- Corrige a leitura de `restricao-eletrica.csv` com encoding UTF-8 e caracteres acentuados.


# Versão 3.7.12

🔗 [Download](https://www.psr-inc.com/app/link/?t=d&f=nwsddp-3.7.12-setup.exe)

## Atualizações

- Adiciona MDC para PMO 2025/03.


# Versão 3.7.11

## Correções

- Corrige erro na leitura do arquivo clast na etapa de patch.


# Versão 3.7.10

## Atualizações

- Adiciona MDC para PMO 2025/02.


# Versão 3.7.8

## Correções

- Corrige leitura da modificação tipo `VOLMIN` quando o volume mínimo especificado supera o volume máximo de cadastro da usina.

- Correção na leitura de modificações `VOLCOTA` e `COTAREA` para aceitar comprimento variavel.

- Correção nos limites das restrições elétricas.

## Atualizações

- Adiciona MDC para PMO 2025/01.


# Versão 3.7.7

## Correções

- Corrige leitura da modificação `VOLCOTA` de hidrelétricas.


# Versão 3.7.6

## Correções

- Correção na leitura de dados de sistemas e classe de combustíveis de casos PDE.


# Versão 3.7.5

## Atualizações

- Altera opções default do SDDP para que se utilizem todos os blocos na política.
- Correção na falta do indices.csv.


# Versão 3.7.4

## Atualizações

- Suporte ao novo formato de restrições elétricas - convertidas em restrições genéricas.
- Suporte ao novo formato de polinomio de jusante - entretanto ainda não utilizadas.
- Suporte a modificação de turbinamento mínimo e máximo TURBMINT/TURBMAXT.
- Por padrão irá corrigir todo o histórico de vazões.


# Versão 3.7.3

## Correções

- Correção na leitura de caso.dat.
- Correção na leitura do CONFT.dat quando houver usinas tipo NC.
- Atualização do MDC para PMO 2024/05 com anos adicionais de Belo Monte.


# Versão 3.7.2

## Correções

- Aumenta o número de cargas adicionais para 30.


# Versão 3.7.1

## Correções

- Aumenta número máximo de anos para 30.


# Versão 3.7.0

## Correções

- Corrige bug na conversão de preços de combustível quando o ultimo mês está em branco

- Corrige erro na leitura de modificações `COTAREA`

- Corrige erro na leitura de modificações de preço de combustível com valor igual a `0`

- Corrige capacidade instalada inicial de térmicas (`cterm*.dat`) quando há expansão.


# Versão 3.6.17

## Correções

* Corrige bug na geração de custos de combustíveis quando mês final no clast está em aberto.

* Corrige erro ao ler modificação `COTAREA`

* Corrige erro ao ler modificaçao de custo de combustível com valor `0`

* Corrige potencia instalada de cadastro de usina térmica (`cterm*.dat`) com expansão.


## Atualizações

* Adiciona opção para leitura dos polinomios de jusante do decomp (`polinjus.dat`)

* Adiciona opção para utilizar dados de fator de capacidade instalada de renováveis configurado no MDC.

* Adiciona arquivo de modificação de cadastro do PMO de maior de 2024.