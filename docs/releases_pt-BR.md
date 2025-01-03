---
title: Release Notes (pt-BR)
nav_order: 2
---

# Versão 3.7.8

🔗 [Download](https://www.psr-inc.com/app/link/?t=d&f=nwsddp-3.7.8-setup.exe)

## Correções

- Corrige leitura da modificação tipo `VOLMIN` quando o volume mínimo especificado supera o volume máximo de cadastro da usina.


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