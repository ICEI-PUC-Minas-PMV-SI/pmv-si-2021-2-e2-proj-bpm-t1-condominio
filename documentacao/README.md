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
  
  - Centralizar em uma única plataforma o gerenciamento de condomínio com base nos seguintes processos de comunicação interna:
Cadastrar moradores;
Cadastrar avisos idealizados pelo síndico;
Emitir e notificar avisos cadastrados aos moradores;
Sistematizar enquetes de votação de novos projetos e melhorias no condomínio;
Gerenciar calendário de eventos e confirmação dos moradores que participarão;
Cadastrar e gerenciar reservas de espaço das áreas de lazer.

- **1.2. Justificativas**
  
  - A administração de um condomínio é uma tarefa muito difícil. Um condomínio demanda a organização de assembleias, reserva do salão de festas, cadastros de moradores, além de manter os moradores informados. Geralmente todas essas funções ficam centralizadas no síndico, dificultando a administração do condomínio, gerando conflito e, em alguns casos, até processos judiciais oriundos de uma má administração.
Assim sendo, vimos a necessidade de elaborar um sistema de gerenciamento condominial que auxilie o condomínio em sua comunicação interna. A adoção de uma plataforma que centraliza os processos de gerenciamento acarreta uma série de benefícios, como: facilidade na comunicação entre o síndico e os condôminos, diminuição de conflitos nos condomínios, o fortalecimento do elo entre os síndicos e os condôminos, facilidade na reserva de espaços de lazer, além de maior celeridade em todo o processo.
  
 **2.Participantes do processo de negócio**
  
  - **Síndico:**
    - Aquele que busca gerenciar o condomínio, manter relações estáveis, ser o representante dos moradores.
  - **Moradores:**
    - São os indivíduos que constituem o condomínio, que serão representados pelo síndico e expressam suas vontades para o mesmo - utilizar um espaço compartilhado, votar em novos projetos, decidir em conjunto o que será ou não realizado dentro do condomínio, por exemplo.
  
**3. Modelagem do processo de negócio**
  
**3.1. Análise da situação atual (AS-IS)**
  
A gestão de um condomínio é uma tarefa complexa que envolve uma grande quantidade de processos administrativos. A situação atual consiste em dar manutenção a esses processos de uma maneira descentralizada, o que acarreta o aumento da dificuldade da administração. Em um condomínio sem uma plataforma de gerenciamento podem-se encontrar diversos problemas:
  
  - **Cadastro de novos moradores**
    - A fim de realizar o cadastro de novos moradores, é necessário que o síndico entre em contato com os novos condôminos e solicite todos os dados necessários. Em seguida, o síndico computa esses dados em algum sistema de armazenamento para os dados - planilhas, cadernos e afins.

![Imagem](/codigo/images/ASIS/cadastroMoradores.png)  
  
  - **Cadastrar, emitir e notificar avisos idealizados pelo síndico**
    - O síndico redige avisos aos condôminos através de ferramentas externas - suíte office, por exemplo.
Após criar os avisos, o síndico imprime os documentos e os coloca em áreas comuns do condomínio como portarias e elevadores, por exemplo. É comum, também, que o síndico envie uma cópia digital do documento via aplicativos de comunicação como o WhatsApp, Telegram etc.

![Imagem](/codigo/images/ASIS/avisos.png)  
  
  - **Cadastro de projetos e sugestões de melhorias no condomínio**
    - O cadastro de projetos e sugestão de melhorias no condomínio é feito presencialmente através de assembleias, conforme ciência e aprovação de todos os moradores. Mediante aprovação, o síndico coordena a execução dos projetos/melhorias.
Imagem do processo de sugestões de melhorias no condomínio (AS-IS) 
  
  - **Sistematizar enquetes de votação de novos projetos e melhorias no condomínio**
    - Enquetes de votação de novos projetos, melhorias e outras modificações diversas no condomínio são realizadas presencialmente em assembleias entre síndicos e proprietários das unidades.

![Imagem](/codigo/images/ASIS/projetosMelhorias.png)  
  
  - **Gerenciar calendário de eventos e confirmação dos moradores que participarão**
    - O calendário de eventos, além do controle da quantidade de indivíduos que participará do evento, é gerenciada de forma manual: o síndico precisa verificar em planilhas ou outros sistemas as datas para as quais eventos foram marcados, além de entrar em contato com os condôminos que participarão desses eventos para confirmar as suas presenças.

![Imagem](/codigo/images/ASIS/confirmaPresenca.png)  
  
  - **Cadastrar e gerenciar reservas de espaço das áreas de lazer**
    - Os condôminos precisam entrar em contato com o síndico e solicitar reserva de espaço das áreas de lazer. O síndico, então, verifica se já existe alguma reserva para a data solicitada. Caso não haja algum problema, o síndico irá efetuar a reserva do local e avisar ao morador que solicitou a reserva.

![Imagem](/codigo/images/ASIS/areasLazer.png)  


**3.2.  Modelagem dos processos aprimorados (TO-BE)**
  
  - **Cadastro de novos moradores**
    - O síndico solicita dados básicos como o e-mail do novo morador para que possa ser criado o login inicial no sistema do condomínio. Ao receber o acesso ao sistema, o novo morador deve preencher a ficha completa que contém os seguintes campos: nome completo, sexo e os dados do endereço desse morador, como: logadouro, cep, bairro, número e complemento. Após cadastrar os dados, o sistema valida automaticamente os dados em buscas de inconsistências. Caso houver alguma inconsistência no cadastro, o morador será alertado para inserir novamente os dados. Uma vez que o cadastro esteja validado pelo sistema, o processo do cadastro é concluído com os dados finais salvos no banco de dados.
 
![Imagem](/codigo/images/TOBE/moradores.png)  
  
  - **Cadastrar, emitir e notificar avisos idealizados pelo síndico**
    - O síndico acessa a plataforma e seleciona a opção de cadastro de avisos. Uma nova página com alguns campos está disposta. Esses campos são: título do aviso, corpo do aviso e data de publicação.
Dessa forma, seria possível centralizar em uma única plataforma uma solução para o cadastro de todo tipo de aviso idealizado pelo síndico, dispensando, assim, a utilização de ferramentas externas.

 ![Imagem](/codigo/images/TOBE/avisos.png)  
  
  - **Cadastro de projetos e sugestões de melhorias no condomínio**
    - O condômino que tiver uma ideia de projeto ou sugestão de melhoria para fazer, acessará a plataforma e identificará a opção de cadastrar uma sugestão de melhoria para o condomínio. Uma nova página com alguns campos está disposta. Essa página contém os  campos: título do projeto/sugestão, descrição do projeto/melhoria e data de publicação. Após o preenchimento dos campos, todos os moradores do condomínio receberão a sugestão. Mediante a aprovação da maioria utilizando um sistema de votação por enquete, é possível colocar em prática a ideia proposta.
Assim sendo, é possível através da plataforma trazer celeridade ao processo de cadastro e execução das melhorias propostas, pois através da utilização da plataforma para cadastrar, notificar e votar as melhorias, inexiste a necessidade de se fazer uma assembleia condominial para tal.

 ![Imagem](/codigo/images/TOBE/melhorias.png)  
  
  - **Sistematizar enquetes de votação de novos projetos e melhorias no condomínio**
    - O síndico acessará a plataforma onde estará disponibilizada a opção de agendar uma assembleia online. O síndico então terá a opção de marcar uma data, com os horários de abertura e encerramento já definidos, para a realização da assembleia. Depois disso se iniciará o processo de definição da assembleia, onde o síndico irá cadastrar as pautas a serem votadas e também poderá disponibilizar arquivos aos participantes, como documentos, planilhas e fotos. A votação apenas poderá ser alterada pelo síndico e apenas antes da assembleia ser realizada, após o início da votação não será possível realizar alterações. Após a reunião já estar definida e publicada, os condôminos serão notificados e poderão confirmar sua presença.

    - No dia da votação os moradores cadastrados irão acessar a plataforma e poderão participar na reunião durante o horário permitido. Serão disponibilizadas as pautas a serem votadas junto com as opções de votação, na qual o voto será totalmente secreto. Ao final da assembleia, as pautas aprovadas e reprovadas serão mostradas, junto com as porcentagens dos votos e a ata da assembleia que será publicada na plataforma pelo síndico. Todas as assembleias realizadas, juntamente com os seus resultados, ficarão registradas na plataforma.

    - Esse processo facilitará a realização das assembleias e também irá aumentar a participação dos condôminos, que na maioria das vezes não participam das reuniões presenciais. 

![Imagem](/codigo/images/TOBE/enquetes.png)  

  - **Gerenciar calendário de eventos**
    - Para o síndico será disponibilizado a ferramenta de cadastro de eventos e gerência dos mesmos. O síndico terá acesso a opções como: consultar, cadastrar, alterar e excluir eventos.
  
![Imagem](/codigo/images/TOBE/eventos.png)

  - **Confirmação dos moradores que participarão de eventos**
    - Por meio da plataforma, os condôminos podem confirmar as suas presenças nos eventos cadastrados pelo síndico. O síndico terá controle sobre a quantia de inscrições em cada um dos eventos criados por ele para que, assim, o síndico possa ter a informação sobre a quantia exata de participantes e o quanto de recursos ele precisará comprar/ter para realizar o evento.
  
![Imagem](/codigo/images/TOBE/confirmaMoradores.png)

  - **Cadastrar e gerenciar reservas de espaço das áreas de lazer**
    - O condômino acessa a plataforma e uma tela de login e senha é disponibilizada. Após realizar a autenticação, o usuário será direcionado para a tela principal na qual são disponibilizadas diversas opções, entre elas a de cadastrar reservas de espaço das áreas de lazer. O condômino, então, terá uma tela com a lista de espaços disponíveis. Após selecionar o espaço desejado, a plataforma mostrará um calendário com dias e horários disponíveis para agendamento. Ao clicar no dia e horário, o condômino será direcionado para uma página com alguns campos pré-preenchidos, como horário, dia, área de lazer selecionada, nome do condômino, unidade habitacional e um check-list de regras e obrigações a serem cumpridas, além de um checkbox com o aceite dos termos de reserva, além de um botão para confirmar a reserva. Ao confirmar a reserva, a plataforma redireciona o condômino para uma tela de confirmação com todos os dados da reserva com a opção de impressão, disparando também um e-mail com os dados da reserva para o síndico e condômino.
  
![Imagem](/codigo/images/TOBE/areaLazer.png)
  
</div>
