
## Contribuidores

| Nome do Contribuidor | Tópico desenvolvido |
| :--- |  :--- |
| Samuel Leite |  [Introdução](#introducao) <br> [Árvores de Tarefas Concorrentes (ConcurTaskTrees– CTT)](#analise-ctt) <br> [Diagrama da Análise de tarefas concorrentes (ConcurTaskTrees–CTT)](#diagrama-ctt) <br> [Referências Bilbiográficas](#referencias-bibliograficas) <br> [Bibliografia](#bibliografia) <br> [Histórico de versão](#historico-de-versoes) <br>|


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
| 01/05/2026 | 1.0 | Elaboração do artefato Técnica de coleta de dados | Samuel Leite | Mariana Martins |