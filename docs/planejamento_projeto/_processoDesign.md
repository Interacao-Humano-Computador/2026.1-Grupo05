# Processo de Design

## Introdução
Antes de detalharmos os processos, é fundamental definir o que é design. Segundo Barbosa et al. (2021), o design pode ser compreendido como um processo que engloba três atividades básicas: a análise da situação atual (identificação e compreensão de um problema), a síntese de uma intervenção (criação de uma solução) e a avaliação da nova situação (verificação dos impactos da intervenção).

Os processos de design em IHC são metodologias que permitem executar essas atividades de forma sistemática e iterativa, garantindo que as soluções desenvolvidas atendam realidades e necessidades dos usuários. Na literatura, destacam-se quatro processos principais: Ciclo de Vida Simples, Ciclo de Vida em Estrela, Engenharia de Usabilidade de Nielsen e Engenharia de Usabilidade de Mayhew.

Neste projeto, o processo escolhido pela equipe foi o **Ciclo de Vida de Mayhew**. A seguir, detalhamos os quatro modelos e apresentamos as motivações que levaram a essa escolha técnica.

## Modelos de Processo de Design

### Ciclo de Vida Simples
Proposto por Preece, Sharp e Rogers, este modelo é considerado uma visão simplificada do design de interação. Ele se concentra fundamentalmente na alternância entre duas atividades principais: o design (ou redesign) e a construção de uma versão interativa.

Durante o design, o avaliador busca alternativas para solucionar os requisitos definidos na fase de análise. Os resultados costumam ser representados por esboços ou descrições textuais. Em seguida, constroem-se versões interativas (protótipos) dessas soluções para demonstrar o funcionamento da interface, permitindo que os usuários avaliem a proposta antes da implementação final.

<div align="center">
  <img src="assets/image1.png" width="800">
</div>
<div align="center"> <p> <i><b>Figura 1:</b> Ciclo de vida de simples (Fonte: BARBOSA, Simone; DINIZ, Bruno. 2010).</i> </p> </div>

### Ciclo de Vida em Estrela
Desenvolvido por Hix e Hartson, o Ciclo de Vida em Estrela tem uma característica marcante: a atividade de **avaliação** está no centro do processo. 

Neste modelo, o designer tem a liberdade de escolher por qual atividade começar (seja análise de tarefas, prototipação ou implementação). No entanto, independentemente do caminho escolhido, é obrigatório passar pela avaliação ao final de cada etapa. Essa centralidade garante que os dados coletados e as representações de design estejam sempre alinhados às necessidades reais do usuário, permitindo a detecção precoce de problemas de usabilidade.

<div align="center">
  <img src="assets/image.png" width="800">
</div>
<div align="center"> <p> <i><b>Figura 2:</b> Ciclo de vida de estrela (Fonte: BARBOSA, Simone; DINIZ, Bruno. 2010).</i> </p> </div>

### Engenharia de Usabilidade de Nielsen
Proposta por Jakob Nielsen, a engenharia de usabilidade é apresentada como um conjunto de práticas que devem acompanhar todo o ciclo de vida do produto. O modelo é focado em garantir a usabilidade por meio de passos metódicos.

A tabela abaixo resume as atividades definidas por Nielsen:

| Passo | Atividade |
| :---: | :--- |
| **1** | Conheça seu usuário |
| **2** | Realize uma análise competitiva |
| **3** | Defina as metas de usabilidade |
| **4** | Faça designs paralelos |
| **5** | Adote o design participativo |
| **6** | Faça o design coordenado da interface como um todo |
| **7** | Aplique diretrizes e análise heurística |
| **8** | Faça protótipos |
| **9** | Realize testes empíricos |
| **10**| Pratique design iterativo |
<div align="center"> <p> <i>Tabela 1: Atividades da Engenharia de Usabilidade de Nielsen (Adaptado de Barbosa et al., 2021).</i> </p> </div>

### Engenharia de Usabilidade de Mayhew
Deborah Mayhew estruturou um modelo iterativo de engenharia de usabilidade focado em integrar a área de IHC ao desenvolvimento de software tradicional. Ele é dividido em três fases principais:

#### 1. Análise de Requisitos
Nesta etapa, são definidas as metas de usabilidade. Isso é feito com base no perfil dos usuários, na análise das tarefas, nas restrições da plataforma e nos princípios gerais de IHC. Os resultados costumam ser documentados em Guias de Estilo, que padronizam o layout, tipografia, cores e padrões de interação.

#### 2. Design, Avaliação e Desenvolvimento
O objetivo desta fase é conceber uma solução que atinja as metas definidas anteriormente, passando por três níveis de detalhamento:
* **Nível 1:** Repensar a execução das tarefas e criar protótipos de baixa fidelidade.
* **Nível 2:** Estabelecer padrões de design e construir protótipos de média fidelidade.
* **Nível 3:** Projetar detalhadamente a interface em alta fidelidade para, então, implementá-la.
Sempre há avaliação entre os níveis para validar as decisões de design.

#### 3. Instalação
Fase em que o sistema é entregue aos usuários. Aqui, coleta-se feedback de uso ao longo do tempo. Essas opiniões servem para apontar defeitos, sugerir melhorias para versões futuras ou até justificar o desenvolvimento de um sistema completamente novo.

## Motivações para a Escolha

Após debater as características de cada processo, a equipe optou pela utilização da **Engenharia de Usabilidade de Mayhew**. 

A principal motivação técnica é o alto nível de detalhamento metodológico que este ciclo oferece. Por ter etapas rigorosamente definidas, o modelo reduz a subjetividade no processo de design e fornece um guia seguro, o que é ideal para garantir o alinhamento com as exigências da disciplina.

Além disso, como o portal escolhido para o projeto já é um sistema em produção (Agendamento Eletrônico), o ciclo de Mayhew se encaixa perfeitamente na nossa realidade. O projeto se iniciará, na prática, pela fase de **Instalação** — avaliando a interface atual para identificar problemas de interação — para, em seguida, realimentar o ciclo retornando à **Análise de Requisitos** e guiando o reprojeto nas fases subsequentes.

## Bibliografia

> [1] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Rio de Janeiro: Autopublicação, 2021.

## Contribuidores

| Nome do Contribuidor |
| :--- |
| Luis Gustavo |
| [--](--) |

## Histórico de Versões

| Data | Versão | Descrição | Autor | Revisor |
| :--- | :--- | :--- | :--- | :--- |
| 12/04/2026 | 1.0 | Elaboração do artefato processo design | Luis Gustavo | --|