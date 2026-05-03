
## Contribuidores

| Nome do Contribuidor | Tópico desenvolvido |
| :--- |  :--- |
| Samuel Leite |  [Introdução](#introducao) <br> [Diagrama de decomposição HTA](#diagrama-hta) <br> [Tabela da Análise Hierárquica de Tarefas (HTA)](#tabela-hta) <br> [Referências Bilbiográficas](#referencias-bibliograficas) <br> [Bibliografia](#bibliografia) <br> [Histórico de versão](#historico-de-versoes) <br>| 
| Pedro Henrique | [HTA para Assinatura Digital do TCE via Reconhecimento Facial](#hta-assinatura-facial) <br> [Diagrama de decomposição HTA - Assinatura Facial](#diagrama-hta-assinatura) <br> [Tabela da Análise Hierárquica de Tarefas (HTA) - Assinatura Facial](#tabela-hta-assinatura) |


<a id="introducao"></a>
# Introdução
<div align="justify">
    A Análise Hierárquica de Tarefas (HTA - Hierarchical Task Analysis) é um método utilizado para entender as competências e habilidades exibidas em tarefas complexas e auxiliar na identificação de problemas de desempenho. O método inicia pela definição dos objetivos principais do usuário, decompondo-os em subobjetivos por meio de um desdobramento hierárquico (Barbosa, 2021).<p> <p>
    As relações entre esses subobjetivos são chamadas de "planos", que definem a ordem e a condição de execução: sequencial (indicado por >), seleção ou escolha (indicado por /) e paralelo (indicado por +). No nível mais baixo da hierarquia encontram-se as operações, que representam as ações concretas detalhadas por inputs (condições de entrada), ações e feedback (condições de atingimento do objetivo) (Barbosa, 2021).
</div>

<a id="diagrama-hta"></a>
### Diagrama de Decomposição (HTA)

0. Jornada de estágio na plataforma (1>2>3>4)
 1. Preparar perfil na plataforma (1>2+3)
    - 1.1. Criar cadastro
    - 1.2. Enviar currículo em PDF
    - 1.3. Enviar documentos pessoais
2. Encontrar e aplicar para vaga (1>2)
    - 2.1. Buscar vaga
    - 2.2. Se candidatar de forma simplificada para a vaga
3. Participar do processo seletivo (1>2>3 ou 1/2 dependendo da vaga, assumido sequencial completo)
    - 3.1. Funcionalidade de realizar prova online pela plataforma
    - 3.2. Realizar agendamento de entrevista em uma vaga disponível
    - 3.3. Realizar a entrevista dentro da plataforma
4. Formalizar a contratação
    - 4.1. Efetuar assinatura de documentos pelo GOV.BR (assinatura eletrônica)
<br><br>
<br>


<a id="tabela-hta"></a>
### Tabela da Análise Hierárquica de Tarefas (HTA)

<p> A tabela a seguir apresenta os detalhes de operações, problemas e recomendações associados ao cumprimento das tarefas.
<br>
<br>

|Objetivos/ações| Problemas e Recomendações|
|:---|:---|
|0. Jornada de estágio na plataforma | **Input:** intenção de encontrar o primeiro estágio remunerado, dados acadêmicos e currículo em mãos.<br> **Feedback:** vaga garantida e termo de estágio (TCE) assinado eletronicamente.<br> **Plano:** preparar o perfil e enviar documentação prévia, para depois encontrar vagas, realizar o processo seletivo e assinar o contrato. <br> **Recomendação:** Centralizar todo o acompanhamento das etapas em um painel único (dashboard) para que o usuário não se perca durante a jornada|
|1. Preparar perfil na plataforma 1>2+3<br>| **Plano:** criar a conta base primeiro e, em seguida, enviar o currículo e documentos pessoais em paralelo (sem ordem restrita).|
|1.1. Criar cadastro| **Problema:** a persona sente frustração em gastar tempo preenchendo formulários longos do zero para diferentes sistemas. <br> **Recomendação:** permitir cadastro facilitado importando dados (ex: "Entrar com Google" ou "Importar do LinkedIn").|
|1.2. Enviar currículo em PDF| **Recomendação:** utilizar ferramenta de extração de dados do PDF para preencher automaticamente os campos de habilidades e experiências no perfil do usuário, poupando tempo |
|1.3. Enviar documentos pessoais| **Problema:** Falhas ou lentidão no upload. <br> **Recomendação:** mostrar claramente os formatos aceitos e limite de tamanho, e dar feedback visual (ex: barra de progresso) durante o envio.|
|2. Encontrar e aplicar para vaga 1>2<br>| **Plano:** Buscar a vaga usando filtros e, ao encontrar o match ideal, candidatar-se.|
|2.1. Buscar vaga| **Recomendação:** Disponibilizar filtros avançados (ex: por localidade, formato home-office, valor da bolsa-auxílio) para alinhar à expectativa de uma busca rápida e assertiva.|
|2.2. Se candidatar de forma simplificada para a vaga| **Problema:** Necessidade de criar cadastros diferentes por vaga, o que desmotiva a persona. <br> **Ação:** o sistema utiliza os dados do objetivo 1 para submeter o perfil instantaneamente.<br> **Recomendação:** habilitar botão "Candidatura simplificada" que dispensa novos preenchimentos.|
|3. Participar do processo seletivo 1>2>3<br>|**Plano:** realizar a prova técnica, agendar uma entrevista e depois realizar a entrevista.|
|3.1. Funcionalidade de realizar prova online pela plataforma| **Problema:** queda de conexão durante a prova ou fechamento acidental da aba.<br> **Recomendação:** salvar o progresso das questões automaticamente a cada minuto |
|3.2. Realizar agendamento de entrevista em uma vaga disponível| **Recomendação:** sincronizar opções de horários com a agenda do recrutador e permitir que o estudante escolha seu horário com poucos cliques, recebendo um lembrete (notificação/e-mail)|
|3.3. Realizar a entrevista dentro da plataforma| **Problema:** O usuário pode ter problemas com permissões de áudio/vídeo no navegador.<br> **Recomendação:** apresentar uma "sala de espera" para testar microfone e câmera antes de entrar definitivamente na chamada.|
|4. Formalizar a contratação||
|4.1. Efetuar assinatura de documentos pelo GOV.BR (assinatura eletrônica)| **Problema:** o usuário pode sair da plataforma de estágio e não saber como voltar após assinar no GOV.BR.<br> **Recomendação:** usar um fluxo de redirecionamento transparente que, ao finalizar a assinatura no ambiente do governo, traga o usuário de volta para a tela de confirmação de "Termo Assinado com sucesso".|

<br>
<br>
<br>

<a id="hta-assinatura-facial"></a>
# HTA para Assinatura Digital do TCE via Reconhecimento Facial

<div align="justify">
    Esta seção apresenta a Análise Hierárquica de Tarefas (HTA) específica para a nova funcionalidade de Assinatura Digital do Termo de Compromisso de Estágio (TCE) via Reconhecimento Facial no sistema Super Estágios. A funcionalidade visa reduzir a carga cognitiva do usuário ao substituir a memorização de senhas por uma operação física rápida, utilizando as capacidades biométricas dos smartphones modernos. Baseado na teoria de Annett e Duncan, a decomposição hierárquica identifica objetivos, subobjetivos, operações e planos, com foco em inputs, ações, feedback e problemas/recomendações para cada etapa crítica.
</div>

<a id="diagrama-hta-assinatura"></a>
### Diagrama de Decomposição (HTA) - Assinatura Facial

0. Assinar o TCE digitalmente (1>2>3>4>5)
 1. Selecionar método de assinatura
 2. Solicitar permissão para câmera (2.1>2.2)
    - 2.1. Exibir popup de solicitação de permissão
    - 2.2. Usuário conceder permissão para câmera frontal
 3. Posicionar rosto para captura (3.1+3.2)
    - 3.1. Ajustar posição do rosto no enquadramento
    - 3.2. Sistema fornecer guia visual em tempo real
 4. Processar validação facial
 5. Fornecer feedback (5.1/5.2)
    - 5.1. Exibir confirmação de sucesso na autenticação
    - 5.2. Exibir alerta para tentar novamente em caso de falha

<a id="tabela-hta-assinatura"></a>
### Tabela da Análise Hierárquica de Tarefas (HTA) - Assinatura Facial

<p> A tabela a seguir apresenta os detalhes de operações, problemas e recomendações associados à funcionalidade de assinatura digital via reconhecimento facial.
<br>
<br>

|Objetivos/ações| Problemas e Recomendações|
|:---|:---|
|0. Assinar o TCE digitalmente | **Input:** Chegada na etapa de assinatura do contrato no processo de contratação.<br> **Ação:** Usuário seleciona método de assinatura e completa o processo biométrico.<br> **Feedback:** Confirmação visual de assinatura autenticada com sucesso ou alerta para tentar novamente.<br> **Plano:** Sequencial: selecionar método, solicitar permissão, posicionar rosto, processar validação e fornecer feedback. <br> **Recomendação:** Garantir que o processo seja rápido (menos de 30 segundos) para manter a eficiência e reduzir frustração.|
|1. Selecionar método de assinatura| **Input:** Tela de assinatura do TCE exibida.<br> **Ação:** Usuário toca na opção 'Assinar com Biometria Facial'.<br> **Feedback:** Destaque visual da opção selecionada.<br> **Problema:** Usuário pode não perceber a opção se não estiver bem destacada.<br> **Recomendação:** Posicionar a opção de biometria facial como padrão ou primeira escolha, com ícone intuitivo de câmera/rosto.|
|2. Solicitar permissão para câmera 2.1>2.2<br>| **Plano:** Exibir popup primeiro, então aguardar concessão da permissão.|
|2.1. Exibir popup de solicitação de permissão| **Input:** Seleção do método de assinatura.<br> **Ação:** Sistema mostra popup pedindo acesso à câmera frontal.<br> **Feedback:** Popup visível com explicação breve.<br> **Problema:** Popup pode ser bloqueado por navegador ou dispositivo.<br> **Recomendação:** Garantir compatibilidade com navegadores móveis e fornecer instruções alternativas.|
|2.2. Usuário conceder permissão para câmera frontal| **Input:** Popup exibido.<br> **Ação:** Usuário clica em "Permitir".<br> **Feedback:** Câmera ativada e tela de captura exibida.<br> **Problema:** Usuário nega permissão.<br> **Recomendação:** Oferecer fallback para método alternativo (ex: senha) e explicar benefícios da biometria.|
|3. Posicionar rosto para captura 3.1+3.2<br>| **Plano:** Ajuste de posição e guia ocorrem em paralelo para orientação em tempo real.|
|3.1. Ajustar posição do rosto no enquadramento| **Input:** Permissão concedida.<br> **Ação:** Usuário move o dispositivo ou rosto para alinhar com o oval na tela.<br> **Feedback:** Oval muda de cor (ex: vermelho para verde) quando alinhado.<br> **Problema:** Dificuldade em alinhamento devido a movimento ou iluminação.<br> **Recomendação:** Permitir captura automática quando alinhado, com tolerância a pequenos movimentos.|
|3.2. Sistema fornecer guia visual em tempo real| **Input:** Rosto detectado.<br> **Ação:** Sistema exibe instruções dinâmicas (ex: "Aproxime mais", "Centralize o rosto").<br> **Feedback:** Texto e ícones atualizados conforme posição.<br> **Problema:** Guias confusas podem frustrar o usuário.<br> **Recomendação:** Usar linguagem simples e ícones universais; testar com usuários para clareza.|
|4. Processar validação facial| **Input:** Imagem capturada.<br> **Ação:** Sistema processa validação dos pontos focais em background.<br> **Feedback:** Indicador de processamento (ex: spinner "Processando...").<br> **Problema:** Falha na validação devido a óculos, barba ou similaridade com outras faces.<br> **Recomendação:** Usar algoritmos robustos; permitir tentativas múltiplas com feedback específico (ex: "Remova óculos para melhor precisão").|
|5. Fornecer feedback 5.1/5.2<br>| **Plano:** Seleção baseada no resultado da validação: sucesso ou falha.|
|5.1. Exibir confirmação de sucesso na autenticação| **Input:** Validação bem-sucedida.<br> **Ação:** Sistema mostra ícone de check e mensagem de sucesso.<br> **Feedback:** TCE assinado digitalmente.<br> **Problema:** Nenhum específico, mas garantir persistência.<br> **Recomendação:** Armazenar assinatura de forma segura e enviar confirmação por e-mail.|
|5.2. Exibir alerta para tentar novamente em caso de falha| **Input:** Validação falhada.<br> **Ação:** Sistema mostra ícone de alerta e botão "Tentar Novamente".<br> **Feedback:** Redirecionamento para nova tentativa.<br> **Problema:** Falhas repetidas podem desmotivar.<br> **Recomendação:** Limitar tentativas (ex: 3) e oferecer alternativa após falhas.|

<br>
<br>
<br>
# Referências bibliográficas:

>  [1] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Rio de Janeiro: Autopublicação, 2021.

<a id="bibliografia"></a>
## Bibliografia

> [1] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Rio de Janeiro: Autopublicação, 2021.

<br>
<br>
<br>


<a id="historico-de-versoes"></a>
## Histórico de Versões

| Data | Versão | Descrição | Autor | Revisor |
| :--- | :--- | :--- | :--- | :--- |
| 01/05/2026 | 1.0 | Elaboração do artefato Técnica de coleta de dados | Samuel Leite | Mariana Martins |
| 03/05/2026 | 1.1 | Adição da HTA para Assinatura Digital do TCE via Reconhecimento Facial | Pedro Henrique | Samuel Leite |