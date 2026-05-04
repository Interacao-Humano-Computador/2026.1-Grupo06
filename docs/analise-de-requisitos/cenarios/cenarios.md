## Cenários

## Introdução

Cenários são descrições evolutivas de situações em um ambiente composto por um conjunto ordenado de interações entre seus participantes, realizadas por usuários ou sistemas externos [2]. Diante disso, os cenários são utilizados para descrever as situações de uso do sistema pelos seus usuários e os relacionamentos entre o sistema em desenvolvimento e outros sistemas externos, auxiliando no entendimento e na descoberta de novos requisitos [2]. Portanto, é uma estratégia para elicitar a parte comportamental do software [1].

## Modelo de Cenário

Existem cinco formas para se descrever cenários: texto narrativo, texto estruturado, diagramas, imagens e animações ou simulações. A forma selecionada para apresentação dos cenários presentes neste documento será a de texto estruturado, a qual se vale da utilização de linguagem natural semi-estruturada para melhor entendimento de cada cenário e validação dos requisitos por parte do cliente [2], tal modelo pode ser observado a seguir na Tabela 1.

| Elemento   | Descrição |
| ---------- | --------- |
| Objetivo   | Finalidade do cenário |
| Contexto   | Descrição de pré-condições, local (físico) e tempo |
| Recursos   | Objetos passivos com os quais os atores interagem |
| Ator       | Pessoa ou estrutura organizacional |
| Episódios  | Ação realizada por um ou vários atores com participação de outros atores utilizando recursos |
| Restrições | Imposição que restrinja um episódio de um cenário |
| Exceção    | Tratamento para uma situação excepcional ou de erro |

<div style="text-align: center">
<p>Tabela 1: Modelo texto estruturado para descrição de cenários (Fonte: [2], 2022).</p>
</div>

## Cenários identificados

Os cenários identificados foram determinados levando em consideração a Persona criada e seus objetivos. A seguir, esses podem ser observados nas tabelas abaixo:

### C01: Solicitar remanejamento escolar pelo sistema

| Elemento   | Descrição |
| ---------- | --------- |
| Objetivo   | Solicitar a reserva de vaga para transferência do filho para uma escola pública do DF mais próxima da nova residência |
| Contexto   | - Local: em casa, em Ceilândia (DF) <br> - Tempo: noite, durante o período de remanejamento (até 14 de novembro) <br> - Pré-condições: ter acesso à internet, possuir smartphone, ter em mãos os documentos exigidos (comprovante de residência, histórico escolar/DEPROV atualizado e documentos pessoais do estudante e do responsável) |
| Recursos   | - Internet <br> - Smartphone <br> - Sistema de remanejamento escolar da SEEDF <br> - Documentos digitalizados do estudante e do responsável |
| Ator       | Maria Oliveira — mãe e responsável legal do estudante |
| Episódios  | - Maria acessa o sistema de remanejamento escolar pelo smartphone <br> - Maria pesquisa escolas públicas com vagas disponíveis próximas ao seu novo endereço em Ceilândia <br> - Maria seleciona a unidade escolar de sua preferência <br> - O sistema exibe um alerta informando que o DEPROV tem validade de 30 dias e orienta Maria a verificar a data do documento antes de prosseguir <br> - Maria realiza o upload dos documentos obrigatórios: comprovante de residência, DEPROV e documentos pessoais <br> - Maria confirma a solicitação e recebe uma mensagem de confirmação de que o pedido foi registrado com sucesso <br> - Maria anota a data de divulgação do resultado (30 de dezembro) para acompanhar no site da SEEDF |
| Restrições | - O pedido só pode ser feito para uma única unidade escolar <br> - O DEPROV deve estar dentro do prazo de validade de 30 dias <br> - A solicitação deve ser concluída até o dia 14 de novembro <br> - A interface deve ser navegável e funcional em dispositivos móveis |
| Exceção    | - Falta de acesso à internet <br> - DEPROV vencido no momento do upload <br> - Ausência de vagas disponíveis na unidade desejada <br> - Falha no upload dos documentos <br> - Sistema indisponível fora do horário de pico |

### C02: Solicitar Atendimento Domiciliar pelo sistema
 
| Elemento | Descrição |
|---|---|
| Objetivo | Solicitar o atendimento pedagógico domiciliar para o filho impossibilitado de frequentar a escola por motivo de saúde |
| Contexto | - Local: em casa ou em ambiente hospitalar, em Samambaia (DF)<br>- Tempo: durante o período de afastamento médico do estudante, logo após a emissão do atestado<br>- Pré-condições: ter acesso à internet, possuir smartphone, ter em mãos o atestado médico com o período de afastamento especificado e os documentos pessoais do estudante e do responsável |
| Recursos | - Internet<br>- Smartphone<br>- Sistema de solicitação de Atendimento Domiciliar da SEEDF<br>- Atestado médico digitalizado<br>- Documentos pessoais do estudante e do responsável |
| Ator | Ana Paula Ferreira — mãe e responsável legal do estudante |
| Episódios | - Ana Paula acessa o sistema pelo smartphone e localiza a opção de solicitação de Atendimento Domiciliar<br>- O sistema exibe os critérios de elegibilidade e Ana Paula confirma que o filho se enquadra na situação prevista (tratamento de saúde prolongado com permanência em casa)<br>- O sistema orienta Ana Paula a entregar o atestado médico à direção da escola imediatamente, informando que o prazo de início do atendimento está vinculado à data de entrega do documento<br>- Ana Paula realiza o upload do atestado médico com o período de afastamento especificado<br>- Ana Paula preenche os dados do estudante e confirma a solicitação<br>- O sistema registra o pedido e exibe uma mensagem de confirmação com as próximas etapas do processo (análise pela escola e pela Coordenação Regional de Ensino)<br>- Ana Paula acompanha o andamento do pedido pelo sistema, sem precisar ligar para a secretaria escolar |
| Restrições | - O atestado médico deve conter explicitamente o período de afastamento do estudante<br>- A solicitação deve ser feita imediatamente após a emissão do atestado, pois o início do atendimento depende da data de entrega<br>- A interface deve ser navegável e funcional em dispositivos móveis, incluindo situações de conexão instável |
| Exceção | - Atestado médico sem especificação do período de afastamento<br>- Falha no upload do documento pelo celular<br>- Sistema indisponível no momento do acesso<br>- Pedido indeferido pela escola ou pela Coordenação Regional por não atendimento aos critérios<br>- Falta de acesso à internet no ambiente hospitalar |


### Cenário C03: Localização de Documentos e Unidades de Ensino Especial


| Elemento | Descrição |
| :--- | :--- |
| **Objetivo** | Obter a lista completa de documentos exigidos e identificar o endereço de uma unidade de Educação Precoce para o filho com autismo. |
| **Contexto** | **Local:** Residência da usuária, ambiente doméstico. <br> **Tempo:** Período vespertino, conciliando a busca com o cuidado de três filhos e os estudos universitários. <br> **Pré-condições:** Possuir acesso à internet e o diagnóstico médico (laudo) prévio do filho. |
| **Recursos** | Computador desktop (utilizado para garantir maior segurança na navegação), navegador web e o portal oficial da SEEDF. |
| **Ator** | **Tais:** Mãe, estudante de Biomedicina, cuidadora principal e usuária que busca eficiência tecnológica para otimizar seu tempo escasso. |
| **Episódios** | 1. Tais acessa a página inicial da SEEDF e busca visualmente pelo termo "Matrícula". <br> 2. Diante da ausência de um botão direto, ela tenta decifrar o menu "Carta de Serviços", incerta se ali encontrará os documentos para o ensino especial. <br> 3. Ao selecionar a modalidade, Tais lê as informações para identificar quais laudos médicos específicos (além da documentação civil) são obrigatórios. <br> 4. Ela localiza a listagem de escolas que oferecem "Educação Precoce", mas percebe que o sistema exibe apenas os nomes das unidades, sem endereços ou links de localização. <br> 5. Frustrada pela interrupção da tarefa, Tais copia o nome da escola e abre uma nova aba no Google para buscar o endereço físico externamente. |
| **Restrições** | O portal deve apresentar informações integradas; o endereço e telefone devem estar vinculados ao nome da unidade escolar para evitar que o usuário abandone o sistema. |
| **Exceção** | 1. Falha de comunicabilidade: A usuária não entende o termo "Carta de Serviços". <br> 2. Ruptura de informação: O portal não fornece o endereço, impossibilitando a conclusão da tarefa de forma autônoma. <br> 3. Queda de conexão ou lentidão no carregamento das listas de escolas especializadas. |


### C04: Solicitação de vaga em creche pelo sistema

| Elemento   | Descrição |
| ---------- | --------- |
| Objetivo   | Solicitar vaga em creche pública para o filho |
| Contexto   | - Local: em casa, no Distrito Federal <br> - Tempo: durante o período de inscrição <br> - Pré-condições: possuir acesso à internet, smartphone e documentos do responsável e da criança |
| Recursos   | - Internet <br> - Smartphone <br> - Página de matrícula da SEEDF <br> - Documentos pessoais |
| Ator       | Maria Aparecida — mãe e responsável legal |
| Episódios  | - Maria acessa o site da Secretaria de Educação pelo celular <br> - Maria localiza a seção de matrícula em creche <br> - Maria lê as informações disponíveis, mas encontra dificuldade devido à quantidade de texto <br> - Maria observa diferentes canais de inscrição (telefone, site e aplicativo) e fica em dúvida sobre qual escolher <br> - Maria tenta entender os próximos passos, mas precisa reler as informações <br> - Maria decide realizar a inscrição pelo canal que considera mais simples |
| Restrições | - Necessidade de acesso à internet <br> - Interface deve funcionar em dispositivos móveis <br> - Usuário deve compreender as instruções apresentadas |
| Exceção    | - Dificuldade de compreensão das informações <br> - Insegurança na escolha do canal de inscrição <br> - Falta de clareza no processo <br> - Abandono da tarefa devido à confusão |

---


### C05: Verificar Informações de Matrícula pelo Sistema

Elemento | Descrição
---------|----------
Objetivo | Consultar informações sobre matrícula escolar do filho
Contexto | - Local: em casa, no Distrito Federal  
- Tempo: durante o período de matrícula escolar  
- Pré-condições: acesso à internet e dispositivo móvel
Recursos | - Internet  
- Smartphone  
- Sistema da Secretaria de Educação  
- Painel do Usuário Educacional
Ator | Ana Souza — responsável legal pelo estudante
Episódios | - Ana acessa o sistema pelo smartphone  
- Realiza login no Painel do Usuário Educacional  
- Visualiza as opções principais do sistema  
- Seleciona a opção de matrícula  
- Acessa as informações de forma direta  
- Conclui a tarefa sem precisar navegar por várias páginas
Restrições | - Necessidade de acesso à internet  
- Interface deve ser adaptada para dispositivos móveis  
- Sistema deve apresentar informações claras e organizadas
Exceção | - Falha no acesso ao sistema  
- Lentidão na conexão  
- Informações não disponíveis ou desatualizadas  

---

### C06: Consultar Avisos Escolares pelo Sistema

Elemento | Descrição
---------|----------
Objetivo | Verificar avisos e comunicados escolares importantes
Contexto | - Local: em qualquer ambiente com acesso à internet  
- Tempo: a qualquer momento, conforme necessidade  
- Pré-condições: possuir acesso ao sistema
Recursos | - Internet  
- Smartphone  
- Sistema da Secretaria de Educação  
- Painel do Usuário Educacional
Ator | João Pereira — estudante da rede pública
Episódios | - João acessa o sistema pelo celular  
- Realiza login no Painel do Usuário Educacional  
- Visualiza a área de avisos e comunicados  
- Seleciona os avisos mais recentes  
- Obtém rapidamente as informações desejadas
Restrições | - Interface deve ser rápida e responsiva  
- Informações devem ser atualizadas constantemente  
- Layout deve facilitar leitura em dispositivos móveis
Exceção | - Sistema fora do ar  
- Avisos não atualizados  
- Falha na exibição das informações  

---

### C07: Acessar Informações Institucionais pelo Sistema

Elemento | Descrição
---------|----------
Objetivo | Acessar informações institucionais e administrativas
Contexto | - Local: ambiente de trabalho ou casa  
- Tempo: durante atividades profissionais  
- Pré-condições: acesso ao sistema
Recursos | - Internet  
- Computador ou smartphone  
- Sistema da Secretaria de Educação  
- Painel do Usuário Educacional
Ator | Carlos Mendes — professor da rede pública
Episódios | - Carlos acessa o sistema  
- Realiza login no Painel do Usuário Educacional  
- Navega pelas opções organizadas  
- Localiza rapidamente informações institucionais  
- Utiliza as informações para suas atividades profissionais
Restrições | - Sistema deve ser estável  
- Informações devem ser bem organizadas  
- A navegação deve ser intuitiva
Exceção | - Dificuldade em encontrar informações específicas  
- Sistema indisponível  
- Falhas na navegação  

---

### C08: Realizar inscrição no PEBI

| Elemento   | Descrição |
| ---------- | --------- |
| Objetivo   | Realizar a inscrição de um estudante do ensino médio no programa bilíngue |
| Contexto   | - Local: em casa ou no trabalho <br> - Tempo: durante o período oficial de matrículas <br> - Pré-condições: acesso à internet, possuir dispositivo (smartphone ou computador) e ter os documentos digitalizados |
| Recursos   | - Internet <br> - Navegador <br> - Sistema SEEDF <br> - Documentação digitalizada |
| Ator       | Joana Silva — mãe e responsável legal (Persona Primária) |
| Episódios  | - Joana acessa o portal e navega até a seção PEBI <br> - Joana seleciona uma das 4 unidades escolares disponíveis <br> - Joana insere os dados de identificação (RG/CPF) <br> - Joana realiza o upload dos 7 documentos obrigatórios <br> - O sistema fornece feedback de progresso durante o preenchimento <br> - Joana confirma a inscrição <br> - O sistema gera e exibe o protocolo de inscrição |
| Restrições | - Escolha permitida de apenas uma unidade escolar <br> - Limite de tamanho para os arquivos enviados <br> - Limite de alunos por unidade|
| Exceção    | - Falha na conexão com a internet <br> - Documentos ilegíveis ou fora do padrão exigido |


## Referências Bibliográficas

> <a id="REF1">1.</a> Slides Requisitos - aula 10. Milene Serrano e Maurício Serrano. Elicitação, modelagem e análise.

> <a id="REF2">2.</a> CENÁRIOS: Rastreamento de Cenários. Disponível em: http://www-di.inf.puc-rio.br/~julio/bnncap3.pdf. Acesso em: 02 mai. 2026.

> Cenários Lichess. Disponível em: <<https://interacao-humano-computador.github.io/2022.2-Lichess/>>. Acesso em 03 de maio de 2026.

## Histórico de versão

| Versão | Data       | Descrição             | Autor(es)                                    | Revisor(es) |
| ------ | ---------- | --------------------- | -------------------------------------------- | ----------- |
| `1.0`  | 03/05/2026 | Criação do documento  | [Ígor Veras](https://github.com/igorvdaniel) |             |
| `1.1`  | 03/05/2026 | Criação da tabela C02 | [Felipe Henrique](https://github.com/fhenrique77)|         |
| `1.2`  | 03/05/2026 | Criação da tabela C03 | [Luara Cristiana](https://github.com/luacristiana)|         |
| `1.3`  | 03/05/2026 | Criação da tabela C04 | [Giulia Paulucci](https://github.com/GiuliaPaulucci)|         |
| `1.4`  | 03/05/2026 | Criação da tabela C02 | [Joao Guilherme](https://github.com/JoaoGSantana10)|         |
| `1.5`  | 02/05/2026 | Criação da tabela C08 | [Matheus](https://github.com/matheus-06)||

