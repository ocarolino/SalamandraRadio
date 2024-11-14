# Como configurar a separação musical no Salamandra

A partir da versão 0.6.0, o Salamandra conta com as configurações de separação musical, para que não se repita a mesma faixa ou artista dentro de um determinado período de tempo.

Você pode adicionar as faixas aleatórias que respeitarão as regras de separação pelo menu **Playlist > Adicionar arquivo aleatório de pasta (com separação)**.

<p align="center">
	<img src="Images/Separation/Separation_03.png" alt="Menu para acessar regras de separação"/>
</p>

Para configurar os tempos a serem respeitados, você pode acessar o menu **Ferramentas > Regras de Separação Musical**.

<p align="center">
	<img src="Images/Separation/Separation_01.png" alt="Menu para acessar regras de separação"/>
</p>

Este menu abrirá a seguinte janela, onde você poderá configurar os tempos padrões para as pastas.

<p align="center">
	<img src="Images/Separation/Separation_02.png" alt="Menu para acessar regras de separação"/>
</p>

Note que você também pode configurar os separadores para como serão reconhecidos múltiplos artistas, deixando um por linha. O Salamandra já vem com alguns identificadores padrões, mas você pode adicionar e remover ao seu gosto.

Há a opção também de **usar apenas o artista principal para separação**. Caso ativada, apenas o primeiro artista reconhecido nas músicas será considerado para as regras.

## Configuração Customizada

Caso para uma pasta (ou pastas) você deseje customizar os tempos das regras de separação, você pode clicar com o botão direito sobre ela na playlist e acessar a opção de **Editar atributos da faixa**.

<p align="center">
	<img src="Images/Separation/Separation_04.png" alt="Menu para acessar regras de separação"/>
</p>

Será aberta para você a janela de edição de atributos da faixa, onde você pode escolher o modo de seleção de faixa e os tempos de separação. Caso você não ative as opções de customização, serão utilizada as opções padrão. Para os tempos de separação, é possível utilizar o tempo 0 (zero), para desativar aquela regra específica.

<p align="center">
	<img src="Images/Separation/Separation_05.png" alt="Menu para acessar regras de separação"/>
</p>

O atributo definido só funcionará **na faixa específica configurada**! Se você tiver várias cópias do mesmo caminho na playlist, será necessário copiar e colar novamente se você desejar replicar a mesma customização em todas.

Observe que para guardar estas customizações, você deverá salvar a playlist como **.m3u, .slrot ou .slseq**. Os formatos .lst, .rot e .seq NÃO SUPORTAM qualquer espécie de customização.

--

Nos eventos, você também pode customizar os atributos de uma faixa clicando no botão de engrenagem ao lado do caminho da pasta.

<p align="center">
	<img src="Images/Separation/Separation_06.png" alt="Menu para acessar regras de separação"/>
</p>

## Como o Salamandra identifica os artistas?

Para que o Salamandra possa identificar os artistas de suas músicas, seu acervo deve estar bem organizado, seja via tags ou nome de arquivo. Primeiro, o Salamandra checa as **tags** de artista e título da faixa, caso tenha informações nesses campos, o que tiver informado neles será considerado. 

Observe que o programa **não tem como validar se as informações das tags são corretas ou não!** Dependendo da fonte onde você conseguiu o arquivo de uma música, podem vir informações preenchidas ali que não correspondem a canção de fato - cabe a você como usuário organizar seu acervo.

Caso não haja nenhuma informação nas tags do arquivo relacionadas à artista e título, o Salamandra detectará através do nome do arquivo. O nome dos arquivos devem estar no formato **ARTISTA - TÍTULO** para serem detectados. Tendo um hífen no arquivo, o Salamandra captará a informação antes do primeiro hífen como o artista, e o restante como título da música.

O Salamandra detectará também se a canção tem múltiplos artistas através dos separadores, mas pra isso, as músicas tem que estar bem organizadas. Seja via tags ou nome do arquivo, múltiplos artistas devem estar no mesmo campo: **"Artista1 feat. Artista2 - Título"**, por exemplo. 

Caso esteja "Artista1 - Título feat. Artista2", o segundo artista não será detectado. Outra coisa a observar é que os nomes do artista também devem ser padronizados, "Beatles", por exemplo, se houver músicas como "Beatles", outras como "The Beatles", ou "Os Beatles", estes serão considerados como artistas diferentes.