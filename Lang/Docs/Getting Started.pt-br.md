# Primeiros Passos

Olá, se você nunca utilizou o Salamandra, este tutorial é para você! Neste tutorial vamos explorar algumas opções básicas do programa para cumprir as necessidades básicas de qualquer rádio.

Os seguintes temas serão explicados nesse tutorial:

* Criar a playlist musical
* Configurar os arquivos de Locução de Hora
* Agendar um bloco de anúncios com os eventos
* Agendar um bloco de anúncios com playlist sequencial
* Agendar uma playlist musical
* Agendar um programa utilizando as prioridades

# Descrição da Tela Inicial

Antes de começar a explicar como fazer a sua programação musical, vamos a uma breve descrição da tela inicial do Salamandra.

<p align="center">
	<img src="Images/MainWindow.png" alt="Tela Principal"/>
</p>

* 1 - **Menu Principal e Barra de Ferramentas** - Onde você poderá acessar as diversas funções do programa separadas em categorias.
* 2 - **Cabeçalho do Player** - Onde você poderá ver o horário, a faixa que está sendo reproduzida no momento e a próxima faixa.  
* 3 - **Planilha de Eventos** - Onde você poderá ver os próximos eventos que serão reproduzidos e também acessar o agendador de eventos.
* 4 - **Playlist** - Onde você poderá colocar as faixas que serão tocadas na sua rádio.
* 5 - **Controles do Player** - Controles do player, volume, modo da playlist e posição da faixa atual.

## Linguagem do Programa

O Salamandra começa por padrão em Inglês, porém seu layout se mantem o mesmo. Para alterar a lingua para Português, acesse o menu **Tools > Settings** e na janela que se abrir, semelhante a imagem abaixo, troque de English para Português e reinicie o programa.

<p align="center">
	<img src="Images/SettingsWindow.png" alt="Tela Principal"/>
</p>

# Criando a playlist musical

Para adicionar faixas a playlist, você pode utilizar o menu **Playlist**, onde você terá a opção de adicionar os diversos tipos de faixa suportados pelo Salamandra, como faixas de áudio, locuções de hora ou arquivos aleatórios. 

Você também pode arrastar arquivos direto do explorador de arquivos do sistema para a sua playlist. As faixas da playlist também podem ser reordenadas arrastando e soltando, para que você possa fazer sua programação musical na ordem que deseja.

<p align="center">
	<img src="Images/PlaylistDragDrop.webp" alt="Tela Principal"/>
</p>

Para manter uma playlist já montada salva, basta utilizar o menu **Arquivo > Salvar** ou o botão de disquete na Barra de Ferramentas. Para abrir uma playlist salva, basta utilizar o menu **Arquivo > Abrir** ou o botão de pasta na Barra de Ferramentas.

# Configurando os arquivos de Locução de Hora

Para configurar os arquivos de Locução de Hora, basta acessar o menu **Ferramentas > Configurações** ou o botão de engrenagem na Barra de Ferramentas. Você então terá acesso a janela de Configurações.

Basta então acessar a opção **Caminho para arquivos de Locução de Horário**, clicar no botão [...] e selecionar a pasta onde estão seus arquivos de horário.

<p align="center">
	<img src="Images/SettingsWindow.png" alt="Tela Principal"/>
</p>

Os arquivos devem estar no seguinte formato. **HRSxx** e **MINxx**, onde o **xx** representa um número indicando o tempo. Um arquivo para 8h da manhã, por exemplo, seria **HRS08**, para o minuto 59, seria **MIN59**. Estes arquivos então são automaticamente combinados pelo Salamandra para indicar a hora nas faixas de Locução de Hora.

Os arquivos de locução de hora podem estar em qualquer um dos formatos de áudio suportados pelo Salamandra.