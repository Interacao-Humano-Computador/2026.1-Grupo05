# Persona 5

## Contribuidores

| Nome do Contribuidor | Tópico desenvolvido |
| :--- | :--- |
| Arthur Mezzaroba | [Introdução](#introducao) <br> [Identidade](#identidade) <br> [Cenários](#cenarios) <br> [Referências Bibliográficas](#referencias-bibliograficas) <br> [Bibliografia](#bibliografia) <br> [Histórico de versão](#historico-de-versoes) |

<a id="introducao"></a>
# Introdução

<div align="justify">
    O método para definição de personas apresentado na literatura baseia-se na criação de personagens fictícios que funcionam como arquétipos hipotéticos de grupos de usuários reais. O objetivo dessa abordagem é evitar o conceito genérico e impreciso de um "usuário elástico", que obriga o usuário a se contorcer para se adaptar ao sistema. Em vez disso, a construção de uma persona foca em projetar interações para alvos muito específicos.
    <p>
    Para complementar o uso de personas na organização do espaço do problema, utilizam-se os cenários. Um cenário é basicamente uma história sobre pessoas realizando uma atividade[cite: 1]. Trata-se de uma narrativa, que pode ser textual ou pictórica, concreta e rica em detalhes contextuais sobre uma situação de uso da aplicação, envolvendo usuários, processos e dados reais ou potenciais[cite: 1]. 
    <p>
    Os cenários descrevem o comportamento e as experiências dos atores, possuindo um enredo que inclui sequências de ações e eventos que ajudam, atrapalham ou são irrelevantes para o atingimento dos objetivos desses atores[cite: 1]. Eles podem ser utilizados em diversas etapas do processo com diferentes objetivos: descrever uma história num domínio de atividade para capturar requisitos, levantar questões sobre a introdução de tecnologia, explorar diferentes soluções de design e avaliar se o produto satisfaz as necessidades dos usuários[cite: 1].
</div>

<a id="identidade"></a>
### Identidade:

- **Foto:**
<div align="center">
  <img src="assets\Persona5.png" width="150">
</div>
<div align="center"> <p> <i><b>Figura 1:</b> Representação de uma persona (Fonte: https://thispersondoesnotexist.com/ acessado em: 03/05/2026).</i> </p> </div>

- **Nome:** Roberto
- **Sobrenome:** Martins Costa
- **Idade:** 42
- **Sexo:** Masculino
- **Gênero:** Cisgênero
- **Escolaridade:** Pós-graduação Completa
- **Cargo Atual:** Coordenador de Estágios / Administrador da Plataforma
- **Área de educação:** Administração de Empresas e Gestão de RH
- **Status:** Persona Secundária
- **Objetivos gerais:** Gerenciar o fluxo de estágios de forma eficiente, garantindo que as empresas parceiras encontrem os candidatos ideais e que a burocracia seja cumprida sem atrasos.
    - **Objetivos pessoais:** 
        - Reduzir o nível de estresse no trabalho gerado pelo acúmulo de papéis físicos e e-mails perdidos.
    - **Objetivos práticos:** 
        - Aprovar documentações e emitir o Termo de Compromisso de Estágio (TCE) rapidamente.
        - Publicar e editar novas vagas solicitadas pelas empresas parceiras.
        - Visualizar um painel (dashboard) com o status atualizado de todos os candidatos em processo seletivo.
        - Responder a dúvidas de alunos de forma centralizada e ágil.
        - Integrar a comunicação entre empresa, aluno e instituição de ensino.
- **Habilidades:** Excelente organização, proficiência em softwares de gestão e sistemas de RH, boa comunicação escrita.
- **Tarefas:**
    - **Básicas:** Fazer login no sistema corporativo, verificar o painel de pendências e publicar novas vagas.
    - **Críticas:** Validar documentação legal de estágio enviada por alunos, gerar contratos (TCE) e gerenciar os agendamentos de entrevistas.
    - **Frequência:** Diária (Uso contínuo durante o horário comercial).
- **Relacionamentos:** Se relaciona com estudantes (candidatos), representantes das empresas parceiras e instituições de ensino.
- **Requisitos:** Painel de controle visual claro, sistema de notificação de pendências, gerador automático de contratos em PDF e chat/ferramenta de suporte aos alunos.
- **Expectativas:** Ele espera que a plataforma automatize a triagem inicial e a geração de contratos, permitindo que ele foque apenas na validação e no suporte humano quando necessário.

### Roberto Martins, Coordenador de Estágios - "Gestão centralizada e sem papelada"

<div align="justify">
Persona: Roberto Martins Costa – “Gestão centralizada e sem papelada” <p> Roberto tem 42 anos, é formado em Administração e trabalha como Coordenador de Estágios em um grande agente de integração há cinco anos. Ele tem uma rotina de escritório intensa e passa a maior parte do dia na frente do computador gerenciando demandas de três frentes diferentes: empresas que precisam de estagiários, alunos buscando vagas e universidades que exigem relatórios legais. Como um profissional experiente, ele tem facilidade com sistemas de gestão, mas sofre com plataformas lentas ou que exigem muitos cliques para realizar ações repetitivas. <p> O maior problema de Roberto é o tempo perdido verificando anexos de e-mails desconexos e conferindo assinaturas manuais em documentos. Sua expectativa é utilizar uma plataforma que ofereça um "Dashboard" limpo e intuitivo, onde ele possa ver instantaneamente quais alunos enviaram os documentos pendentes, validar essas informações com poucos cliques e gerar o Termo de Compromisso de Estágio (TCE) automaticamente. Ele deseja uma ferramenta que lhe dê controle total sobre a publicação de vagas e que centralize a comunicação, evitando que ele precise usar o e-mail pessoal ou telefone para cobrar respostas dos candidatos.
</div>    

#### Objetivos pessoais:
- Minimizar o estresse com burocracia repetitiva e evitar a perda de documentos importantes
- Manter o ambiente de trabalho digital organizado, dispensando o uso de papéis

#### Objetivos práticos (instrumentais e finais):
- Visualizar um painel de controle (dashboard) com alertas automáticos de tarefas pendentes
- Publicar, pausar ou editar anúncios de vagas com rapidez e precisão
- Analisar, aprovar ou rejeitar documentos (como RG, CPF e comprovantes de matrícula) enviados pelos candidatos
- Gerar e distribuir o Termo de Compromisso de Estágio (TCE) automaticamente para coleta de assinaturas digitais
- Interagir com os alunos através de um sistema de suporte ou chat integrado

<a id="cenarios"></a>
## Cenário de Interação: Triagem de documentos e geração de contrato de estágio

Atores: 

<div align="justify"; style="font-style: italic;">
"Em uma manhã de segunda-feira, Roberto chega ao escritório do agente de integração e se depara com o acúmulo de documentações enviadas pelos alunos durante o final de semana. Focado em zerar essa fila antes da sua reunião de equipe às 10h, ele acessa o sistema da plataforma e utiliza o filtro de 'Documentos Pendentes de Análise' no seu painel de controle. A plataforma exibe a lista de alunos aprovados nas entrevistas, e ele seleciona o perfil da candidata Carla Alves. Roberto analisa visualmente os documentos escaneados, como o RG e a declaração de matrícula, diretamente na tela do sistema, sem a necessidade de baixar anexos ou imprimir papéis. Satisfeito com a conformidade dos dados, ele clica no botão para aprovar a documentação e, em seguida, seleciona a opção de gerar o contrato. Instantaneamente, o sistema atualiza o status do processo de Carla para 'Contrato em Emissão', compila os dados cadastrais da empresa e da aluna, e gera o Termo de Compromisso de Estágio (TCE) em formato PDF com os campos para assinatura digital. O próprio sistema dispara automaticamente uma notificação para o e-mail e aplicativo de Carla solicitando a assinatura. Ao observar a fila de pendências do seu painel diminuir rapidamente, Roberto conclui suas tarefas aliviado com a agilidade do processo, confirmando que a automação evitou o retrabalho de digitar dados manualmente e garantiu a contratação sem atrasos legais."
</div>

<a id="referencias-bibliograficas"></a>
# Referências bibliográficas

> [1] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Rio de Janeiro: Autopublicação, 2021.

<a id="bibliografia"></a>
## Bibliografia

> [1] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Rio de Janeiro: Autopublicação, 2021.

<a id="historico-de-versoes"></a>
## Histórico de Versões

| Data | Versão | Descrição | Autor | Revisor |
| :--- | :--- | :--- | :--- | :--- |
| 03/05/2026 | 1.0 | Elaboração do artefato da Persona Administrativa e Cenário | Arthur Mezzaroba | Mariana Martins |