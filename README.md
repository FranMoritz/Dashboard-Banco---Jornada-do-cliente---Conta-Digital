# Dashboard-Banco---Jornada-do-cliente---Conta-Digital

Análise da Jornada de Abertura de Conta Digital
Entendendo atritos, otimizando etapas críticas e destravando conversão em um banco digital

Visão Geral

Este projeto simula a jornada completa de abertura de conta em um banco digital, identificando pontos de atrito, analisando segmentos críticos e aplicando testes A/B para melhorar a conversão.

A iniciativa nasce do desafio enfrentado pelo Head de CX, André Duarte, que precisava aumentar a aprovação de novas contas em 20% no próximo trimestre. Para isso, foi desenvolvido um dashboard executivo e um conjunto de análises baseadas em dados reais da jornada.

O objetivo final é revelar onde o funil estava “sangrando”, propor melhorias estruturadas e medir o impacto financeiro de cada intervenção.

Objetivos do Projeto

Mapear a jornada completa de abertura de conta digital

Identificar etapas com maior abandono

Analisar segmentos mais sensíveis ao atrito

Construir testes A/B estruturados

Medir significância estatística (p-value)

Simular impacto financeiro das melhorias

Criar um dashboard executivo no Looker Studio

Dataset

O projeto utiliza dados sintéticos gerados especificamente para simular:

Eventos da jornada do cliente (eventos por etapa)

Tabela agregada de funil

Tabela de segmentação

Testes A/B

Uplift e impacto financeiro

Principais arquivos do projeto
Arquivo	Descrição
journey_events.csv	Eventos da jornada (etapas, abandono, timestamps)
journey_summary.csv	Tabela consolidada por usuário/jornada
funnel_dashboard.csv	Funil agregado para visualizações
seg_income_dashboard.csv	Conversão por faixa de renda
seg_channel_dashboard.csv	Conversão por canal de aquisição
seg_device_dashboard.csv	Conversão por dispositivo
ab_custom_tests.csv	Resultados dos testes A/B
ab_uplift_dashboard.csv	Uplift das variantes
ab_consolidated.csv	Testes A/B + impacto financeiro

Metodologia
1. Construção da Árvore Lógica

Reunião colaborativa com stakeholders das áreas de Produto, CX, Marketing, Dados e Engenharia.
Hipóteses como problemas de UX, dificuldades de KYC, falhas técnicas e perfis de risco foram mapeadas.

2. Análise Exploratória

As primeiras análises mostraram abandonos críticos em:

onboarding_start

selfie_biometric

Segmentos mais impactados:

Classe média

Canal de aquisição "referência"

Dispositivos Android e acesso Web

3. Testes A/B

Foram criados dois experimentos principais:

Experimento: Onboarding Start

Variante A: formulário antigo

Variante B: formulário em formato de diálogo
➡ +7 p.p. de conversão (p < 0.001)

Experimento: Selfie Biométrica

Variante A: selfie sem instruções

Variante B: selfie com instruções claras
➡ +9 p.p. de conversão (p < 0.001)

4. Simulação Financeira

Cálculo de impacto:

Custo do atrito por etapa

Receita perdida acumulada

Receita adicional projetada com rollout das variantes vencedoras

Estimativa anualizada dos ganhos

Dashboard Executivo (thebricks)

O dashboard contém:

Visão Geral do Funil

KPIs: Iniciados, Aprovados, Taxa de Aprovação

Receita estimada e perdida

Funil completo

Conversão ao longo do tempo

Filtros por renda, canal, dispositivo, risco e data
