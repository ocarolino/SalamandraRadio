<p align="center">
	<img alt="Salamandra" height="150" src="../Readme/lizard.png"/>
</p>

<p align="center">
	<b>Salamandra</b> é um software de automação de rádio para o <b>Windows</b>.
</p> 

<p align="center">
	Projetado para rádios que precisam de um software <b>simples</b>, <b>fácil</b> e <b>estável</b> para programar suas transmissões.
</p>

<hr>

<p align="center">
	<a href="https://github.com/ocarolino/SalamandraRadio">English</a> | <a href="https://github.com/ocarolino/SalamandraRadio/blob/main/Lang/README.pt-BR.md">Português do Brasil</a>
</p>

<hr>

# Recursos
* Player com suporte aos formatos de áudio mais comuns (wav, mp3, wma, ogg and flac)
* Diversos modos para seleção das faixas, como aleatório, embaralhar ou manual para maior controle da programação.
* Faixas especiais, como locução de horário ou arquivos de áudio aleatórios de uma pasta.
* Um programador de eventos versátil, para faixas de áudio ou iniciar/parar o player, em um dia e hora agendados ou de forma periódica, como dias da semana ou horas do dia.
* Um player simplificado para pré-escuta de faixas de áudio em outra saída de som.
* Gerador de arquivos de log, para registrar qualquer atividade ou erros do player.

# Primeiros Passos
Você pode baixar o último release, descompactar e abrir o **Salamandra.exe**. Não há a necessidade de instalação ou configurações extras.

We have a [Getting Started tutorial](Docs/Getting Started.md) where you can see an overview of Salamandra features. But even for functionalities not explained yet, Salamandra is designed to be intuitive, with all relevant functions written in a clear manner. You can also put the cursor on top of any option and read an explanation of what it does.


Nós temos um <a href="https://github.com/ocarolino/SalamandraRadio/blob/main/Lang/Docs/Getting%20Started.pt-br.md">tutorial de Primeiros Passos</a>, onde você pode ter uma visão geral das funcionalidades do Salamandra. Mas mesmo para funcionalidades que ainda não tem um tutorial, o Salamandra foi desenvolvido de forma a ser intuitivo, com todas as funções escritas de uma maneira clara. Você também pode colocar o cursor do mouse em qualquer opção e ler uma breve explicação do que ela faz.

# Screenshots

### Player Principal
<p align="center">
	<img src="../Readme/sc01.png" alt="Main Player"/>
</p>

### Programador de Eventos
<p align="center">
	<img src="../Readme/sc02.png" alt="Event Scheduler"/>
</p>

### Player de Pré-Escuta
<p align="center">
	<img src="../Readme/sc03.png" alt="Pre-Listen"/>
</p>

### Um dos logs diários
<p align="center">
	<img src="../Readme/sc04.png" alt="Pre-Listen"/>
</p>

# Bibliotecas e Recursos

* [BASS](https://www.un4seen.com/)
* [ManagedBass](https://github.com/ManagedBass/ManagedBass)
* [TagLib#](https://github.com/mono/taglib-sharp)
* [Serilog](https://github.com/serilog/serilog)
* [PropertyChanged.Fody](https://github.com/Fody/PropertyChanged)
* [Ookii.Dialogs.Wpf](https://github.com/ookii-dialogs/ookii-dialogs-wpf)
* [Newtonsoft.Json](https://www.newtonsoft.com/json)
* [WpfExtendedToolkit](https://github.com/dotnetprojects/WpfExtendedToolkit)
* [GongSolutions.WPF.DragDrop](https://github.com/punker76/gong-wpf-dragdrop)
* [WPFDarkTheme](https://github.com/AngryCarrot789/WPFDarkTheme)

### Recursos de Imagem/Visuais

* [Icons8](https://icons8.com)
* [famfamfam Silk Icons](http://www.famfamfam.com/lab/icons/silk/)
* [Lizard icons created by Kiranshastry - Flaticon](https://www.flaticon.com/free-icons/lizard)

# Contribuições
Antes de qualquer coisa, obrigado por pensar em contribuir para este projeto! Salamandra é um software gratuito, mas não é de código aberto - isso não quer dizer que as contribuições não são bem vindas!

Você pode sempre contribuir testando, com documentação, tradução, reportando bugs ou dando ideias para novas funcionalidades.

Neste momento, o que precisamos é de testes. Todas as funcionalidades são estaveis em nossos ambientes de teste, mas bugs e outros comportamentos inesperados podem acontecer com máquinas e configurações diferentes, ainda mais nessas primeiras versões.

## Doações

O Salamandra é um software completamente gratuito, você não precisa pagar de forma alguma para usá-lo na totalidade de suas funções. Porém, ele é um software desenvolvido no meu tempo livre como um hobby para praticar programação. Caso você considere-o útil para sua rádio ou trabalho de alguma forma e deseje fazer uma contribuição monetária, sinta-se livre para contribuir com um valor simbólico de R$ 50,00 através dos links abaixo:

<script src="https://www.mercadopago.com.br/integrations/v1/web-payment-checkout.js"data-preference-id="246242802-8d66f19d-86b9-4ab1-8371-647e6f86c514" data-source="button"></script>

<div id="smart-button-container">
      <div style="text-align: center;">
        <div id="paypal-button-container"></div>
      </div>
    </div>
  <script src="https://www.paypal.com/sdk/js?client-id=sb&enable-funding=venmo&currency=BRL" data-sdk-integration-source="button-factory"></script>
  <script>
    function initPayPalButton() {
      paypal.Buttons({
        style: {
          shape: 'pill',
          color: 'blue',
          layout: 'horizontal',
          label: 'paypal',
          
        },

        createOrder: function(data, actions) {
          return actions.order.create({
            purchase_units: [{"description":"Salamandra - Contribuição","amount":{"currency_code":"BRL","value":50}}]
          });
        },

        onApprove: function(data, actions) {
          return actions.order.capture().then(function(orderData) {
            
            // Full available details
            console.log('Capture result', orderData, JSON.stringify(orderData, null, 2));

            // Show a success message within this page, e.g.
            const element = document.getElementById('paypal-button-container');
            element.innerHTML = '';
            element.innerHTML = '<h3>Thank you for your payment!</h3>';

            // Or go to another URL:  actions.redirect('thank_you.html');
            
          });
        },

        onError: function(err) {
          console.log(err);
        }
      }).render('#paypal-button-container');
    }
    initPayPalButton();
  </script>