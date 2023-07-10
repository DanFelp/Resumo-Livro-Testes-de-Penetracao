# Testes de Invasão - Uma introdução prática ao Hacking

## Capítulo 0 - Introdução aos testes de invasão

### Fases de um teste de invasão

- Fase de preparação (pre-engagement) - Conversar com o cliente para entender o planejamento.
  
  - Quando o pentester e o cliente chegarem a um acordo sobre o escopo e outros assuntos, o teste tem início.
    

- Fase de coleta de informações (information-gathering), o pentester procura informações publicamente disponíveis sobre o cliente e identifica formas de conectar-se em seus sistemas.
  

- Fase de modelagem de ameaças (threat-modeling) - O pentester usa essas informações para determinar o valor de cada descoberta e o impacto sobre o cliente.
  
  - Permite desenvolver um plano de ação e método de ataque
    

Antes que um pentester ataque um sistema, ele executa uma **Análise de Vulnerabilidade**, onde se procura vulnerabilidades para serem exploradas na fase de exploração de falhas.

Um exploit bem sucedido pode conduzir a uma fase de pós exploração de falhas (post explotaition)

- Fase de geração de relatório (reporting), onde o pentester sintetiza as informações para os executivos quanto para os técnicos.
  

"Um bom local para informações sobre pentest é: www.pentest-standard.org"

### Preparação

A falha de comunicação entre um pentester e um cliente que espera uma análise pode levar a uma situação complicada, pois os testes são mais intrusivos.

- É o primeiro teste de invasão?
  
- O que levou a procurar um pentest?
  
- Quais as exposições que eles mais temem?
  
- Existe algum dispositivo frágil que deverá ter cuidado ao efetuar os testes?
  
- O que é mais importante para o cliente?
  

### Escopo

- Quais endereços IP estão incluídos no escopo e quais não estão?
  
- Quais tipos de ações podem ser realizadas?
  
- Tem permissão para utilizar exploits e desativar potencialmente um serviço?
  
- Deve limitar a avaliação a simplesmente detectar possíveis vulnerabilidades?
  
- Mesmo um simples scan de portas pode desativar um servidor ou um roteador?
  
- Tem permissão para realizar ataques de engenharia social?
  

### Janelas de testes

O cliente pode requerer que sejam realizados testes somente em horários específicos.

### Informações de contato

- Quem contatar caso derrube algo sério?
  
- O cliente espera que você entre em contato com alguém 24 horas por dia?
  
- Eles preferem que você use criptografia nos emails?
  

### Cartão para "sair da cadeira livremente"

Certifique-se que possua autorização para realizar um teste de invasão no alvo.

- Se um alvo não pertence à empresa, não esqueça de verificar se o cliente tem aprovação formal do terceiro para realizar o teste de invasão.
  
- Certifique-se que o seu contrato inclua uma cláusula que limite a sua responsabilidade nos casos que algo inesperado aconteça, e obtenha permissão por escrito para realizar o teste.
  

### Termos de pagamento

- Como e quando será pago?
  
- Qual o valor?
  

Por fim, inclua uma cláusula para um acordo de confidencialidade em seu contrato.

- Os clientes irão apreciar o seu comprometimento por escrito para manter o teste de invasão e qualquer descoberta confidenciais.
  

### Coleta de informações

Durante essa fase, você analisará livremente as fontes de informações disponíveis.

Esse processo é conhecido como OSINT (Open Source Intelligence)

Também usará ferramentas como scanners de porta para ter uma ideia de quais sistemas estão presentes na Internet ou na rede interna, bem como quais softwares estão sendo executados.

### Modelagem de ameaças.

Com o conhecimento da fase de ameaças, pensaremos como os invasores e desenvolveremos planos de ataque de acordo com as informações coletadas.

De acordo com os dados encontrados durante a fase de coleta de informações, desenvolveremos estratégias para invadir os sistemas de um cliente.

### Análise de vulnerabilidade

Nessa fase, os pentesters executam scanners de vulnerabilidades, que usam banco de dados de vulnerabilidades e uma série de verificações ativas para obter um palpite melhor a respeito de quais vulnerabilidade estão presentes no sistema de um cliente.

Embora os scanners de vulnerabilidades sejam ferramentas eficazes, não podem substituir o raciocínio crítico, portanto, realiza-se também análises manuais e verifica-se resultados por conta própria.

### Exploração de falhas

Nessa etapa, executa-se vulnerabilidades descobertas (usando ferramentas, como o metasploit) em uma tentativa de acessar os sistemas de um cliente.

### Pré-exploração de falhas

Você entrou no sistema, mas o que essa invasão significa? Invadir um sistema legado (sem patches), que não faça parte de um domínio ou que não esteja ligado a alvos muito valiosos, e esse sistema não contiver nenhuma informação que interesse a um invasor, o risco dessa vulnerabilidade será significativamente menor do que você pudesse explorar um controlador de domínio ou um sistema de desenvolvimento de um cliente.

Nessa fase, reune-se informações importantes, tenta-se elevar o nível dos privilégios, etc.

### Geração de relatórios

Última etapa, onde se informa as descobertas ao cliente de maneira significativa.

- O que está sendo feito corretamente
  
- Os pontos que devem melhorar
  
- A postura quanto a segurança
  
- Como se conseguiu invadir
  
- O que se descobriu
  
- Como corrigir os problemas
  
- E outros
  

É necessário prática para escrever bons relatórios, para informar de forma clara a todos, da equipe de TI responsável para correção de vulnerabilidades até a alta gerência que aprova as alterações junto aos auditores externos.

O relatório do teste de invasão deve incluir tanto um sumário executivo quanto um relatório técnico.

### Sumário executivo

O Sumário executivo descreve os objetivos do teste e oferece uma visão geral das descobertas.

O público-alvo que se pretende atingir são os executivos responsáveis pelo programa de segurança. O sumário deve conter:

- Histórico - Uma descrição do propósito do teste e definições de qualquer termo que possa não ser familiar aos executivos.
  
  - Exemplo: vulnerabilidades e medidas de prevenção
    
- Postura geral - Uma visão geral da eficiência do teste, os problemas encontrados e problemas gerais que causam vulnerabilidades, como a ausência de gerenciamento de patches
  
- Perfil do risco - Uma classificação geral da postura da empresa quanto à segurança, quando comparada com organizações semelhantes, com medidas como alto, moderado ou baixo. Também é importante incluir uma explicação sobre a classificação
  
- Descobertas gerais - Uma sinopse geral dos problemas identificados, juntamente com estatísticas e métricas sobre a eficiência de qualquer medida de prevenção implementada.
  
- Resumo de recomendações - Uma visão geral das tarefas necessárias para corrigir os problemas descobertos no teste de invasão
  
- Mapa estratégico - Oferece objetivos de curto e longo prazo ao cliente para melhorar a sua postura quanto a segurança.
  
  - Exemplo: Informar que se apliquem determinados patches para endereçar problemas de curto prazo, sem montar um plano de longo prazo, o cliente estará na mesma posição após novos patches terem sido disponibilizados.
    

### Relatório técnico

Essa seção oferece detalhes técnicos sobre o teste. Deve incluir o seguinte:

- Introdução - Um inventário dos detalhes como escopo, contatos e assim por diante
  
- Coleta de informações - Detalhes das descobertas da fase de coleta de informações. De particular interesse, são os rastros do cliente (footprint) deixados na Internet
  
- Avaliação de vulnerabilidades - Detalhes das descobertas da fase de análise de vulnerabilidades do teste
  
- Exploração de falhas/verificação de vulnerabilidades - Detalhes das descobertas da fase de exploração e falhas do teste.
  
- Pós-exploração de falhas - Detalhes das descobertas da fase de pós-expliração de falhas do teste
  
- Risco/exposição - Uma descrição quantitativa do risco identificado. Essa seção faz uma estimativa das perdas caso as vulnerabilidades identificadas sejam exploradas por um invasor.
  
- Conclusão - Uma visão geral do teste.
