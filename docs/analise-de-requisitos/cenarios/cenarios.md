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
| **Objetivo** | Solicitar o atendimento pedagógico domiciliar para o filho impossibilitado de frequentar a escola por motivo de saúde |
| **Contexto** | - Local: em casa ou em ambiente hospitalar, em Samambaia (DF)<br>- Tempo: durante o período de afastamento médico do estudante, logo após a emissão do atestado<br>- Pré-condições: ter acesso à internet, possuir smartphone, ter em mãos o atestado médico com o período de afastamento especificado e os documentos pessoais do estudante e do responsável |
| **Recursos** | - Internet<br>- Smartphone<br>- Sistema de solicitação de Atendimento Domiciliar da SEEDF<br>- Atestado médico digitalizado<br>- Documentos pessoais do estudante e do responsável |
| **Ator** | Ana Paula Ferreira — mãe e responsável legal do estudante |
| **Episódios** | - Ana Paula acessa o sistema pelo smartphone e localiza a opção de solicitação de Atendimento Domiciliar<br>- O sistema exibe os critérios de elegibilidade e Ana Paula confirma que o filho se enquadra na situação prevista (tratamento de saúde prolongado com permanência em casa)<br>- O sistema orienta Ana Paula a entregar o atestado médico à direção da escola imediatamente, informando que o prazo de início do atendimento está vinculado à data de entrega do documento<br>- Ana Paula realiza o upload do atestado médico com o período de afastamento especificado<br>- Ana Paula preenche os dados do estudante e confirma a solicitação<br>- O sistema registra o pedido e exibe uma mensagem de confirmação com as próximas etapas do processo (análise pela escola e pela Coordenação Regional de Ensino)<br>- Ana Paula acompanha o andamento do pedido pelo sistema, sem precisar ligar para a secretaria escolar |
| **Restrições** | - O atestado médico deve conter explicitamente o período de afastamento do estudante<br>- A solicitação deve ser feita imediatamente após a emissão do atestado, pois o início do atendimento depende da data de entrega<br>- A interface deve ser navegável e funcional em dispositivos móveis, incluindo situações de conexão instável |
| **Exceção** | - Atestado médico sem especificação do período de afastamento<br>- Falha no upload do documento pelo celular<br>- Sistema indisponível no momento do acesso<br>- Pedido indeferido pela escola ou pela Coordenação Regional por não atendimento aos critérios<br>- Falta de acesso à internet no ambiente hospitalar |

## Referências Bibliográficas

> <a id="REF1">1.</a> Slides Requisitos - aula 10. Milene Serrano e Maurício Serrano. Elicitação, modelagem e análise.

> <a id="REF2">2.</a> CENÁRIOS: Rastreamento de Cenários. Disponível em: http://www-di.inf.puc-rio.br/~julio/bnncap3.pdf. Acesso em: 02 mai. 2026.

> Cenários Lichess. Disponível em: <<https://interacao-humano-computador.github.io/2022.2-Lichess/>>. Acesso em 03 de maio de 2026.

## Histórico de versão

| Versão | Data       | Descrição             | Autor(es)                                    | Revisor(es) |
| ------ | ---------- | --------------------- | -------------------------------------------- | ----------- |
| `1.0`  | 03/05/2026 | Criação do documento  | [Ígor Veras](https://github.com/igorvdaniel) |             |
| `1.1`  | 03/05/2026 | Criação da tabela C02 | [Felipe Henrique](https://github.com/fhenrique77)|         |
