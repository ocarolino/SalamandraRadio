# Primeiros Passos

Olá, se você nunca utilizou o Salamandra, este tutorial é para você! Neste tutorial vamos explorar algumas opções básicas do programa para cumprir as necessidades básicas de qualquer rádio.

Os seguintes temas serão explicados nesse tutorial:

* Configurar a linguagem do Salamandra
* Criar a playlist musical
* Configurar os arquivos de Locução de Hora
* Agendar um bloco de anúncios com os eventos
* Agendar um bloco de anúncios com playlist sequencial
* Agendar uma playlist musical
* Agendar um programa utilizando as prioridades

# Linguagem do Programa

O Salamandra começa por padrão em Inglês, mas tem disponível tradução para Português. Para alterar a língua, acesse o menu **Tools > Settings** ou clique no botão superior de engrenagem e troque de English para Português na janela que se abrir. Qualquer dúvida, basta fazer como na animação abaixo.

**É NECESSÁRIO REINICIAR O PROGRAMA PARA QUE ESTA CONFIGURAÇÃO SEJA APLICADA!**

<p align="center">
	<img src="Images/ChangingLanguage.webp" alt="Alterando a linguagem do Salamandra"/>
</p>

# Criando a playlist musical

## Entendendo a Tela Inicial

Antes de começar a explicar como fazer a sua programação musical, vamos a uma breve descrição da tela inicial do Salamandra.

<p align="center">
	<img src="Images/MainWindow.png" alt="Tela Principal"/>
</p>

* 1 - **Menu Principal e Barra de Ferramentas** - Onde você poderá acessar as diversas funções do programa separadas em categorias.
* 2 - **Cabeçalho do Player** - Onde você poderá ver o horário, a faixa que está sendo reproduzida no momento e a próxima faixa.  
* 3 - **Planilha de Eventos** - Onde você poderá ver os próximos eventos que serão reproduzidos e também acessar o agendador de eventos.
* 4 - **Playlist** - Onde você poderá colocar as faixas que serão tocadas na sua rádio.
* 5 - **Controles do Player** - Controles do player, volume, modo da playlist e posição da faixa atual.

## Adicionando faixas à Playlist

Para adicionar faixas a playlist, você pode utilizar o menu **Playlist**, onde você terá a opção de adicionar os diversos tipos de faixa suportados pelo Salamandra, como faixas de áudio, locuções de hora ou arquivos aleatórios. 

Você também pode arrastar arquivos direto do explorador de arquivos do sistema para a sua playlist. As faixas da playlist também podem ser reordenadas arrastando e soltando, para que você possa fazer sua programação musical na ordem que deseja.

<p align="center">
	<img src="Images/PlaylistDragDrop.webp" alt="Adicionando arquivos do explorador na playlist"/>
</p>

Para manter uma playlist já montada salva, basta utilizar o menu **Arquivo > Salvar** ou o botão de disquete na Barra de Ferramentas. Para abrir uma playlist salva, basta utilizar o menu **Arquivo > Abrir** ou o botão de pasta na Barra de Ferramentas.

Após montar a playlist, basta utilizar os **Controles do Player** para começar a tocar as suas músicas. 

# Configurando os arquivos de Locução de Hora

Para configurar os arquivos de Locução de Hora, basta acessar o menu **Ferramentas > Configurações** ou o botão de engrenagem na Barra de Ferramentas. Você então terá acesso a janela de Configurações.

Basta então acessar a opção **Caminho para arquivos de Locução de Horário**, clicar no botão [...] e selecionar a pasta onde estão seus arquivos de horário.

<p align="center">
	<img src="Images/SettingsWindow.png" alt="Tela de Configuração"/>
</p>

Os arquivos devem estar no seguinte formato. **HRSxx** e **MINxx**, onde o **xx** representa um número indicando o tempo. Um arquivo para 8h da manhã, por exemplo, seria **HRS08**, para o minuto 59, seria **MIN59**. Estes arquivos então são automaticamente combinados pelo Salamandra para indicar a hora nas faixas de Locução de Hora.

Os arquivos de locução de hora podem estar em qualquer um dos formatos de áudio suportados pelo Salamandra.

# Agendar um bloco de anúncio com eventos

A forma mais fácil de montar uma programação de bloco de anúncios ou agendar qualquer outra ação do player é através do agendador de eventos. Logo acima da **Planilha de Eventos**, clique no botão de calendário. Será aberta então a seguinte janela:

<p align="center">
	<img src="Images/EventListWindow.png" alt="Agendador de Eventos"/>
</p>

Esta janela mostra todos os seus eventos cadastrados, permitindo que você crie novos, edite ou exclua eventos já cadastrados.

## Agendando as Locuções de Hora

Vamos criar então um alguns eventos de locução de hora que serão disparados de 15 em 15 minutos, para dar a entrada do nosso bloco de anúncios. Clique em **Novo** e siga os seguintes passos:

<p align="center">
	<img src="Images/SchedulingTimeAnnouncements.webp" alt="Agendando Locuções de Hora"/>
</p>

Como pode notar, teremos ao fim quatro eventos que serão disparados aos minutos 00, 15, 30 e 45. Vamos a uma explicação então do agendamento destes.

<p align="center">
	<img src="Images/EventWindow_DateAndTime.png" alt="Data e Hora no Agendamento de Evento"/>
</p>

Em **Data e Hora de Início**, colocamos o horário do evento e logo em seguida, a primeira opção a ter sido marcada foi a opção **Imediato**. Esta opção significa que o evento entrará exatamente no horário agendado - **isso significa que qualquer música que esteja tocando será cortada para a entrada do evento**. Se você deseja que a música toque até o final e logo seguida o evento, não marque esta opção!

<p align="center">
	<img src="Images/EventWindow_TimeAndDays.png" alt="Horários e Dias no Agendamento de Evento"/>
</p>

Vamos então a explicação da opção **Horários e Dias**. Quando marcamos **Outros Horários**, indicamos ao salamandra que queremos que o evento toque em mais horários do que o configurado inicialmente (17:00:00). Podemos então marcar as horas, neste caso de 08h até 19h, que o evento será disparado. Caso você deseje que o evento toque apenas em um horário específico, não marque esta opção. 

Note que o horário original muda para (__:00:00), isto significa que o evento tocará em todos os horários selecionados aos zero minutos e zero segundos, 8:00:00, 9:00:00, 10:00:00, etc.

Já a opção **Dias da Semana**, torna o agendamento do evento periódico, assim como a opção anterior. Quando você marca esta opção, você indica ao Salamandra que deseja que o evento toque em mais dias do que só o configurado em **Data e Hora de Início**. Caso você deseje que o evento toque apenas em um único dia específico, não marque esta opção!

<p align="center">
	<img src="Images/EventWindow_EventType.png" alt="Tipo do Evento no Agendamento de Evento"/>
</p>

Após isto, basta selecionar o **Tipo de Evento**. Para as locuções de hora, basta nós selecionarmos **Locução de Hora**. Para arquivos de áudio, como veremos em seguida, devemos clicar no botão [...] e selecionar o arquivo que desejamos.

Para finalizar, como queremos que os eventos toquem de 15 em 15 minutos, basta copiar e colar o evento original e apenas trocar a minutagem de acordo.

## Agendando os anúncios

Vamos então agendar alguns anúncios para demonstrar. Para que o tutorial seja breve, vamos programar todos apenas para disparar no bloco dos 45 minutos. 

Se você deseja que seus anúncios disparem em outros minutos, basta então copiar e colar, assim como fizemos com as Locuções de Hora.

<p align="center">
	<img src="Images/SchedulingAds.webp" alt="Agendando Anúncios"/>
</p>

As diferenças de um agendamento para outro são poucas. Para agendar os anúncios, nós apenas não marcamos a caixa **Imediato**, já que os anúncios não devem cortar as músicas nem um anúncio cortar o outro. O bloco será disparado pela **Locução de Hora**, esta sim que terá seu disparo no modo imediato.

Também diferente da Locução de Hora, para arquivos de áudio temos que obrigatoriamente selecionar o arquivo que será reproduzido pelo player.

Você deve notar que a Planilha de Próximos Eventos deve ficar da seguinte forma, ou parecida:

<p align="center">
	<img src="Images/UpcomingEventOrder1.png" alt="Próximos Eventos - Sem Ordenação"/>
</p>

### Customizando a Ordem dos Eventos

Algo que pode acontecer em diversas rádios é ter anunciantes do mesmo segmento, em nosso exemplo, os dois mercados, e não é interessante anunciar eles um atrás do outro. Para evitar isso, podemos utilizar a opção **Ordem do Evento na Fila**. 

A ordem do evento é um número que varia de **0 a 99**, com todos os eventos iniciando em **50**. Para eventos que compartilham o mesmo horário, neste caso 10:45:00, esta é uma opção para customizar a ordem deles de acordo com a sua vontade. Podemos então pegar um dos mercados, neste caso o **Mercado 24 Horas** e modificar este valor.

<p align="center">
	<img src="Images/EventWindow_Order.png" alt="Ordenação do Evento"/>
</p>

 Como os dois mercados estão na posição inferior na grade, devemos então mudar um deles para qualquer número menor que 50, neste caso 49, e confirmar. Assim, "puxamos" o anúncio para o topo do bloco, se fosse o contrário, colocariamos um número maior que 50, "empurrando" o anúncio para baixo.

Após essa alteração, os eventos então serão reposicionados na fila de Próximos Eventos, ficando desta forma:

<p align="center">
	<img src="Images/UpcomingEventOrder2.png" alt="Próximos Eventos - Pós Ordenação"/>
</p>

Assim conseguimos evitar que anúncios de concorrentes sejam anunciados um seguidos do outro, com um maior controle do nosso bloco de anunciantes.

# Agendar um bloco de anúncios com playlist sequencial

Para agendar um bloco de anúncios utilizando uma playlist sequencial, basta montar a playlist de anúncios no mesmo local da playlist musical. Ao salvar a playlist, selecione o formato **Playlist seq** e salve com o nome que desejar. **As playlists sequenciais só suportam arquivos de áudio no momento**, outros tipos de faixas não são suportadas.

<p align="center">
	<img src="Images/SequentialPlaylist.webp" alt="Salvando playlist seq"/>
</p>

Ao agendar o bloco de anúncios, basta então selecionar **Arquivo de Playlist** como o Tipo do Evento e selecionar a playlist salva.

<p align="center">
	<img src="Images/SchedulingSequentialPlaylist.png" alt="Agendando playlist seq"/>
</p>

## Playlists Sequenciais e Rotativas

As playlists sequenciais são um tipo especial de faixa, na qual você pode colocar diversas faixas de áudio e **todas elas tocarão na sequencia salva até que termine a playlist**. São uma opção interessante para criar blocos customizados de anúncios como demonstrado acima.

Outro tipo especial de faixa são as playlists rotativas, você pode criá-las da mesma forma que as playlists sequenciais, mas salve como **Playlist rot**. Estas faixas são ótimas para quando você tem um anunciante com mais de uma versão de seu anúncio ou então diversas vinhetas que você deseja rotacionar. Basta colocar todos em uma playlist rotativa e agendar, dessa forma, **toda vez que a faixa for disparada, ela tocará uma das faixas, alternando entre as faixas salvas na playlist**.

# Agendar uma playlist musical

Aproveitando o assunto de playlists, para agendar uma playlist musical basta da mesma forma selecionar **Arquivo de Playlist** como o Tipo do Evento e agendar a sua playlist.

<p align="center">
	<img src="Images/SchedulingPlaylist.png" alt="Agendando playlist m3u"/>
</p>

Esta opção é muito interessante para rádios que tem diferentes grades musicais durante o dia, ou diferentes grades por dia da semana. Basta montar e agendar suas playliste de acordo com os dias e horários desejados para tornar a troca da grade musical mais fácil.

Note que também há tipos de eventos especiais, como **Iniciar Playlist** e **Parar playlist**. Estes eventos simulam um clique no botão de **Play** e **Stop**, respectivamente, para que você possa agendar quando iniciar ou parar a reprodução do player, automatizando ainda mais o seu controle sobre os horários de sua rádio.

# Agendar um programa utilizando as prioridades