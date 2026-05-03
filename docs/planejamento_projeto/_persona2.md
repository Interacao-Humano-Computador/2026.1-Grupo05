## Contribuidores

| Nome do Contribuidor | Tópico desenvolvido |
| :--- |  :--- |
| Pedro Henrique |  [Introdução](#introducao) <br> [Identidade Persona 2](#identidade-persona2) <br> [Cenário Persona 2](#cenario-persona2) <br> [Referências Bibliográficas](#referencias-bibliograficas) <br> [Bibliografia](#bibliografia) <br> [Histórico de versão](#historico-de-versoes) <br>| | | 

<a id="introducao"></a>
# Introdução
<div align="justify">
    O método para definição de personas apresentado no Capítulo 8 baseia-se na criação de personagens fictícios que funcionam como arquétipos hipotéticos de grupos de usuários reais. O objetivo dessa abordagem é evitar o conceito genérico e impreciso de um "usuário elástico", que obriga o usuário a se contorcer para se adaptar ao sistema. Em vez disso, a construção de uma persona foca em projetar interações para alvos muito específicos (Barbosa, 2021). <p><p>
    O método consiste em um processo de refinamentos sucessivos baseados na investigação inicial do domínio, no qual a persona ganha uma solidez tangível ao ser detalhada com elementos característicos fundamentais Para estruturá-la corretamente, o livro indica o preenchimento dos seguintes atributos: identidade (nome, dados demográficos e foto), status (se é uma persona primária, secundária ou antiusuário), objetivos (finais, instrumentais e de vida), habilidades, tarefas principais, relacionamentos, requisitos e expectativas. <p>
    A literatura recomenda que a equipe defina um elenco reduzido e memorável de personas (geralmente em torno de três personas primárias), utilizando-as ativamente como ferramentas de comunicação para guiar reuniões, avaliações e a tomada de decisão no projeto de IHC. <p>
    A seguir temos a descrição de identidade e persona.
</div>

<a id="identidade-persona2"></a>
### Identidade:
- Foto:
<div align="center">
  <img src="assets\Persona2.png" width="150">
</div>
<div align="center"> <p> <i><b>Figura 1:</b> Representação de uma persona (Fonte: https://thispersondoesnotexist.com/ acessado em: 02/05/2026).</i> </p> </div>

- **Nome:** Lourdes
- **Sobrenome:** Ribeiro Campos
- **Idade:** 50
- **Sexo:** Feminino
- **Gênero:** Cisgênero
- **Escolaridade:** Superior Completa
- **Cargo Atual:** Proprietária de Microempresa
- **Área de formação:** Administração
- **Status:** Persona Secundária
- **Objetivos gerais:** Identificar novos talentos para a empresa, formar mão de obra qualificada e cumprir obrigações legais de estágio.
    - **Objetivos de vida:** 
        - Contribuir para o aprendizado social e profissional de jovens, promovendo inclusão.
    - **Objetivos finais (práticos):** 
        - Publicar vagas com requisitos específicos, selecionar candidatos alinhados e gerenciar documentação.
        - Garantir conformidade com a Lei do Estágio e oferecer ambiente de aprendizagem.
    - **Objetivos instrumentais (experiência):**
        - Utilizar dashboards visuais para filtrar currículos e acompanhar processos de contratação.
- **Habilidades:** Experiência em gestão de microempresa, conhecimento em RH básico, familiaridade com leis trabalhistas e plataformas digitais.
- **Tarefas:**
    - **Básicas:** Descrever atividades de vagas, publicar no Super Estágios e revisar candidaturas.
    - **Críticas:** Filtrar candidatos por curso e localidade, convocar para entrevistas e validar TCE.
    - **Frequência:** Semanal, conforme necessidades de contratação.
- **Relacionamentos:** Se relaciona com estudantes candidatos, supervisores internos e suporte da plataforma.
- **Requisitos:** Interface web com dashboards para múltiplas vagas, filtros por curso/semestre/localidade e notificações de vencimento de contratos.
- **Expectativas:** Espera que a plataforma reduza triagens manuais, automatize encontros entre perfil acadêmico e necessidade técnica, transmitindo autoridade legal.


### Lourdes Ribeiro, Proprietária de Microempresa - "Eficiência no recrutamento de estagiários"

<div align="justify">
Persona: Lourdes Ribeiro Campos – "Gestora focada em formação profissional" <p> Lourdes tem 50 anos e é proprietária de uma microempresa no setor de serviços. Com formação em Administração, ela busca estagiários para integrar sua equipe e contribuir para o desenvolvimento de jovens. Seu foco é contratar candidatos que se adaptem à cultura da empresa e atendam às necessidades técnicas, garantindo conformidade com leis trabalhistas. <p> Lourdes utiliza o Super Estágios para publicar vagas e gerenciar seleções de forma eficiente. Ela valoriza ferramentas que automatizam triagens e facilitam a validação de documentos, permitindo que ela se concentre em entrevistas e no crescimento da empresa. Sua expectativa é que a plataforma transmita autoridade legal e reduza burocracias, promovendo um recrutamento produtivo e inclusivo.
</div>    

#### Objetivos de vida:
- Apoiar o aprendizado profissional de estudantes e fortalecer a empresa com novos talentos.

#### Objetivos finais e instrumentais:
- Publicar vagas detalhadas com requisitos específicos e valores de bolsa-auxílio.
- Selecionar candidatos alinhados ao perfil acadêmico e cultural da empresa.
- Gerenciar contratos de estágio e relatórios de atividades de forma digital.

<a id="cenario-persona2"></a>
## Cenário de Interação: Seleção e formalização de estágio com reconhecimento facial

Atores: Lourdes Ribeiro (proprietária de microempresa), Candidato Estudante (estudante de Administração), Suporte da Plataforma Super Estágios.

<div align="justify"; style="font-style: italic;">
    "Em uma quarta-feira à noite, Lourdes acessa o Super Estágios no seu smartphone para dar continuidade ao processo de seleção. Ela navega pelo dashboard de candidatos e encontra um estudante de Administração do 5º semestre que se destaca pelo desempenho em sua entrevista. Após revisar o currículo e as notas da entrevista (conforme as tarefas descritas em <a href='_analiseTarefasHTA.md#hta-assinatura-facial'>HTA - Assinatura Facial (Objetivo 3 e 4)</a>), ela aprova o candidato para a etapa final: <strong>formalização da contratação com assinatura biométrica do TCE</strong>. <p> <p> Lourdes envia ao candidato um link para iniciar o processo de assinatura digital. No dia seguinte, o candidato recebe a notificação e acessa o Super Estágios. O sistema apresenta o Termo de Compromisso de Estágio (TCE) na tela e oferece duas opções: assinar com senha tradicional (GOV.BR) ou com <strong>Reconhecimento Facial</strong>. O candidato seleciona a opção biométrica, conforme descrito na <a href='_analiseTarefasCTT.md#ctt-assinatura-facial'>CTT - Assinatura Facial (T₁.₁ - Selecionar biometria facial)</a>. <p> <p> <strong>Processo de Validação Facial:</strong> O sistema solicita permissão para acessar a câmera frontal do smartphone (<a href='_analiseTarefasHTA.md#hta-assinatura-facial'>HTA 2.1 e 2.2</a>). Após concessão, o candidato é guiado a posicionar seu rosto dentro do enquadramento visual (<a href='_analiseTarefasHTA.md#hta-assinatura-facial'>HTA 3.1 e 3.2</a>). Quando o rosto está corretamente posicionado, o sistema captura a imagem e processa a validação biométrica em background (<a href='_analiseTarefasHTA.md#hta-assinatura-facial'>HTA 4.0</a>). Em menos de 10 segundos, a validação é concluída e a assinatura é registrada no sistema. <p> <p> <strong>Confirmação em Dashboard de Lourdes:</strong> Quando o candidato completa a assinatura facial com sucesso (<a href='_analiseTarefasHTA.md#hta-assinatura-facial'>HTA 5.1</a>), Lourdes recebe uma notificação no seu dashboard: <em>"TCE do candidato assinado e validado com sucesso via reconhecimento facial"</em>. Ela visualiza o status atualizado do contrato, contendo a confirmação de autenticação biométrica, data/hora e validade. O processo, que anteriormente exigia redirecionamento manual para o GOV.BR e retorno à plataforma, agora ocorre de forma integrada e segura em uma única jornada (<a href='_analiseTarefasCTT.md#ctt-assinatura-facial'>conforme CTT T₄ - Formalizar Contratação</a>). <p> <p> Satisfeita com a eficiência e segurança do processo, Lourdes finaliza a contratação e envia um e-mail de boas-vindas ao novo estagiário. A plataforma automaticamente: (1) registra o TCE assinado no sistema de documentação, (2) sincroniza a informação com os órgãos reguladores (se aplicável), e (3) ativa o acesso do estagiário ao ambiente de trabalho colaborativo. Lourdes percebe que a integração do reconhecimento facial otimizou a experiência, reduzindo tempo burocrático e aumentando a confiança na autenticidade do contrato."
</div>

<a id="referencias-bibliograficas"></a>
# Referências bibliográficas:

>  [1] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Rio de Janeiro: Autopublicação, 2021.

<a id="bibliografia"></a>
## Bibliografia

> [1] BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. **Interação Humano-Computador e Experiência do Usuário**. 1. ed. Rio de Janeiro: Autopublicação, 2021.



<a id="historico-de-versoes"></a>
## Histórico de Versões

| Data | Versão | Descrição | Autor | Revisor |
| :--- | :--- | :--- | :--- | :--- |
| 03/05/2026 | 1.4 | Integração do cenário com reconhecimento facial e conexão com análises HTA e CTT para assinatura biométrica do TCE | Pedro Henrique | Samuel Leite |
| 03/05/2026 | 1.3 | Alinhamento da Persona 2 com perfil da empresa, atualização de identidade, objetivos e cenário | Pedro Henrique | Samuel Leite |
| 02/05/2026 | 1.2 | Modificação do cenário da Persona 2 para foco em recrutamento inclusivo | Pedro Henrique | Samuel Leite |

## Colaboradores

<div align="center">
  <p style="font-size: 0.9em; font-style: italic;">Pedro Henrique</p>
</div>
<div align="center">
  <p style="font-size: 0.9em; font-style: italic;">Samuel Leite</p>
</div></content>
