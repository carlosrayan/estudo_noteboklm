# estudo_noteboklm
Corrida para iniciantes


<div align="center">

# 🏃‍♂️ Caderno de Estudos: Corrida de Rua para Iniciantes com NotebookLM

![GitHub](https://img.shields.io/badge/Project-NotebookLM-blue?style=for-the-badge&logo=google)
![Topic](https://img.shields.io/badge/Topic-Corrida%20de%20Rua-brightgreen?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge)

<p align="center">
  Projeto de curadoria, síntese de conhecimento e engenharia de prompts aplicada à ciência esportiva e corrida de rua, utilizando LLMs com Grounding no Google NotebookLM.
</p>

</div>

---

## 📑 Sumário

- [1. Contexto e Objetivos](#1-contexto-e-objetivos)
- [2. Curadoria de Fontes](#2-curadoria-de-fontes)
- [3. Engenharia de Prompts e Cicatrizes (Troubleshooting)](#3-engenharia-de-prompts-e-cicatrizes-troubleshooting)
- [4. Miniguia de Estudo (Entrega Final)](#4-miniguia-de-estudo-entrega-final)
  - [4.1 Resumo Estruturado do Assunto](#41-resumo-estruturado-do-assunto)
  - [4.2 Glossário de Conceitos-Chave](#42-glossário-de-conceitos-chave)
  - [4.3 Prompts Reutilizáveis](#43-prompts-reutilizáveis)
- [5. Conclusão e Próximos Passos](#5-conclusão-e-próximos-passos)

---

## 1. Contexto e Objetivos

* **Assunto Escolhido:** Corrida de rua para iniciantes — transição estruturada do sedentarismo e da caminhada até a conclusão dos primeiros 5 km e progressão técnica (meta sub-30 minutos), integrando biomecânica, prevenção de lesões ortopédicas e estratégias de nutrição esportiva.
* **Objetivos de Estudo:**
  1. Compreender o processo de adaptação cardiovascular e musculoesquelética para corredores iniciantes de forma progressiva e segura.
  2. Mapear os erros técnicos e biomecânicos mais frequentes (ex.: *overstriding*, cadência baixa e sobrecarga tibial/canelite) e desenhar rotinas preventivas de fortalecimento e educativos.
  3. Estruturar uma base consistente de treinos (planilhas de caminhada/corrida, treinos regenerativos e controle de ritmo/pace) respaldada por literatura técnica e fisiologia do exercício.
  4. Documentar o processo prático de **Engenharia de Prompts com Grounding** no Google NotebookLM, evidenciando como ancorar respostas de inteligência artificial em fontes confiáveis e contornar limitações de contexto.

---

## 2. Curadoria de Fontes

Foram selecionadas e organizadas no caderno fontes abertas contemplando literatura acadêmica, medicina esportiva, portais técnicos e guias de treinamento:

| # | Fonte / Autor | Título do Material | Foco Principal | Link de Acesso |
|---|---|---|---|---|
| **01** | **Repositório Institucional UFMG** | *Utilização do VO₂ máx e Limiar de Lactato como Preditores de Desempenho em 5km* | Fisiologia do exercício, consumo de oxigênio e limiares ventilatórios | [repositorio.ufmg.br](https://repositorio.ufmg.br/items/0d6cd236-75a8-478a-b15d-52158e5e3f7b) |
| **02** | **Dr. Adriano Leonardi** | *Canelite pode arruinar seu treino* | Medicina esportiva, causas biomecânicas da síndrome do estresse tibial medial e reabilitação | [adrianoleonardi.com.br](https://adrianoleonardi.com.br/artigos/canelite-pode-arruinar-treino/) |
| **03** | **Smart Fit News** | *Como começar a correr: planilha de 4 semanas para iniciantes* | Periodização prática e método de intervalos progressivos (*run/walk method*) | [smartfit.com.br](https://www.smartfit.com.br/news/fitness/como-comecar-correr-planilha/) |
| **04** | **Portugal Running / ASICS Training** | *Como Respirar a Correr: Guia Prático* | Respiração diafragmática, oxigenação eficiente e cadência respiratória rítmica (2:2 ou 3:3) | [portugalrunning.com](https://www.portugalrunning.com/como-respirar-correr/) |
| **05** | **Azon Assessoria Esportiva / Runna** | *5K abaixo dos 30 minutos: guia de ritmo e progressão* | Gestão de esforço, divisão de parciais (*splits*) e sustentação de pace alvo (6:00 min/km) | [azonesportes.com.br](https://azonesportes.com.br/5k-abaixo-dos-30-minutos/) |

---

## 3. Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

A engenharia de prompts em ferramentas com recuperação em fontes fechadas (*Grounding*) exige refinamento contínuo para evitar generalismos e alucinações de volume.

### A. Evolução de Prompts Estratégicos

#### 🔴 Iteração 1: Prompt Ingênuo / Genérico
> **Prompt:**  
> *"Como começar a correr 5km sem se machucar?"*
> 
> **Resultado:**  
> A resposta trouxe clichês comuns da internet (beba 2 litros de água, compre um tênis macio, corra devagar), sem explorar a profundidade técnica das fontes anexadas e sem fornecer métricas ou critérios fisiológicos claros.

#### 🟢 Iteração 2: Prompt Refinado (Papel, Restrições e Formato)
> **Prompt:**  
> *"Atuando como um treinador e fisioterapeuta esportivo especializado em corredores amadores, sintetize as fontes anexadas e estruture um plano de transição de 4 semanas (do sedentarismo aos primeiros 5 km contínuos). Exija: (1) divisão semanal de dias de treino e descanso, (2) proporção exata de caminhada/corrida por sessão, (3) 3 exercícios preventivos específicos para canelite/joelho e (4) sinais clínicos de alerta para interrupção imediata do treino."*
> 
> **Resultado:**  
> Saída técnica, estruturada em blocos, com citações diretas das fontes ortopédicas e parâmetros claros de esforço percebido (Zona 2).

---

### B. "Cicatrizes" de Engenharia e Troubleshooting

1. **Barreira de Ingestão por Paywall / Autenticação:**
   * **Problema:** Ao tentar carregar uma planilha hospedada no Scribd via URL direta (`pt.scribd.com/document/...`), o NotebookLM retornou status de falha de ingestão devido a restrições de login e bloqueios anti-scraping do portal.
   * **Solução:** O conteúdo foi substituído por artigos técnicos abertos de assessorias esportivas e calculadoras abertas de pace (*PaceCalc* e *Runna*), além de transcrições manuais em notas de texto estruturadas em Markdown.
2. **Alucinação de Intensidade Precoce:**
   * **Problema:** Ao solicitar um plano para "conquistar os primeiros 5 km em ritmo forte", a IA sugeriu séries de tiros anaeróbicos de alta intensidade logo na primeira semana de treinamento.
   * **Solução:** Inclusão de trava de segurança no *system prompt* da consulta: *"Baseie a progressão unicamente nas diretrizes para iniciantes das fontes, respeitando o princípio da adaptação musculoesquelética prévia ao trabalho de velocidade."*
3. **Equilíbrio de Formatos Multimídia:**
   * **Problema:** O excesso de transcrições de vídeos informais do YouTube acabou puxando o tom das respostas para uma linguagem muito coloquial e com pouca precisão em termos anatômicos.
   * **Solução:** Uso do filtro seletivo de fontes na barra lateral do NotebookLM, ativando apenas os artigos clínicos e o trabalho acadêmico da UFMG para formular os blocos de fisiologia e lesões.

---

## 4. Miniguia de Estudo (Entrega Final)

### 4.1 Resumo Estruturado do Assunto


```

┌─────────────────────────────────────────────────────────────┐
│          PILARES DA CORRIDA DE RUA PARA INICIANTES          │
├──────────────┬──────────────┬───────────────┬───────────────┤
│ Sobrecarga   │ Biomecânica  │ Respiração &  │ Nutrição &    │
│ Progressiva  │ Preventiva   │ Ritmo         │ Regeneração   │
└──────────────┴──────────────┴───────────────┴───────────────┘

```

1. **Princípio da Sobrecarga Progressiva:**
   * O sistema cardiovascular adapta-se em menor tempo que tendões, ossos e cartilagens.
   * As primeiras semanas devem priorizar o método intercalado (ex.: alternar 2 minutos de caminhada rápida com 1 minuto de trote leve), permitindo a remodelação óssea sem desencadear microlesões articulares.
2. **Biomecânica e Prevenção:**
   * **Cadência e Impacto:** Manter uma cadência de passos mais alta e passos mais curtos (em torno de 170 a 180 passos/minuto) evita o *overstriding* (aterrissar com o calcanhar muito à frente do corpo), diminuindo expressivamente o impacto sobre tíbias e joelhos.
   * **Superfície e Tênis:** Recomenda-se iniciar com calçados confortáveis e amortecimento intermediário, sem recorrer precipitadamente a tênis com placa de carbono na fase de adaptação motora.
3. **Respiração e Pacing:**
   * A respiração deve ser combinada (nasal e bucal) e predominantemente diafragmática, sincronizada com o ritmo dos passos (padrão 2:2 ou 3:3 em treinos aeróbicos contínuos).
   * O ritmo base deve se manter na **Zona 2 (Z2)**, na qual é possível conversar em frases completas sem perder o fôlego.
4. **Nutrição e Recuperação:**
   * Para percursos de até 5 km, géis de carboidrato intra-treino são dispensáveis.
   * O foco deve residir na hidratação regular prévia, consumo de carboidratos de fácil absorção antes da atividade e respeito ao intervalo de pelo menos 48 horas entre estímulos de impacto no estágio inicial.

---

### 4.2 Glossário de Conceitos-Chave

| Conceito | Descrição Técnica |
| :--- | :--- |
| **Pace** | Ritmo de deslocamento na corrida, expresso em minutos e segundos necessários para completar 1 km (ex.: `6'00"/km`). |
| **Canelite (MTSS)** | Síndrome do estresse tibial medial; processo inflamatório no periósteo da tíbia gerado por estresse mecânico repetitivo e tração muscular excessiva. |
| **Cadência (SPM)** | Quantidade total de passos por minuto (*steps per minute*). Cadências maiores reduzem o tempo de contato e a sobrecarga de pico no solo. |
| **Zona 2 (Z2)** | Faixa de treinamento aeróbico em intensidade moderada (60% a 70% da FC máxima), essencial para desenvolvimento mitocondrial e resistência de base. |
| **Treino Regenerativo** | Sessão de baixa intensidade e curta duração com o propósito de estimular a circulação local e acelerar a recuperação muscular sem gerar fadiga residual. |
| **Overstriding** | Desvio biomecânico caracterizado pela aterrissagem do pé excessivamente à frente do centro de gravidade, atuando como força de frenagem e aumentando forças de impacto. |

---

### 4.3 Prompts Reutilizáveis

#### 🔁 Prompt 1: Reajuste de Carga por Sinais de Fadiga ou Dor
```text
Atue como meu treinador de corrida. Estou na Semana [X] e sinto [dor na face interna da canela / fadiga muscular excessiva] após as sessões. Com base nas diretrizes médicas e de treinamento das fontes, determine se devo pausar totalmente ou substituir por exercícios de baixo impacto, indicando o protocolo seguro para a próxima semana.

```

#### 🔁 Prompt 2: Planejamento de Parciais de Prova (Pacing)

```text
Com base nos artigos de pacing e fisiologia esportiva das fontes, elabore uma estratégia de parciais km a km (split negativo) para concluir uma prova de 5 km na meta de [X minutos, ex.: 29:30]. Descreva o ritmo de cada quilômetro e as instruções de autocontrole para não largar em ritmo excessivo nos primeiros 1.000 metros.

```

#### 🔁 Prompt 3: Checklist Estruturado Pré-Prova

```text
Gere um checklist operacional em ordem cronológica (48 horas antes, noite anterior, 2 horas antes e 15 minutos antes da largada) focado em um corredor iniciante em sua primeira corrida de 5 km, contemplando hidratação, alimentação pré-treino, checagem de vestuário e protocolo de aquecimento dinâmico.

```

---

## 5. Conclusão e Próximos Passos

A aplicação do **Google NotebookLM** aliada a técnicas de curadoria e engenharia de contexto viabilizou a extração de recomendações esportivas seguras, eliminando alucinações habituais e estruturando um caminho prático para quem busca sair do zero rumo aos primeiros 5 km.

* [x] Curadoria de fontes multidisciplinares
* [x] Ingestão e validação de documentos
* [x] Documentação de testes de prompt e troubleshooting
* [ ] Implementação prática da planilha de 4 semanas
* [ ] Avaliação do primeiro teste de 5 km cronometrado

---
