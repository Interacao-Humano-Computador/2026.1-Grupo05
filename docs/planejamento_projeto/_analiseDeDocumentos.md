# Análise de Documentos – Super Estágios

| Nome do Contribuidor |
| :--- |
| [Mariana Martins](https://github.com/Marianamrts) | 
| [Samuel Leite](https://github.com/osamuelleite) |

## Introdução

A análise de documentos é uma técnica de elicitação de requisitos na 
qual o analista coleta documentos existentes relacionados ao sistema e 
os lê com o objetivo de obter informações e um melhor entendimento 
sobre o domínio, os usuários e os requisitos do sistema (VAZQUEZ; 
SIMÕES, 2016). A técnica foi aplicada seguindo três etapas:

- **Preparação:** identificação dos documentos relevantes disponíveis 
no portal Super Estágios e na legislação vigente;
- **Execução:** leitura e análise de cada documento, extraindo 
requisitos do sistema;
- **Finalização:** documentação dos requisitos identificados, 
apresentada nas seções a seguir.

Os documentos analisados foram: a Política de Privacidade do Super 
Estágios, a Política de Tratamento de Dados, a Cartilha da Lei do 
Estágio (Lei nº 11.788/2008) e a Lei Geral de Proteção de Dados 
Pessoais (Lei nº 13.709/2018 — LGPD).

## Análise

### Documento 1 – Política de Privacidade (superestagios.com.br)

**Descrição do documento:** Documento que descreve quais dados 
pessoais dos usuários são coletados pela plataforma, com qual 
finalidade e como são armazenados e compartilhados.

**Requisitos identificados:**

- O sistema deve solicitar o consentimento explícito do usuário 
antes de coletar seus dados pessoais, conforme previsto na Política 
de Privacidade da plataforma;
- O sistema deve garantir que os dados dos usuários sejam 
armazenados em ambiente seguro e controlado;
- O sistema deve permitir que o usuário acesse, corrija ou solicite 
a exclusão de seus dados pessoais diretamente na área logada da 
plataforma;
- O sistema deve notificar os usuários afetados em caso de 
identificação de violação de dados pessoais;
- O sistema não deve compartilhar dados pessoais dos usuários com 
terceiros, exceto nos casos previstos na Política de Privacidade ou 
na legislação aplicável.

---

### Documento 2 – Política de Tratamento de Dados 
(superestagios.com.br)

**Descrição do documento:** Documento que detalha as bases legais 
utilizadas para o tratamento de dados pessoais dos usuários, em 
conformidade com a LGPD (Lei nº 13.709/2018).

**Requisitos identificados:**

- O sistema deve tratar os dados pessoais dos usuários respeitando 
os princípios da finalidade, adequação e necessidade previstos na 
LGPD;
- O sistema deve permitir que o usuário solicite a confirmação de 
existência de seus dados pessoais na plataforma;
- O sistema deve registrar e manter o histórico de consentimento 
do usuário para fins de auditoria e conformidade legal;
- O acesso interno aos dados dos usuários deve ser restrito apenas 
a profissionais devidamente autorizados pela Super Estágios;
- O sistema deve disponibilizar um canal de contato para 
solicitações, dúvidas e pedidos dos titulares de dados, conforme 
exigido pelo art. 41 da LGPD.

---

### Documento 3 – Cartilha da Lei do Estágio 
(Lei nº 11.788/2008)

**Descrição do documento:** Cartilha publicada pelo Ministério do 
Trabalho e Emprego que explica os direitos e obrigações dos 
estagiários, empresas e instituições de ensino com base na Lei do 
Estágio.

**Requisitos identificados:**

- O sistema deve exibir a carga horária de cada vaga, que não pode 
ultrapassar 6 horas diárias e 30 horas semanais, conforme o 
art. 10 da Lei nº 11.788/2008;
- O sistema deve indicar nas vagas se o estágio é obrigatório ou 
não obrigatório, pois as regras de bolsa e seguro diferem entre 
os dois tipos;
- O sistema deve registrar o vínculo entre estudante, empresa e 
instituição de ensino, pois a lei exige a celebração de Termo de 
Compromisso entre as três partes;
- O sistema deve informar ao estudante que o estágio não 
obrigatório exige pagamento de bolsa e auxílio-transporte 
obrigatórios;
- O sistema deve registrar o prazo máximo do estágio, que não 
pode exceder 2 anos na mesma empresa, conforme o art. 11 da 
Lei nº 11.788/2008;
- O sistema deve garantir que estudantes com deficiência tenham 
acesso às vagas, sem qualquer tipo de restrição discriminatória, 
conforme previsto na legislação.

---

### Documento 4 – Lei Geral de Proteção de Dados Pessoais 
(Lei nº 13.709/2018 — LGPD)

**Descrição do documento:** Lei federal brasileira que regula o 
tratamento de dados pessoais por pessoas físicas e jurídicas, com 
o objetivo de proteger os direitos fundamentais de liberdade e 
privacidade.

**Requisitos identificados:**

- O sistema deve coletar apenas os dados pessoais estritamente 
necessários para a finalidade declarada (princípio da necessidade);
- O sistema deve apresentar ao usuário, de forma clara e acessível, 
a finalidade do tratamento de seus dados antes da coleta;
- O sistema deve permitir que o usuário revogue seu consentimento 
a qualquer momento, com a consequente exclusão dos dados coletados 
com base nesse consentimento;
- O sistema deve garantir a portabilidade dos dados do usuário 
mediante solicitação;
- O sistema deve manter um Encarregado de Proteção de Dados (DPO) 
identificável e acessível ao usuário para esclarecimentos sobre 
o tratamento de dados.

## Conclusão

<div align="justify">

A análise dos documentos disponíveis no portal Super Estágios e 
da legislação aplicável ao contexto de estágios revelou um conjunto 
de requisitos funcionais e não funcionais que o sistema deve 
atender. Os requisitos mais críticos estão relacionados à proteção 
de dados pessoais dos usuários, em conformidade com a LGPD, e ao 
respeito às regras estabelecidas pela Lei do Estágio, especialmente 
no que diz respeito à carga horária, prazo máximo, obrigatoriedade 
de bolsa e formalização do vínculo de estágio por meio do Termo de 
Compromisso.

</div>

## Bibliografia

> VAZQUEZ, Carlos Eduardo; SIMÕES, Guilherme Siqueira. 
> **Engenharia de Requisitos: Software Orientado ao Negócio**. 
> Rio de Janeiro: Brasport, 2016. Capítulo 7, Seção 7.3 – 
> Técnica: Análise de Documentos.

> SUPER ESTÁGIOS. **Política de Privacidade**. Disponível em: 
> https://www.superestagios.com.br/index/politica-privacidade-se.pdf. 
> Acesso em: 03/05/2026.

> SUPER ESTÁGIOS. **Política de Tratamento de Dados**. Disponível 
> em: https://www.superestagios.com.br/index/politica-tratamento-dados.pdf. 
> Acesso em: 03/05/2026.

> BRASIL. Ministério do Trabalho e Emprego. **Cartilha Esclarecedora 
> sobre a Lei do Estágio: Lei nº 11.788/2008**. Brasília: MTE, 2008. 
> Disponível em: 
> https://s3-web.superestagios.com.br/web/arquivos/cartilha_lei_estagio.pdf. 
> Acesso em: 03/05/2026.

> BRASIL. **Lei nº 13.709, de 14 de agosto de 2018**. Lei Geral de 
> Proteção de Dados Pessoais (LGPD). Brasília: Presidência da 
> República, 2018. Disponível em: 
> https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/l13709.htm. 
> Acesso em: 03/05/2026.

## Histórico de Versões

| Data | Versão | Descrição | Autor | Revisor |
|------|--------|-----------|-------|---------|
| 03/05/2026 | `1.0` | Criação do artefato de análise de documentos | Luís Gustavo | Mariana Martins |