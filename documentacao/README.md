<div align="center">
<h1> Documentação do projeto</h1>
</div>

<div align="justify">
  
**1. Introdução**
  
Devido ao grande crescimento demográfico das cidades brasileiras nos últimos anos, a verticalização das cidades é cada vez mais comum. Segundo pesquisas da Associação Brasileira de Síndicos e Síndicos Profissionais (ABRASP), o mercado condominial movimentou 165 bilhões de reais somente em 2019. Apesar disso, administrar um condomínio não é uma tarefa fácil.
Além do básico de um gerenciamento de um condomínio, como gestão de moradores e funcionários, pagamentos e despesas, a recente pandemia de COVID-19 trouxe novos desafios para a organização de um condomínio: controle de áreas coletivas e higienização, por exemplo.
E com isso, os sistemas de gestão condominial estão ganhando destaque. Tanto dentro quanto fora desse cenário de pandemia, os sistemas de gerenciamento para condomínios trazem conforto e facilidade para a administração e para os moradores. Segundo o censo citado anteriormente, 34% dos gestores afirmaram utilizar algum sistema de gerenciamento para condomínio.
Por isso, este trabalho visa o desenvolvimento de um sistema de gerenciamento condominial, com o objetivo de facilitar as atividades e garantir a eficiência da gestão do condomínio. 
  
- **1.1. Objetivos geral e específicos**

  - **1.1.1 Objetivo Geral**  
  
    - O objetivo deste trabalho é desenvolver um sistema de gerenciamento de condomínio que supra demandas administrativas deste, visando o seu bom funcionamento.

  - **1.1.2. Objetivos Específicos**
  
    Centralizar em uma única plataforma o gerenciamento de condomínio com base nos seguintes processos de comunicação interna:
    
    - Cadastrar moradores;
    - Cadastrar avisos idealizados pelo síndico;
    - Emitir e notificar avisos cadastrados aos moradores;
    - Sistematizar enquetes de votação de novos projetos e melhorias no condomínio;
    - Gerenciar calendário de eventos e confirmação dos moradores que participarão;
    - Cadastrar e gerenciar reservas de espaço das áreas de lazer.

- **1.2. Justificativas**
  
  - A administração de um condomínio é uma tarefa muito difícil. Um condomínio demanda a organização de assembleias, reserva do salão de festas, cadastros de moradores, além de manter os moradores informados. Geralmente todas essas funções ficam centralizadas no síndico, dificultando a administração do condomínio, gerando conflito e, em alguns casos, até processos judiciais oriundos de uma má administração. Assim sendo, vimos a necessidade de elaborar um sistema de gerenciamento condominial que auxilie o condomínio em sua comunicação interna. A adoção de uma plataforma que centraliza os processos de gerenciamento acarreta uma série de benefícios, como: facilidade na comunicação entre o síndico e os condôminos, diminuição de conflitos nos condomínios, o fortalecimento do elo entre os síndicos e os condôminos, facilidade na reserva de espaços de lazer, além de maior celeridade em todo o processo.
  
 **2.Participantes do processo de negócio**
  
  - **Síndico:**
  Aquele que busca gerenciar o condomínio, manter relações estáveis, ser o representante dos moradores.
  - **Moradores:**
  São os indivíduos que constituem o condomínio, que serão representados pelo síndico e expressam suas vontades para o mesmo - utilizar um espaço compartilhado, votar em novos projetos, decidir em conjunto o que será ou não realizado dentro do condomínio, por exemplo.
  
**3. Modelagem do processo de negócio**
  
- **3.1. Análise da situação atual (AS-IS)**
  
  A gestão de um condomínio é uma tarefa complexa que envolve uma grande quantidade de processos administrativos. A situação atual consiste em dar manutenção a esses processos de uma maneira descentralizada, o que acarreta o aumento da dificuldade da administração. Em um condomínio sem uma plataforma de gerenciamento podem-se encontrar diversos problemas:
  
  - **Cadastro de novos moradores**
  
    A fim de realizar o cadastro de novos moradores, é necessário que o síndico entre em contato com os novos condôminos e solicite todos os dados necessários. Em seguida, o síndico computa esses dados em algum sistema de armazenamento para os dados - planilhas, cadernos e afins.

    ![Imagem](/documentacao/images/ASIS/cadastroMoradores.png)  
  
  - **Cadastrar, emitir e notificar avisos idealizados pelo síndico**

    O síndico redige avisos aos condôminos através de ferramentas externas - suíte office, por exemplo. Após criar os avisos, o síndico imprime os documentos e os coloca em áreas comuns do condomínio como portarias e elevadores, por exemplo. É comum, também, que o síndico envie uma cópia digital do documento via aplicativos de comunicação como o WhatsApp, Telegram etc.

    ![Imagem](/documentacao/images/ASIS/avisos.png)  
  
  - **Cadastro de projetos e sugestões de melhorias no condomínio**
  
    O cadastro de projetos e sugestão de melhorias no condomínio é feito presencialmente através de assembleias, conforme ciência e aprovação de todos os moradores. Mediante aprovação, o síndico coordena a execução dos projetos/melhorias.
    
    ![Imagem](/documentacao/images/ASIS/enquetes.png) 
  
  - **Sistematizar enquetes de votação de novos projetos e melhorias no condomínio**

    Enquetes de votação de novos projetos, melhorias e outras modificações diversas no condomínio são realizadas presencialmente em assembleias entre síndicos e proprietários das unidades.

    ![Imagem](/documentacao/images/ASIS/projetosMelhorias.png)  
  
  - **Gerenciar calendário de eventos e confirmação dos moradores que participarão**

    O calendário de eventos, além do controle da quantidade de indivíduos que participará do evento, é gerenciada de forma manual: o síndico precisa verificar em planilhas ou outros sistemas as datas para as quais eventos foram marcados, além de entrar em contato com os condôminos que participarão desses eventos para confirmar as suas presenças.

    ![Imagem](/documentacao/images/ASIS/confirmaPresenca.png)  
  
  - **Cadastrar e gerenciar reservas de espaço das áreas de lazer**

    Os condôminos precisam entrar em contato com o síndico e solicitar reserva de espaço das áreas de lazer. O síndico, então, verifica se já existe alguma reserva para a data solicitada. Caso não haja algum problema, o síndico irá efetuar a reserva do local e avisar ao morador que solicitou a reserva.

    ![Imagem](/documentacao/images/ASIS/areasLazer.png)  


- **3.2.  Modelagem dos processos aprimorados (TO-BE)**

  - **Cadastro de novos moradores**

    O síndico solicita dados básicos como o e-mail do novo morador para que possa ser criado o login inicial no sistema do condomínio. Ao receber o acesso ao sistema, o novo morador deve preencher a ficha completa que contém os seguintes campos: nome completo, sexo e os dados do endereço desse morador, como: logadouro, cep, bairro, número e complemento. Após cadastrar os dados, o sistema valida automaticamente os dados em buscas de inconsistências. Caso houver alguma inconsistência no cadastro, o morador será alertado para inserir novamente os dados. Uma vez que o cadastro esteja validado pelo sistema, o processo do cadastro é concluído com os dados finais salvos no banco de dados.
 
    ![Imagem](/documentacao/images/TOBE/moradores.png)  
  
  - **Cadastrar, emitir e notificar avisos idealizados pelo síndico**

    O síndico acessa a plataforma e seleciona a opção de cadastro de avisos. Uma nova página com alguns campos está disposta. Esses campos são: título do aviso, corpo do aviso e data de publicação. Dessa forma, seria possível centralizar em uma única plataforma uma solução para o cadastro de todo tipo de aviso idealizado pelo síndico, dispensando, assim, a utilização de ferramentas externas.

    ![Imagem](/documentacao/images/TOBE/avisos.png)  
  
  - **Cadastro de projetos e sugestões de melhorias no condomínio**

    O condômino que tiver uma ideia de projeto ou sugestão de melhoria para fazer, acessará a plataforma e identificará a opção de cadastrar uma sugestão de melhoria para o condomínio. Uma nova página com alguns campos está disposta. Essa página contém os  campos: título do projeto/sugestão, descrição do projeto/melhoria e data de publicação. Após o preenchimento dos campos, todos os moradores do condomínio receberão a sugestão. Mediante a aprovação da maioria utilizando um sistema de votação por enquete, é possível colocar em prática a ideia proposta. Assim sendo, é possível através da plataforma trazer celeridade ao processo de cadastro e execução das melhorias propostas, pois através da utilização da plataforma para cadastrar, notificar e votar as melhorias, inexiste a necessidade de se fazer uma assembleia condominial para tal.

    ![Imagem](/documentacao/images/TOBE/TOBE.png)
  
  - **Sistematizar enquetes de votação de novos projetos e melhorias no condomínio**

    O síndico acessará a plataforma onde estará disponibilizada a opção de agendar uma assembleia online. O síndico então terá a opção de marcar uma data, com os horários de abertura e encerramento já definidos, para a realização da assembleia. Depois disso se iniciará o processo de definição da assembleia, onde o síndico irá cadastrar as pautas a serem votadas e também poderá disponibilizar arquivos aos participantes, como documentos, planilhas e fotos. A votação apenas poderá ser alterada pelo síndico e apenas antes da assembleia ser realizada, após o início da votação não será possível realizar alterações. Após a reunião já estar definida e publicada, os condôminos serão notificados e poderão confirmar sua presença.

    No dia da votação os moradores cadastrados irão acessar a plataforma e poderão participar na reunião durante o horário permitido. Serão disponibilizadas as pautas a serem votadas junto com as opções de votação, na qual o voto será totalmente secreto. Ao final da assembleia, as pautas aprovadas e reprovadas serão mostradas, junto com as porcentagens dos votos e a ata da assembleia que será publicada na plataforma pelo síndico. Todas as assembleias realizadas, juntamente com os seus resultados, ficarão registradas na plataforma.

    Esse processo facilitará a realização das assembleias e também irá aumentar a participação dos condôminos, que na maioria das vezes não participam das reuniões presenciais. 

    ![Imagem](/documentacao/images/TOBE/enquetes.png)  

  - **Gerenciar calendário de eventos**

    Para o síndico será disponibilizado a ferramenta de cadastro de eventos e gerência dos mesmos. O síndico terá acesso a opções como: consultar, cadastrar, alterar e excluir eventos.
  
    ![Imagem](/documentacao/images/TOBE/eventos.png)

  - **Confirmação dos moradores que participarão de eventos**

    Por meio da plataforma, os condôminos podem confirmar as suas presenças nos eventos cadastrados pelo síndico. O síndico terá controle sobre a quantia de inscrições em cada um dos eventos criados por ele para que, assim, o síndico possa ter a informação sobre a quantia exata de participantes e o quanto de recursos ele precisará comprar/ter para realizar o evento.
    
    ![Imagem](/documentacao/images/TOBE/confirmaMoradores.png)

  - **Cadastrar e gerenciar reservas de espaço das áreas de lazer**

    O condômino acessa a plataforma e uma tela de login e senha é disponibilizada. Após realizar a autenticação, o usuário será direcionado para a tela principal na qual são disponibilizadas diversas opções, entre elas a de cadastrar reservas de espaço das áreas de lazer. O condômino, então, terá uma tela com a lista de espaços disponíveis. Após selecionar o espaço desejado, a plataforma mostrará um calendário com dias e horários disponíveis para agendamento. Ao clicar no dia e horário, o condômino será direcionado para uma página com alguns campos pré-preenchidos, como horário, dia, área de lazer selecionada, nome do condômino, unidade habitacional e um check-list de regras e obrigações a serem cumpridas, além de um checkbox com o aceite dos termos de reserva, além de um botão para confirmar a reserva. Ao confirmar a reserva, a plataforma redireciona o condômino para uma tela de confirmação com todos os dados da reserva com a opção de impressão, disparando também um e-mail com os dados da reserva para o síndico e condômino.
  
    ![Imagem](/documentacao/images/TOBE/areaLazer.png)
  
**4. Projeto da arquitetura de dados da solução proposta**

  - **4.1. Diagrama de Entidades e Relacionamentos (DER)**
  
  ![Imagem](/documentacao/images/outros/der.png)
  
  - **4.2. Impactos da implementação em um banco de dados NoSQL**
  
    NoSQL (refere-se também a “Não só SQL”, “Não SQL” ou “não relacional”) é um banco de dados que fornece uma maneira de gerenciar os dados que estão em uma forma não relacional, ou seja, que não está estruturado de forma tabular e não possui relações tabulares. Esse tipo de banco de dados vem ganhando popularidade cada vez mais à medida que é empregado em aplicativos de big data e tempo real. Os bancos de dados NoSQL são escaláveis, de alto desempenho e flexíveis por natureza. Suas estruturas são completamente diferentes daquelas dos bancos de dados relacionais. Nesses os dados são colocados em tabelas e a estrutura de dados é projetada antes de o banco de dados ser criado. Algumas diferenças entre Banco de Dados NoSQL e SQL:
  
**NoSQL** | **SQL**
------------ | -------------
São principalmente bancos de dados não relacionais ou distribuídos. Tecnologia relativamente nova. | São principalmente bancos de dados relacionais (RDBMS). Tecnologia madura e consolidada. NoSQL podem ser baseados em documentos, pares de valores-chave, gráficos ou colunas e não precisam seguir as definições de esquema padrão.
Os bancos de dados SQL são baseados em tabelas na forma de linhas e colunas e devem seguir estritamente as definições de esquema padrão. | Eles são a melhor opção para aplicativos que precisam de transações com várias linhas.
Eles têm o esquema dinâmico para dados não estruturados. Os dados podem ser armazenados de forma flexível sem ter uma estrutura predefinida.|Eles têm um esquema predefinido bem projetado para dados estruturados.
Os bancos de dados NoSQL favorecem o esquema desnormalizado.|Os bancos de dados SQL favorecem o esquema normalizado.
Mais barato para escalar quando comparado a bancos de dados relacionais.|Escalabilidade cara.
Os bancos de dados NoSQL são escalonáveis horizontalmente.| Os bancos de dados SQL são escalonáveis verticalmente.
Não é um bom ajuste para consultas complexas, pois não existe uma interface padrão no NoSQL para lidar com consultas. As consultas no NoSQL não são tão poderosas quanto as consultas SQL. É chamado de UnQL e a sintaxe para usar a linguagem de consulta não estruturada varia de sintaxe para sintaxe.|Eles são adequados para consultas complexas, pois o SQL tem uma interface padrão para lidar com consultas. A sintaxe das consultas SQL é fixa.
Os bancos de dados NoSQL seguem corretamente o teorema do CAP de Brewers (consistência, disponibilidade e tolerância de partição).|Os bancos de dados SQL seguem corretamente as propriedades ACID (Atomicidade, Consistência, Isolamento e Durabilidade).
Você pode usar o NoSQL para fins transacionais pesados. No entanto, não é a melhor opção para isso.| Melhor ajuste para aplicativos baseados em altas transações.
Exemplos de bancos de dados NoSQL: MongoDB, Apache CouchDB, Redis, HBase. | Exemplo de bancos de dados SQL: MySQL, Oracle, MS-SQL, PostgreSQL.
  
  Percebe-se com as diferenças acima que os bancos de dados possuem características próprias e propósitos específicos. Enquanto os bancos de dados NoSQL buscam trabalhar com grandes volumes de dados com uma arquitetura eficiente e escalável, os bancos de dados SQL seguem padrões bem definidos como ISI e ANSI, que são aceitos em todo o mundo, além de usarem linguagem padronizada única, ou seja, SQL em diferentes RDBMS (Sistema de Gerenciamento de Banco de Dados Relacional). Além disso, as transações em bancos de dados SQL são compatíveis ACID (Atomicidade, Consistência, Isolamento e Durabilidade), o que garante segurança e estabilidade.
  
  Conforme apresentamos as diferenças entre NoSQL e SQL, a escolha do banco de dados dependerá de preferências, requisitos de negócios, volume e variedade de dados. Os bancos de dados NoSQL estão ganhando grande popularidade atualmente devido à sua capacidade de integrar big data, baixo custo, fácil escalabilidade e recursos de código aberto. No entanto, ainda é uma tecnologia relativamente nova e carece de padronização, ao contrário do SQL. A falta de conformidade com o ACID também é uma preocupação com o NoSQL. Após o cotejamento entre os bancos de dados NoSQL e SQL, seus propósitos e aplicabilidades, e devido às preocupações quanto à segurança e estabilidade, o projeto condomínio, por ser um sistema transacional, não encontra nos bancos de dados NoSQL alguns requisitos fundamentais para sua adoção. Sendo assim, os bancos de dados relacionais possuem maior aderência ao negócio.
  
  - **4.3. Modelo relacional**
  
![Imagem](/documentacao/images/outros/mer.png)
  
**5. Relatórios analíticos**

![Imagem](/documentacao/images/relatorios/eventosAreasLazer.png)

O objetivo desse relatório é analisar, por meio de um gráfico de pizza, quais são as áreas de lazer mais reservadas pelos condôminos.

![Imagem](/documentacao/images/relatorios/eventosAreasLazerPorAno.png)

Esse relatório é semelhante ao anterior, no entanto o seu é foco é avaliar quais são as áreas de lazer mais reservadas pelos condôminos em um intervalo de um ano.

![Imagem](/documentacao/images/relatorios/mediaEventosAno.png)

Esse relatório destaca a quantidade de eventos realizados em um intervalo de um ano.

![Imagem](/documentacao/images/relatorios/participantesPorEvento.png)

Através de uma tabela, esse relatório lista diversas informações sobre participações em determinados eventos. A coluna "Nome do evento" pode ser utilizada para filtrar as participações por evento.
  
  -  **5.1. Associação de comandos SQL com relatórios analíticos**

**Nome do Relatório Analítico** | **Comando SQL-DML (SELECT)**
------------ | -------------
Relatório de participantes por evento | select m.nomemorador, e.nome, e.datarealizacao,	al.nome, me.confirmacao from tbmorador m, tbevento e, tbeventoarealazer eal, tbmoradoreseventos me, tbarealazer al where m.idmorador = me.idmorador and e.idevento = eal.idevento and e.idevento = me.idevento and eal.idarealazer = al.idarealazer
Relatório de eventos por tipo de eventos | Rafael
Relatório eventos em áreas de lazer | SELECT evento.Nome 'Nome do evento', areaLazer.Nome 'Área do evento', FROM tbEvento Evento LEFT JOIN tbEventoAreaLazer EventoAreaLazer ON eventoAreaLazer.IDEvento = evento.IDEvento LEFT JOIN tbAreaLazer AreaLazer ON areaLazer.IDAreaLazer = eventoAreaLazer.IDAreaLazer ORDER BY areaLazer.Nome
Relatório de média de eventos por ano | SELECT YEAR(DataRealizacao) AS Ano, COUNT(IDEvento) AS QTD_Eventos FROM tbEvento GROUP BY YEAR(DataRealizacao)
Relatório da quantidade de participantes por tipo de evento | XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
Relatório de utilização de areas de lazer por ano em eventos | select evento.Nome NomeEvento, areaLazer.Nome 'Local do Evento', convert(varchar, eventoArea.DataRealizacao, 103) DataRealizacao, count(eventoArea.IDEvento) Quantidade from tbEvento evento left join tbEventoAreaLazer eventoArea on eventoArea.IDEvento = evento.IDEvento left join tbAreaLazer areaLazer on areaLazer.IDAreaLazer = eventoArea.IDAreaLazer group by evento.Nome, areaLazer.Nome, eventoArea.DataRealizacao
  
**6. Indicadores de desempenho**
</div>

**Indicador** | **Objetivo** | **Descrição** | **Fórmula de Cálculo** | **Fontes de dados** | **Perspectiva**
------------- | ------------ | ------------- | ---------------------- | ------------------- | -------------
 Média de Participantes por Evento | Constatar a média de participantes por Evento | Apresentar a porcentagem de participação de moradores por evento. | (Qtde Participantes/TotalEventos)*100 | Tabela de moradores/eventos | Visualizar o histograma de média de participação de moradores por eventos.
 Porcentagem de eventos por área de lazer | Constatar quais áreas de lazer são mais utilizadas em eventos a fim de auxiliar o síndico a organizar-se melhor. | Apresentar a porcentagem de ocupação das áreas de lazer reservadas para eventos. | (Eventos em uma área de lazer/Total de eventos)*100 | Tabelas de eventos e áreas de lazer. | Visualizar um gráfico de pizza relativo aos eventos por área de lazer. 
 Quantidade de eventos por tipo de eventos | zzzzzzzzzzzz | zzzzzzzzzzzzz | zzzzzzzzzzz | zzzzzzzzzzzzzzzzzzz | zzzzzzzzzzzzz
 Média de eventos por ano | Constatar a média de incidência de eventos no período de um ano | Apresentar a média de ocorrência de eventos | (QtdeEventos/365) | Tabela de eventos | Visualizar o histograma de eventos.
 Quantidade de participantes por tipo de eventos | Constatar a quantidade de participantes por tipo de evento | Apresentar a quantidade de moradores por tipo de evento.  | (Qtde ParticipantesTipoEvento/TipoDeEvento) | Tabela de Morador Evento e de eventos  | Visualizar um gráfico de barras relativo a quantidade de moradores em cada tipo de evento.
 
<div align="justify">
  
 **7. Conclusão**
  
O objetivo deste trabalho foi a centralização administrativa de um condomínio em uma plataforma que simplifica e dá fluidez a todo o processo gerencial de um condomínio. Sempre foi o nosso foco ao longo do projeto a obtenção de uma ferramenta que seja de fácil usabilidade, não apenas para a figura do síndico que é o maior beneficiado mas também para os condôminos, facilitando assim a convivência e gerenciamento dentro de um condomínio.
Conseguimos cumprir com todos os objetivos propostos pela ementa da disciplina, porém, reduzimos o escopo original de nossa proposta em virtude do tempo que tínhamos para concluir o trabalho.  
Assim sendo, estamos entregando uma plataforma pronta para ser implementada com as funcionalidades que automatizamos em pleno funcionamento e devidamente testadas. Havendo interesse em continuar o desenvolvimento dessa proposta e para que se obtenha uma plataforma de gerenciamento mais completa, recomendamos a automatização dos demais processos que citamos, pois conforme já citado em virtude do tempo de entrega automatizamos apenas o processos de Cadastrar Reservas De Espaço Das Áreas De Lazer e o processo de Confirmação Dos Moradores Que Participarão De Eventos.

</div>
