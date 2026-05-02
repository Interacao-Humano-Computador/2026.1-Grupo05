# Avaliação Heurística – Super Estágios

## Introdução

O site Super Estágios (superestagios.com.br) é uma plataforma privada de intermediação de estágios que conecta estudantes, empresas e instituições de ensino em todo o Brasil. Fundada em 2009, a plataforma oferece serviços de divulgação de vagas, recrutamento e gestão de programas de estágio de forma gratuita para estudantes. A avaliação focou nas principais funcionalidades do portal do estudante: busca de vagas, cadastro e candidatura.

## Avaliação Heurística

A metodologia de avaliação escolhida foi a avaliação heurística, que é uma inspeção sistemática de interface baseada em diretrizes de usabilidade chamadas heurísticas (BARBOSA et al., 2021, p. 281). São ao todo 10 heurísticas, analisadas a seguir.

## Ponto 1 – Visibilidade do estado do sistema

Não foram encontrados erros nessa heurística no site.

## Ponto 2 – Correspondência entre o sistema e o mundo real

O formulário de busca de vagas usa termos que dependem de uma ordem específica de preenchimento, mas não comunica isso ao usuário de forma clara. Ao tentar selecionar a cidade sem ter escolhido o estado, o campo exibe apenas "Selecione um Estado!" sem nenhum destaque visual ou explicação. Uma análise mais detalhada pode ser vista na [Tabela 1](#tabela-1).

<a id="tabela-1"></a>

| Correspondência entre o sistema e o mundo real |
| :--- |
| **Verificação:** O site utiliza linguagem e convenções familiares ao usuário? |
| **Grau de severidade:** Simples |
| **Natureza do problema:** Obstáculo |
| **Perspectiva do usuário:** Problema Geral |
| **Perspectiva da tarefa:** Problema Principal |
| **Perspectiva do projeto:** Não se aplica |
| **Descrição do problema:** O campo "Cidade" do filtro de busca fica bloqueado sem explicação visível quando o usuário não seleciona o estado primeiro. |
| **Causa do problema:** Dependência de ordem entre campos sem orientação visual adequada ao usuário. |
| **Efeito sobre o usuário:** Confusão e frustração, especialmente para usuários menos experientes. |
| **Efeito sobre a tarefa:** O usuário não consegue filtrar vagas por cidade sem entender a ordem correta de preenchimento. |

*Tabela 1 – Formulário de Avaliação Heurística do Ponto 2.*
*Fonte: Luís, 2026.*

## Ponto 3 – Controle e liberdade do usuário

Não foram encontrados erros nessa heurística no site.

## Ponto 4 – Consistência e padronização

O formulário de cadastro do estudante não apresenta um padrão visual consistente para indicar campos obrigatórios. Além disso, campos como CPF, telefone e CEP não possuem máscaras de entrada, permitindo que o usuário insira dados em formatos incorretos e só descubra o erro ao tentar enviar o formulário. Uma análise mais detalhada pode ser vista na [Tabela 2](#tabela-2).

<a id="tabela-2"></a>

| Consistência e padronização |
| :--- |
| **Verificação:** O site segue convenções e padrões consistentes ao longo de suas páginas? |
| **Grau de severidade:** Grave |
| **Natureza do problema:** Obstáculo |
| **Perspectiva do usuário:** Problema Geral |
| **Perspectiva da tarefa:** Problema Principal |
| **Perspectiva do projeto:** Não se aplica |
| **Descrição do problema:** O formulário de cadastro não padroniza a indicação de campos obrigatórios e não aplica máscaras de entrada para campos com formato definido (CPF, telefone, CEP). |
| **Causa do problema:** Falta de validação em tempo real e ausência de padrão visual para campos obrigatórios. |
| **Efeito sobre o usuário:** Frustração ao descobrir erros apenas no envio do formulário. |
| **Efeito sobre a tarefa:** O cadastro do estudante é interrompido por erros evitáveis de preenchimento. |

*Tabela 2 – Formulário de Avaliação Heurística do Ponto 4.*
*Fonte: Luís, 2026.*

## Ponto 5 – Reconhecimento em vez de memorização

Os cards de vagas exibidos na listagem mostram apenas o nome do curso, cidade e valor da bolsa, sem informações sobre área de atuação, empresa ou carga horária. O usuário precisa clicar em cada vaga para descobrir informações básicas que poderiam ajudá-lo a decidir se tem interesse. Uma análise mais detalhada pode ser vista na [Tabela 3](#tabela-3).

<a id="tabela-3"></a>

| Reconhecimento em vez de memorização |
| :--- |
| **Verificação:** O site minimiza a necessidade de o usuário memorizar informações entre telas? |
| **Grau de severidade:** Simples |
| **Natureza do problema:** Obstáculo |
| **Perspectiva do usuário:** Problema Preliminar |
| **Perspectiva da tarefa:** Problema Secundário |
| **Perspectiva do projeto:** Não se aplica |
| **Descrição do problema:** Os cards de vagas apresentam informações insuficientes para triagem, forçando o usuário a abrir cada vaga individualmente para obter dados básicos. |
| **Causa do problema:** Cards com campos resumidos demais que não permitem comparação direta entre vagas. |
| **Efeito sobre o usuário:** Cansaço e perda de tempo ao navegar por muitas vagas. |
| **Efeito sobre a tarefa:** O usuário leva mais tempo do que o necessário para encontrar uma vaga adequada ao seu perfil. |

*Tabela 3 – Formulário de Avaliação Heurística do Ponto 5.*
*Fonte: Luís, 2026.*

## Ponto 6 – Flexibilidade e eficiência de uso

Não foram encontrados erros nessa heurística no site.

## Ponto 7 – Projeto estético e minimalista

A página inicial do site exibe um carrossel de banners promocionais que ocupa a maior parte da tela no primeiro acesso, sem apresentar de forma clara e imediata o propósito do portal ou como começar a usá-lo. Um usuário que acessa o site pela primeira vez precisa rolar a página para entender o que o site oferece. Uma análise mais detalhada pode ser vista na [Tabela 4](#tabela-4).

<a id="tabela-4"></a>

| Projeto estético e minimalista |
| :--- |
| **Verificação:** A interface contém apenas informações necessárias, sem elementos que distraiam o usuário? |
| **Grau de severidade:** Simples |
| **Natureza do problema:** Ruído |
| **Perspectiva do usuário:** Problema Preliminar |
| **Perspectiva da tarefa:** Problema Secundário |
| **Perspectiva do projeto:** Não se aplica |
| **Descrição do problema:** A página inicial prioriza banners promocionais em detrimento de uma apresentação clara do propósito e das funcionalidades do portal. |
| **Causa do problema:** Design com foco em marketing sem orientação suficiente ao novo usuário. |
| **Efeito sobre o usuário:** Desorientação no primeiro acesso; o usuário não sabe imediatamente o que fazer. |
| **Efeito sobre a tarefa:** O usuário perde tempo procurando como acessar as funcionalidades principais. |

*Tabela 4 – Formulário de Avaliação Heurística do Ponto 7.*
*Fonte: Luís, 2026.*

## Ponto 8 – Prevenção de erros

Não foram encontrados erros nessa heurística no site.

## Ponto 9 – Ajude os usuários a reconhecerem, diagnosticarem e se recuperarem de erros

Não foram encontrados erros nessa heurística no site.

## Ponto 10 – Ajuda e documentação

O site não possui uma seção de ajuda ou FAQ facilmente acessível durante o fluxo de uso. O link de contato está disponível apenas no rodapé, e não há suporte contextual nos formulários de cadastro ou nas páginas de candidatura a vagas. Uma análise mais detalhada pode ser vista na [Tabela 5](#tabela-5).

<a id="tabela-5"></a>

| Ajuda e documentação |
| :--- |
| **Verificação:** O sistema oferece ajuda e documentação facilmente acessíveis? |
| **Grau de severidade:** Simples |
| **Natureza do problema:** Ruído |
| **Perspectiva do usuário:** Problema Preliminar |
| **Perspectiva da tarefa:** Problema Secundário |
| **Perspectiva do projeto:** Não se aplica |
| **Descrição do problema:** Não há ajuda contextual nos formulários nem FAQ de fácil acesso durante o fluxo de uso. O suporte está disponível apenas no rodapé da página. |
| **Causa do problema:** Documentação de ajuda centralizada e desconectada do fluxo de uso do estudante. |
| **Efeito sobre o usuário:** Usuários com dúvidas precisam interromper o que estão fazendo para procurar ajuda em outro local. |
| **Efeito sobre a tarefa:** Pode atrasar ou interromper o cadastro e a candidatura a vagas. |

*Tabela 5 – Formulário de Avaliação Heurística do Ponto 10.*
*Fonte: Luís

> [1] SUPER ESTÁGIOS. **Portal Super Estágios**. Disponível em: https://www.superestagios.com.br. Acesso em: 01 maio 2026.

> [2] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Autopublicação, 2021.

## Histórico de Versões

| Data | Versão | Descrição | Autor | Revisor |
|------|--------|-----------|-------|---------|
| 01/05/2026 | `1.1` | Criação da avaliação heurística | Luís Oliveira | Samuel |