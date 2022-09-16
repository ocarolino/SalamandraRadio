# Getting Started

Hello! If you've never used Salamandra, this tutorial is for you. We're going to show some of the software's functions so that you can get an idea of how to fulfill the basic needs of your radio.

Heads up! Here we assume that you already know the least about operating any software on your computer, giving just a general brushstroke on Salamandra's various options and how they can fit into the practical contexts of your radio.

The following topics will be explained in this tutorial:

- [Changing Salamandra's language](#linguagem-do-programa)
- [Creating a playlist with your music](#criando-a-playlist-musical)
  - [Understanding the Main Window](#entendendo-a-tela-inicial)
  - [Adding tracks to the playlist](#adicionando-faixas-%C3%A0-playlist)
- [Setting Time Announcement files path](#configurando-os-arquivos-de-locução-de-hora)
- [Scheduling advertisement blocks with Events](#agendar-um-bloco-de-anúncio-com-eventos)
  - [Scheduling Time Announcements](#agendando-as-locu%C3%A7%C3%B5es-de-hora)
  - [Scheduling Advertisements](#agendando-os-an%C3%BAncios)
    - [Setting event order on Upcoming Events queue](#customizando-a-ordem-dos-eventos) 
- [Scheduling advertisement blocks with Sequential Playlist](#agendar-um-bloco-de-an%C3%BAncios-com-playlist-sequencial)
  - [Sequential and rotation playlists](#playlists-sequenciais-e-rotativas)
- [Scheduling a music playlist](#agendar-uma-playlist-musical)
- [Scheduling an radio show with priorities](#agendar-um-programa-utilizando-as-prioridades)

# Changing Salamandra's language

Salamandra starts by default in English, but has a Portuguese translation available. To change the language, access the menu **Tools > Settings** or click on the gear button on the toolbar and, in the window that opens, switch from English to Portuguese as shown in the animation below.

**YOU MUST RESTART THE PROGRAM FOR THIS SETTING TO APPLY!**

<p align="center">
	<img src="Images/ChangingLanguage.webp" alt="Alterando a linguagem do Salamandra"/>
</p>

# Creating a playlist with your music

## Understanding the Main Window

Before starting to explain how to make your music playlist, let's go through a brief description of Salamandra's main window.

<p align="center">
	<img src="Images/MainWindow.png" alt="Main Window"/>
</p>

* 1 - **Main Menu and Toolbar** - Where you can access the functions of the program split into categories.
* 2 - **Player Header** - Where you can see the time, the track that is currently playing and the next track.  
* 3 - **Events Playlist** - Where you will be able to see upcoming events that will be played and also access the event scheduler.
* 4 - **Playlist** - Where you can put the tracks that will be played on your radio.
* 5 - **Player Controls** - Player controls, volume, playlist mode and current track position.

## Adding tracks to the playlist

To add tracks to the playlist, you can use the menu **Playlist**, where you'll have the option to add the various track types supported by Salamandra, such as audio tracks, time announcements or random files.

You can also drag and drop files from your system file explorer to your playlist. Playlist tracks can also be reordered by dragging and dropping, so you can put the songs in the order you want.

<p align="center">
	<img src="Images/PlaylistDragDrop.webp" alt="Adicionando arquivos do explorador na playlist"/>
</p>

To save your playlists, you can use the menu **File > Save** or the floppy disk button on the Toolbar. To open an saved playlist, just use the **File > Open** menu or the folder button on the Toolbar.

After creating your playlist, you can use the **Player Controls** to start the playback. Don't forget to try all the playlist modes, so that you can know all the ways that Salamandra sets the next track.

# Setting Time Announcement files path

To set the Time Annoucement files path, you can access the menu **Tools > Settings** or click on the gear button on the toolbar. 

In the Settings window, you will see at the bottom of the screen the option **Time Announcement files path**. Just click the [...] button and select the folder where your time announcement files are.

<p align="center">
	<img src="Images/SettingsWindow.png" alt="Tela de Configuração"/>
</p>

The files must be in the following format:  **HRSxx** and **MINxx**, where **xx** is an number indicating the time. A file for 8 am, for example, would be **HRS08**, for minute 59, it would be **MIN59**. These files are then automatically combined by Salamandra to indicate the time in the Time Announcement tracks.

The audio files for time announcement can be in any of the audio formats supported by Salamandra.

# Scheduling advertisement blocks with Events

The easiest way to set up the advertisements blocks or schedule any other player action is through the event scheduler. Just above the **Events Playlist**, click on the calendar button. The following window will then open:

<p align="center">
	<img src="Images/EventListWindow.png" alt="Events Scheduler"/>
</p>

This window shows all your scheduled events, allowing you to create, edit or delete them.

## Scheduling Time Announcements

So let's create some Time Announcement events that will fire every 15 minutes, to serve as the opening of our ad blocks. Click **New** and follow these steps:

<p align="center">
	<img src="Images/SchedulingTimeAnnouncements.webp" alt="Agendando Locuções de Hora"/>
</p>

As you can see, we will end up with four events that will be triggered at 00, 15, 30 and 45 minutes. Let's go to an explanation of the scheduling of these.

<p align="center">
	<img src="Images/EventWindow_DateAndTime.png" alt="Data e Hora no Agendamento de Evento"/>
</p>

In **Starting date and time**, we put the time of when we want the event to start, and then, we check the option **Immediate**. This means that the event will start exactly at the scheduled time - **this means that any track that is playing will be stopped so that the event can start**. If you want the event to wait until the current track ends, don't check this option!

<p align="center">
	<img src="Images/EventWindow_TimeAndDays.png" alt="Horários e Dias no Agendamento de Evento"/>
</p>

So let's explain the option **Time and days**. When we check **Other hours**, we indicate to Salamandra that we want the event to play at more times than initially configured (16:00:00). We can then set the hours, in this case from 08:00 to 19:00, that the event will be triggered. If you only want the event to play at a specific time, do not check this option.

Note that the starting time changes to (__:00:00), this means the event will play at all selected times at zero minutes and zero seconds, 8:00:00, 9:00:00, 10:00:00, etc.

The **Week Days** option makes scheduling the event periodic, just like the previous option. When you check this option, we indicate to Salamandra that we want the event to play on more days than just the one configured in **Starting date and time**. If you only want the event to play on a single specific day, do not check this option!

<p align="center">
	<img src="Images/EventWindow_EventType.png" alt="Tipo do Evento no Agendamento de Evento"/>
</p>

After that, we just need to set the **Event Type**. For time announcements, we simply select **Time Announcement**. For audio files, as we will see later, we must click on the [...] button and select the file we want.

Finally, as we want the events to play every 15 minutes, we just need to copy and paste the original event and change the time accordingly.

## Scheduling Advertisements

Now, let's schedule some ads. To make the animation brief, we will schedule all of them to fire on the 45-minute block.

If you want your ads to fire in other minutes, then just copy and paste, just like we did with Time Announcements.

<p align="center">
	<img src="Images/SchedulingAds.webp" alt="Agendando Anúncios"/>
</p>

Here we didn't check the **Immediate** box, as the ads must not cut the music, nor should one ad cut the other. The block will be triggered by the **Time Announcement**, which will start immediatelly, with the ads following after.

Other difference from the Time Annoucement, is that for Audio Files we have to choose the file that will be played by the player.

Your Upcoming Events list should look like this, or similar:

<p align="center">
	<img src="Images/UpcomingEventOrder1.png" alt="Upcoming Events - Before ordering"/>
</p>

### Setting event order on Upcoming Events queue

Something that can happen in your radio station is to have advertisers from the same segment, in our example, two markets (*mercado*), and playing them one after the other may not be the best practice. To avoid this, we can use the **Queue order** option.

The queue order is a number ranging from **0 to 99**, with all events starting at **50**. For events that share the same time, in this case 12:45:00, this is an option to customize their order according to your wishes. We can then take one of the markets, in this case the **Mercado 24 Horas** and modify this value.

<p align="center">
	<img src="Images/EventWindow_Order.png" alt="Event queue order"/>
</p>

As both markets are at the bottom of the list, we must then change one of them to any number less than 50, in this case 49, and confirm. Thus, we "pull" the ad to the top of the block, otherwise we would place a number greater than 50, "pushing" the ad down.

After this change, the events will then be repositioned in the Upcoming Events queue, looking like this:

<p align="center">
	<img src="Images/UpcomingEventOrder2.png" alt="Upcoming Events - After Ordering"/>
</p>

In this way, we are able to prevent competitors' ads from being announced one after the other, with greater control of our block of advertisers.

# Scheduling advertisement blocks with Sequential Playlist

To schedule an ad block using a sequential playlist, simply create a playlist with your ads the same as you create a music playlist. When saving, select the **Playlist seq** format and save it with the name you want. **Sequential playlists only support audio files at this time**, other track types are not supported.

<p align="center">
	<img src="Images/SequentialPlaylist.webp" alt="Saving seq playlist"/>
</p>

When scheduling the event, select **Playlist File** as the Event Type and then select the playlist you created.

<p align="center">
	<img src="Images/SchedulingSequentialPlaylist.png" alt="Scheduling seq playlist"/>
</p>

## Sequential and rotation playlists

Sequential playlists are a special type of track where you can place multiple audio tracks and **all of them will play in the saved sequence until the playlist ends**. They are an interesting option to create custom ad blocks as shown above.

Another special type of track is rotation playlists, in which **every time it is triggered, it will play only one of the audio tracks, switching between the tracks saved in the playlist**. You can create them in the same way as sequential playlists, but save as **Playlist rot**. These tracks are great for when you have an advertiser with more than one version of their ad or multiple sweepers that you want to rotate.

# Scheduling a music playlist

On the subject of playlists, to schedule a music playlist select **Playlist File** as the Event Type and schedule your playlist. For m3u or lst files, this will change the music playlist to the new one selected in the event.

<p align="center">
	<img src="Images/SchedulingPlaylist.png" alt="Agendando playlist m3u"/>
</p>

This option is very interesting for radio stations that have different music playlists during the day, or different schedules by day of the week. Just create and schedule your playlists according to the days and times you want to make switching music lists easier.

Note that there are also special event types such as **Start Playback** and **Stop Playback**. These events simulate a click on the **Play** and **Stop** buttons, respectively, so you can schedule when to start or stop the player, further automating your control over your radio's schedules.

# Agendar um programa utilizando as prioridades

Para agendar um programa de rádio já gravado, basta utilizar a mesma forma que se utiliza para agendar um arquivo de áudio normal. Vamos dizer que nós queiramos agendar um programa de esportes que dure de 13:15 a 14:15. 

No nosso exemplo de blocos comerciais de 15 em 15 minutos, poderiamos utilizar a ordenação para este ser o primeiro evento a ser disparado, mas ainda assim, os outros eventos de comerciais ainda ficariam acumulados, prejudicando o restante da programação.

Para lidar com essa situação comum que pode acontecer na sua rádio, temos a opção de prioridades. Perceba que nos eventos que agendamos até aqui, todos eles, na parte de **Ordenação e Prioridade**, vem como padrão com a **Prioridade Baixa**. Podemos então pegar o nosso programa de esportes e marcar como **Prioridade Alta**.

<p align="center">
	<img src="Images/EventHighPriority.png" alt="Prioridade Alta do Evento"/>
</p>

Dessa forma, todos os eventos que "concorrem" com ele pelo horário serão descartados enquanto ele estiver tocando, sem que você precise criar outra grade de eventos alternativa para encaixar o seu programa.

<p align="center">
	<img src="Images/UpcomingEventPriority.png" alt="Próximos Eventos com Prioridade Alta"/>
</p>

Com a opção de Prioridade Alta marcada, o nosso programa de Mesa Redonda muda seu ícone de **verde para vermelho** na grade de Próximos Eventos. Isso significa que enquanto este estiver sendo reproduzido pelo player, **todos os eventos posteriores (os marcados pela caixa vermelha e outros que possam surgir quando virar a hora) serão descartados enquanto o programa estiver tocando.**

Note o seguinte, a primeira Locução de Hora das 13:15 ainda tocará e logo em seguida o nosso programa de Mesa Redonda. Isto ocorre pelo seguinte: a ordenação da grade de eventos primeiro vem pelo **Horário**, logo em seguida se o evento é **Imediato ou Atrasado**, com prioridade para os Imediatos, e finalmente pela opção de **Ordenação**. 

Neste caso, se quisermos que nem mesmo a Locução de Hora toque, basta tornar a Mesa Redonda também Imediato e modificar a sua ordenação para ser menor do que a Locução de Hora.

<p align="center">
	<img src="Images/UpcomingEventPriority2.png" alt="Próximos Eventos com Prioridade Alta"/>
</p>

# Conclusão

Neste tutorial tivemos uma visão geral de como montar a programação de sua rádio e diversas situações e necessidades comuns que você pode ter durante o uso do Salamandra. Ainda há também muitas configurações e funcionalidades do próprio Salamandra que você pode utilizar para fazer ajustes finos de acordo com a sua necessidade.

Você pode por exemplo programar não somente outra grade musical para ser disparada, mas também outra planilha de eventos para quando houver necessidade de uma programação específica para um dia ou momento. Além do Salamandra, é possível buscar outros tutoriais, como sobre fazer seu computador ligar sozinho, utilizar o Agendador de Tarefas do Windows para iniciar/fechar um programa, entre outras funcionalidades de seu sistema operacional.

Através da criatividade para combinar e configurar seu sistema junto com a versatilidade dos eventos do Salamandra, é possível automatizar a sua rádio de forma que o trabalho manual fique somente para aquilo que seja realmente necessário o seu esforço =)