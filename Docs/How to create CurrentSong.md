# How to create a CurrentSong file

- [Template File](#arquivo-de-modelo)
  - [File Types](#tipos-de-arquivo)
- [Output File](#arquivo-de-saída)
- [Tokens](#tokens)
  - [Audio Track Tokens](#tokens-da-faixa-de-áudio)
  - [Other Tokens](#outros-tokens)

For the export of metadata, Salamandra can generate a CurrentSong file, so that you can integrate this information into another software, such as a streaming encoder.

You can access the CurrentSong settings through the menu **Tools > Settings**, then access the **Logs** tab and you will have the screen below.

<p align="center">
    <img src="Images/CurrentSong_Settings.png" alt="Log tab on Settings Window" />
</p>

To generate a CurrentSong file, first of all, it is necessary to activate the option **Enable generating CurrentSong file**.

## Template File

Salamandra does not have a standard format to generate CurrentSong files, giving the user freedom to generate this file with the layout he wants. To set the output format you need, you must choose the **Path to import template file**.

<p align="center">
    <img src="Images/CurrentSong_InputFile.png" alt="CurrentSong input file setting" />
</p>

This file can be a plain text file or even another more structured format, such as XML. You can see some examples below:

<p align="center">
<strong>Simple CurrentSong template</strong>
</p>

<p align="center">
    <img src="Images/CurrentSong_SimpleTemplate.png" alt="Plain text CurrentSong template" />
</p>

<p align="center">
<strong>Structured CurrentSong template</strong>
</p>

<p align="center">
    <img src="Images/CurrentSong_ComplexTemplate.png" alt="XML CurrentSong template" />
</p>

In this way, Salamandra manages to generate an output file in the format desired by the user, which can be adjusted to be read by any software that needs this information.

To create this template file, just use a simple text editor such as **Notepad** and see the list of tokens below to find out what metadata you can use.

### File Types

Usually, the metadata/tags of songs is more complete than that of advertisments or pre-recorded shows, for example. For these, if you wish, you can customize the template that will be used as well, through the File Types.

## Output Files

To generate the output file, set the **Path to generate output file** setting. This is a text file, but there is no fixed extension. You can define the output file as **TXT**, **XML**, just setting the extension with the file name, according to your needs.

<p align="center">
    <img src="Images/CurrentSong_OutputFile.png" alt="CurrentSong output file setting" />
</p>

**Watch out for the output file encoding setting!** Your streaming program may ask for a specific text encoding, so check this setting if you experience any problems.

## Tokens

### Audio Track Tokens

**%friendlyname%** - The "friendly name" of the track. Usually the file name without its extension.

**%durationInSeconds%** - Audio file duration in seconds.

**%artist%** - Audio file artist tag.

**%title%** - Audio file title tag.

**%album%** - Audio file album tag.

**%track%** - Audio file track tag.

**%year%** - Audio file year tag.

**%genre%** - Audio file genre tag.

**%composer%** - Audio file composer tag.

**%comment%** - Audio file comment tag.

### Outros Tokens

#### Hora

**%time_now_hour%** - Current hour

**%time_now_minute%** - Current minute

**%time_now_second%** - Current second

**%time_now_short%** - Current time in short format

**%time_now_long%** - Current time in long format

#### Data

**%date_now_day%** - Current day (numeric)

**%date_now_month%** - Current month (numeric)

**%date_now_year%** - Current year (numeric)

**%date_now_short%** - Current date in short format

**%date_now_long%** - Current date in long format