
## Contribuidores

| Nome do Contribuidor | Tópico desenvolvido |
| :--- |  :--- |
| Samuel Leite |  [Introdução](#introducao) <br> [Árvores de Tarefas Concorrentes (ConcurTaskTrees– CTT)](#analise-ctt) <br> [Diagrama da Análise de tarefas concorrentes (ConcurTaskTrees–CTT)](#diagrama-ctt) <br> [Referências Bilbiográficas](#referencias-bibliograficas) <br> [Bibliografia](#bibliografia) <br> [Histórico de versão](#historico-de-versoes) <br>|
| Pedro Henrique | [CTT para Assinatura Digital do TCE via Reconhecimento Facial](#ctt-assinatura-facial) <br> [Análise de Tarefas (CTT) - Assinatura Digital do TCE via Reconhecimento Facial](#analise-ctt-assinatura) <br> [Diagrama de análise de tarefas CTT - Assinatura Facial](#diagrama-ctt-assinatura) <br> 


<a id="introducao"></a>
# Introdução
<div align="justify">
    <p> O modelo de Árvores de Tarefas Concorrentes (ConcurTaskTrees – CTT) foi criado para auxiliar o design e a avaliação de Interação Humano-Computador (IHC). Diferente de outros modelos tradicionais, o CTT vai além da análise de tarefas convencional para representar uma solução completa de design da interação, pois permite o registro explícito não só do que o usuário faz, mas também do que o sistema faz (Barbosa, 2021).</p>
    <p> Para isso, o CTT classifica as tarefas em quatro tipos principais (Barbosa, 2021): 
    <ul>
        <li><strong>Tarefas do usuário:</strong> Realizadas fora do sistema (ações cognitivas ou físicas que não envolvem interação direta com a máquina).</li>
        <li><strong>Tarefas do sistema:</strong> O sistema realiza um processamento sem interagir com o usuário.</li>
        <li><strong>Tarefas interativas:</strong> Onde ocorrem os diálogos entre o usuário e o sistema.
        <li><strong>Tarefas abstratas:</strong> não são tarefas em si, mas uma representação de uma composição de outras tarefas menores, auxiliando a decomposição da árvore.</li>
    </ul>
    <br>
    Além da hierarquia (onde uma tarefa pai é decomposta em tarefas filhas), a grande expressividade do CTT está nas relações temporais e lógicas entre as tarefas
    As principais relações são (Barbosa, 2021):
    <ul>
        <li><strong>Ativação (>>):</strong> uma tarefa só inicia após a anterior terminar.</li>
        <li><strong>Ativação com passagem de informação ([]>>):</strong> a segunda tarefa inicia após a primeira e recebe informações produzidas por ela.</li>
        <li><strong>Escolha ([]):</strong> tarefas alternativas; iniciar uma desabilita a outra.</li>
        <li><strong>Concorrência (|||):</strong> as tarefas podem ser realizadas em qualquer ordem ou ao mesmo tempo.</li>
        <li><strong>Concorrência e comunicação (|[]|):</strong> as tarefas ocorrem juntas e podem trocar informações entre si.</li>
        <li><strong>Independência (|=|):</strong> podem ser iniciadas em qualquer ordem, mas quando uma inicia, precisa terminar para que a outra comece.</li>
        <li><strong>Desativação ([>):</strong> a primeira tarefa é completamente interrompida pela segunda.</li>
        <li><strong>Suspensão/retomada (|>)</strong>: a primeira tarefa é interrompida pela segunda e retomada de onde parou assim que a segunda terminar</li>
    </ul>
</div>

<br>

<a id="analise-ctt"></a>
# Análise de Tarefas (CTT) para o Cenário da Plataforma SuperEstágios
<div align="justify">
    <p>Aplicando o modelo CTT para a persona Carla Alves Silva, que deseja realizar todo o processo de seleção (desde a busca até a assinatura do contrato) de forma rápida e concentrada, desenvolvemos a seguinte árvore de tarefas concorrentes. Devido à limitação de interface gráfica de texto, a árvore é representada de forma hierárquica e textual, utilizando os operadores de relação:</p>
    <ul>
        <li><strong>T0: Gerenciar jornada de estágio na plataforma (Tarefa Abstrata) Para que Carla consiga seu estágio, ela passa por quatro grandes fases sequenciais.</strong></li>
            <ul>
                <li><strong> Decomposição de T0:</strong>> T1: Preparar perfil na plataforma (Abstrata) >> T2: Encontrar e aplicar para vaga (Abstrata) >> T3: Participar do processo seletivo (Abstrata) >> T4: Formalizar a contratação (Abstrata).</li>
            </ul>
        <li><strong>T1: Preparar perfil na plataforma (Tarefa Abstrata) Carla valoriza seu tempo e deseja fazer o cadastro apenas uma vez.</strong></li>
        <ul>
                <li><strong>Decomposição de T1:</strong> T1.1: Criar cadastro inicial (Interativa) >> T1.2: Enviar documentação complementar (Abstrata).</li>
                <li><strong>Decomposição de T1.2:</strong> T1.2.1: Enviar currículo em PDF (Interativa) ||| T1.2.2: Enviar documentos pessoais (Interativa) (O uso de concorrência ||| indica que Carla pode enviar o currículo e os documentos pessoais na ordem que preferir, ou até simultaneamente em abas diferentes).</li>
            </ul>
        <li><strong>T2: Encontrar e aplicar para vaga (Tarefa Abstrata) Carla busca vagas usando filtros e espera se candidatar com apenas um clique.</strong></li>
        <ul>
                <li><strong>Decomposição de T2:</strong> T2.1: Buscar vaga disponível (Interativa) []>> T2.2: Se candidatar de forma simplificada para a vaga (Interativa) >> T2.3: Registrar candidatura da estudante (Sistema). (A ativação com passagem de informação []>> é usada porque os dados e o ID da vaga que Carla encontrou na busca (T2.1) são passados diretamente para a função de se candidatar (T2.2), permitindo a candidatura em 1 clique).</li>
            </ul>
        <li><strong>T3: Participar do processo seletivo (Tarefa Abstrata) Para vagas que exigem testes e entrevistas centralizadas na plataforma.</strong></li>
        <ul>
                <li><strong>Decomposição de T3: T3.1:</strong> Realizar etapa de testes (Abstrata) >> T3.2: Etapa de Entrevistas (Abstrata).</li>
                <li><strong>Decomposição de T3.1: T3.1.1:</strong> Realizar prova online pela plataforma (Interativa) |[]| T3.1.2: Salvar progresso da prova automaticamente (Sistema). (A relação de concorrência e comunicação |[]| mostra que, enquanto Carla resolve a prova (T3.1.1), o sistema trabalha ao mesmo tempo salvando seu progresso e trocando informações com a interface para evitar perda de dados)</li>
                <li><strong>Decomposição de T3.2: T3.2.1:</strong> Realizar agendamento de entrevista em uma vaga disponível (Interativa) >> T3.2.2: Realizar a entrevista dentro da plataforma (Interativa).</li>
            </ul>
        <li><strong>T4: Formalizar a contratação (Tarefa Abstrata) Etapa final burocrática para emissão do Termo de Compromisso de Estágio (TCE)</strong></li>
        <ul>
                <li><strong>Decomposição de T4: T4.1:</strong> Analisar TCE gerado (Interativa) >> T4.2: Efetuar assinatura de documentos pelo GOV.BR (Interativa) []>> T4.3: Validar assinatura eletrônica e liberar termo assinado (Sistema). (Novamente, a ativação com passagem de informação []>> entra em ação, pois o GOV.BR devolve os tokens de autenticação da assinatura de Carla para que o sistema (T4.3) valide o documento internamente de forma automática</li>
        </ul>
    </ul>
</div>

<a id="diagrama-ctt"></a>
### Diagrama de análise de tarefas CTT
O Diagrama 1 a seguir represeta a análise de tarefas realizadas pela persona Carla Alves Silva de forma gráfica:
<div align="center">
  <img src="assets\analise-tarefas-CTT.jpg" width="100%">
</div>
<div align="center"> <p> <i><b>Figura 1:</b> Diagrama CTT. Fonte: Elaboração própria</i> </p> </div>

<br>
<br>
<br>

<a id="ctt-assinatura-facial"></a>
# CTT para Assinatura Digital do TCE via Reconhecimento Facial

<div align="justify">
    <p>Esta seção apresenta a modelagem utilizando o método de Árvores de Tarefas Concorrentes (CTT - ConcurTaskTrees) para a nova funcionalidade de Assinatura Digital do Termo de Compromisso de Estágio (TCE) via Reconhecimento Facial no sistema Super Estágios. A funcionalidade visa reduzir a carga cognitiva do usuário, substituindo senhas por uma operação física rápida através das capacidades biométricas dos smartphones.</p>
    <p>Aplicando o modelo CTT para o contexto de formalização de contratação onde o candidato necessita assinar o TCE de forma segura e rápida, desenvolvemos a seguinte árvore de tarefas concorrentes:</p>
</div>

### Análise de Tarefas (CTT) - Assinatura Digital do TCE via Reconhecimento Facial
<div align="justify">
    <ul>
        <li><strong>T0: Assinar TCE com Reconhecimento Facial (Tarefa Abstrata)</strong> O candidato completa a assinatura do Termo de Compromisso através de validação biométrica integrada.</li>
        <ul>
            <li><strong>Decomposição de T0:</strong> T1: Selecionar método de assinatura (Interativa) >> T2: Configurar e validar câmera (Abstrata) >> T3: Capturar e processar dados biométricos (Abstrata) >> T4: Confirmar assinatura (Interativa).</li>
        </ul>
        <li><strong>T1: Selecionar método de assinatura (Tarefa Interativa)</strong> O candidato escolhe a opção de biometria facial como método preferencial de autenticação.</li>
        <ul>
            <li><strong>Decomposição de T1:</strong> T1.1: Visualizar opções de assinatura (Interativa) >> T1.2: Selecionar "Assinar com Biometria Facial" (Interativa) >> T1.3: Sistema confirma seleção (Sistema).</li>
            <li><strong>Operador: >> (Ativação Sequencial)</strong> Cada etapa depende da anterior para prosseguir.</li>
        </ul>
        <li><strong>T2: Configurar e validar câmera (Tarefa Abstrata)</strong> O sistema prepara o ambiente para captura biométrica e solicita permissões necessárias.</li>
        <ul>
            <li><strong>Decomposição de T2:</strong> T2.1: Sistema solicita permissão de câmera (Sistema) >> T2.2: Candidato conceder permissão (Usuário) >> T2.3: Validar acesso à câmera (Sistema).</li>
            <li><strong>Operador: >> (Ativação com Passagem de Informação []>>)</strong> O resultado da permissão é passado para validação.</li>
        </ul>
        <li><strong>T3: Capturar e processar dados biométricos (Tarefa Abstrata)</strong> O rosto do candidato é capturado, posicionado e validado de forma segura.</li>
        <ul>
            <li><strong>Decomposição de T3: T3.1:</strong> Posicionar rosto no enquadramento (Usuário) |[]| T3.2: Fornecer orientações de posição em tempo real (Sistema) (A concorrência e comunicação |[]| indica que o usuário se posiciona enquanto o sistema oferece feedback simultâneo).</li>
            <li><strong>Após T3.1 e T3.2 completadas:</strong> T3.3: Capturar imagem biométrica (Sistema) >> T3.4: Processar validação facial em background (Sistema) >> T3.5: Notificar resultado (Sucesso ou Falha) (Sistema) [].</li>
            <li><strong>Operador: [] (Escolha)</strong> O sistema informa sucesso ou falha, levando a desfechos diferentes.</li>
        </ul>
        <li><strong>T4: Confirmar assinatura (Tarefa Interativa)</strong> O candidato visualiza a confirmação de sucesso e concluir o processo.</li>
        <ul>
            <li><strong>Decomposição de T4:</strong> T4.1: Exibir confirmação visual de assinatura (Sistema) >> T4.2: Candidato visualiza termo assinado (Usuário) >> T4.3: Sistema envia confirmação por e-mail e notifica Lourdes (Sistema).</li>
            <li><strong>Operador: >> (Ativação Sequencial)</strong> Cada etapa depende da conclusão anterior.</li>
        </ul>
    </ul>
</div>

<a id="diagrama-ctt-novavaga"></a>
### Diagrama de análise de tarefas CTT - Nova Vaga
O diagrama a seguir representa graficamente a árvore de tarefas concorrentes para a Criação de uma Nova Vaga:


<div align="center"> <p> <i><b>Figura 2:</b> Diagrama CTT para Nova Vaga. Fonte: Elaboração própria</i> </p> </div>


<a id="ctt-nova-vaga"></a>
# CTT para Nova Vaga

Esta seção apresenta a modelagem utilizando o método de Árvores de Tarefas Concorrentes (CTT - ConcurTaskTrees) para a funcionalidade de Cadastro de Novas Vagas no sistema de integração universidade e empresa. O objetivo desta análise é mapear a interação entre o recrutador e a plataforma, otimizando o fluxo de trabalho para que a publicação de oportunidades seja intuitiva e livre de ambiguidades, mantendo o usuário informado sobre o estado do sistema em cada etapa.
</div>


<div align="justify"> <ul> <li><strong>T0: Recrutador cadastra nova vaga</strong> O recrutador preenche as informações de título, competências e remuneração, e publica a vaga no sistema.</li> <ul> <li><strong>Decomposição de T0:</strong> T1: Informar título da vaga (Interativa) >> T2: Selecionar competências (Interativa) >> T3: Definir remuneração (Interativa) >> T4: Confirmar publicação (Interativa).</li> </ul> <li><strong>T1: Informar título da vaga (Tarefa Interativa)</strong> O recrutador insere o título do cargo e recebe sugestões para evitar ambiguidade.</li> <ul> <li><strong>Decomposição de T1:</strong> T1.1: Preencher campo título (Usuário) >> T1.2: Sistema sugerir títulos padrão (Sistema) >> T1.3: Recrutador escolher entre sugestão ou título original (Interativa).</li> <li><strong>Operador: >> (Ativação Sequencial) com [] (Escolha) implícita</strong> O sistema apresenta sugestões, e o recrutador decide qual título manter.</li> </ul> <li><strong>T2: Selecionar competências (Tarefa Interativa)</strong> O recrutador escolhe requisitos técnicos e comportamentais a partir de uma lista categorizada.</li> <ul> <li><strong>Decomposição de T2:</strong> T2.1: Visualizar categorias de competências (Sistema) >> T2.2: Navegar/expandir categorias (Usuário) >> T2.3: Selecionar competências via tags (Usuário) >> T2.4: Sistema armazenar seleção (Sistema).</li> <li><strong>Operador: >> (Ativação Sequencial)</strong> Cada etapa ocorre em ordem, garantindo que o sistema exiba as opções antes da seleção.</li> </ul> <li><strong>T3: Definir remuneração (Tarefa Interativa)</strong> O recrutador informa o valor da bolsa e os benefícios oferecidos, com validação automática.</li> <ul> <li><strong>Decomposição de T3: T3.1:</strong> Inserir valor da bolsa com máscara monetária (Usuário) |[]| T3.2: Marcar benefícios (Usuário) (a concorrência com comunicação |[]| indica que o recrutador pode preencher ambos os campos em qualquer ordem, com o sistema validando simultaneamente).</li> <li><strong>Após T3.1 e T3.2 completadas:</strong> T3.3: Sistema validar se valor > 0 (Sistema) >> T3.4: Notificar resultado (sucesso ou aviso) (Sistema) [].</li> <li><strong>Operador: [] (Escolha)</strong> Se o valor for zero, o sistema exibe um aviso sobre vaga não remunerada e solicita confirmação.</li> </ul> <li><strong>T4: Confirmar publicação (Tarefa Interativa)</strong> O recrutador revisa um resumo da vaga e confirma a publicação.</li> <ul> <li><strong>Decomposição de T4:</strong> T4.1: Acionar botão "Publicar vaga" (Usuário) >> T4.2: Sistema exibir resumo de todos os campos preenchidos (Sistema) >> T4.3: Recrutador confirmar (Usuário) ou cancelar (Usuário) [].</li> <li><strong>Operador: [] (Escolha)</strong> O recrutador pode confirmar a publicação ou cancelar e retornar à edição.</li> </ul> </ul> </div>

<a id="referencias-bibliograficas"></a>
# Referências bibliográficas:

>  [1] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Rio de Janeiro: Autopublicação, 2021.

<a id="bibliografia"></a>
## Bibliografia

> [1] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Rio de Janeiro: Autopublicação, 2021.

> DRAW.IO.  https://app.diagrams.net/?src=about#LAnalise%20de%20tarefas%20CTT.drawio#%7B%22pageId%22%3A%22-hnVmBIHt5F1DQTBS-kz%22%7D Acessado em:03/05/2026



<a id="historico-de-versoes"></a>
## Histórico de Versões

| Data | Versão | Descrição | Autor | Revisor |
| :--- | :--- | :--- | :--- | :--- |
| 03/05/2026 | 1.2 | Padronização e expansão da CTT para Assinatura Digital do TCE via Reconhecimento Facial com cenário de interação conectado à Persona 2 | Pedro Henrique | Samuel Leite |
| 01/05/2026 | 1.0 | Elaboração do artefato Técnica de coleta de dados | Samuel Leite | Mariana Martins |
| 03/05/2026 | 1.1 | Adição da CTT para Assinatura Digital do TCE via Reconhecimento Facial | Pedro Henrique | Samuel Leite |