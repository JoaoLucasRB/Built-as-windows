## Logbook equipe 02
###### Almir Neto,André Portella, Gabriel Lyrio, Gabriel Muricy, João Silva, Jonas Rafael, Lucas Lima  

Esse documento descreve como foi feita a configuração do servidor e porque tais configurações foram escolhidas bem como as ferramentas nela instaladas. Tambem é descrito no mesmo todo processo (checklist) do handering para promover segurança e estabilidade no servidor.

## Hardware e Sistema Operacional
Para este servidor em especifico foi utilizado o hardware ofercido pela instituição e como se trata de um laboratorio Windows&trade; será usado servidor da Microsoft &reg;.

Hardware|Descrição
-|-
Processador|1 Núcleo, 2 Sockets
Memória RAM| 2GiB
Interface de rede | Virtualizada
Disco Rígido | 50 GB
  
  
Sistema| Versão 
-|-
Windows Server 2012 R2 &reg;| Datacenter

## Particionamento do Disco Rígido
Partição |Tamanho| Propósito
-|-|-
Partição	0 |350|	MB Kernel
Partição	1| 40.7GB |Armazenamento	Principal
Partição	2 |9GB |Swap

## Configuração IPv4
Configuração |Valor
-|-
Endereço	|IP 192.168.1.52
Máscara de sub-rede | 255.255.255.0
Gateway Padrão | 192.168.1.1
IPv4|	DNS	#1 8.8.8.8
IPv4|	DNS	#2 8.8.4.4

## Endereço MAC
> 9e:7e:3d:9a:6e:bd

## Atualizações do sistema

 > Última verificação no dia 27/09/2018. Foi deixado para atualizar os seguintes pacotes durante a noite:
 
 Pacotes|
 -|
 Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	for	Windows	8.1	for	x64-based	Systems	(KB3097997)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	on	Windows	8.1	and	Windows	Server	2012	R2	x64-based	Sys tems	(KB2977765)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	on	Windows	8.1	and	Windows	Server	2012	R2	x64-based	Sys tems	(KB2978041)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	on	Windows	8.1	and	Windows	Server	2012	R2	x64-based	Sys tems	(KB2978126)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	on	Windows	8.1	and	Windows	Server	2012	R2	x64-based	Sys tems	(KB3023222)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	on	Windows	8.1	and	Windows	Server	2012	R2	x64-based	Sys tems	(KB3032663)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	on	Windows	8.1	and	Windows	Server	2012	R2	x64-based	Sys tems	(KB3037579)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	on	Windows	8.1	and	Windows	Server	2012	R2	x64-based	Sys tems	(KB3074228)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	on	Windows	8.1	and	Windows	Server	2012	R2	x64-based	Sys tems	(KB3074548)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	and	4.5 .2	on	Windows	8.1	and	Windows	Server	2012	R2	x64-based	Sys tems	(KB3098779)|
Security	Update	for	Microsoft	.NET	Framework	4.5.1	on	Wind ows	8.1	and	Windows	Server	2012	R2	for	x64-based	Systems	( KB2894856)|
Security	Update	for	Windows	Server	2012	R2	(KB2973201)|
Security	Update	for	Windows	Server	2012	R2	(KB2976897)|
Security	Update	for	Windows	Server	2012	R2	(KB3004365)|
Security	Update	for	Windows	Server	2012	R2	(KB3010788)|
Security	Update	for	Windows	Server	2012	R2	(KB3011780)|
Security	Update	for	Windows	Server	2012	R2	(KB3019978)|
Security	Update	for	Windows	Server	2012	R2	(KB3021674)|
Security	Update	for	Windows	Server	2012	R2	(KB3023266)|
Security	Update	for	Windows	Server	2012	R2	(KB3035126)|
Security	Update	for	Windows	Server	2012	R2	(KB3045685)|
Security	Update	for	Windows	Server	2012	R2	(KB3045755)|
Security	Update	for	Windows	Server	2012	R2	(KB3045999)|
Security	Update	for	Windows	Server	2012	R2	(KB3046017)|
Security	Update	for	Windows	Server	2012	R2	(KB3055642)|
Security	Update	for	Windows	Server	2012	R2	(KB3059317)|
Security	Update	for	Windows	Server	2012	R2	(KB3061512)|
Security	Update	for	Windows	Server	2012	R2	(KB3071756)|
Security	Update	for	Windows	Server	2012	R2	(KB3081320)|
Security	Update	for	Windows	Server	2012	R2	(KB3082089)|
Security	Update	for	Windows	Server	2012	R2	(KB3084135)|
Security	Update	for	Windows	Server	2012	R2	(KB3086255)|
Security	Update	for	Windows	Server	2012	R2	(KB3092601)|
Security	Update	for	Windows	Server	2012	R2	(KB3102939)|
Security	Update	for	Windows	Server	2012	R2	(KB3109103)|
Security	Update	for	Windows	Server	2012	R2	(KB3110329)|
Security	Update	for	Windows	Server	2012	R2	(KB3126041)|
Security	Update	for	Windows	Server	2012	R2	(KB3126434)|
Security	Update	for	Windows	Server	2012	R2	(KB3126587)|
Security	Update	for	Windows	Server	2012	R2	(KB3126593)|
Security	Update	for	Windows	Server	2012	R2	(KB3133043)|
Security	Update	for	Windows	Server	2012	R2	(KB3139398)|
Security	Update	for	Windows	Server	2012	R2	(KB3139914)|
Security	Update	for	Windows	Server	2012	R2	(KB3146723)|
Security	Update	for	Windows	Server	2012	R2	(KB3155784)|
Security	Update	for	Windows	Server	2012	R2	(KB3156059)|
Security	Update	for	Windows	Server	2012	R2	(KB3159398)|
Security	Update	for	Windows	Server	2012	R2	(KB3161949)|
Security	Update	for	Windows	Server	2012	R2	(KB3162343)|
Security	Update	for	Windows	Server	2012	R2	(KB3172729)|
Security	Update	for	Windows	Server	2012	R2	(KB3175024)|
Security	Update	for	Windows	Server	2012	R2	(KB3178539)|
Update	for	.NET	Native	on	Windows	8.1	and	Windows	Server	2 012	R2	for	x64-based	Systems	(KB2954879)|
Update	for	Windows	Server	2012	R2	(KB2938066)|
Update	for	Windows	Server	2012	R2	(KB2967917)|
Update	for	Windows	Server	2012	R2	(KB2989930)|
Update	for	Windows	Server	2012	R2	(KB3000850)|
Update	for	Windows	Server	2012	R2	(KB3008242)|
Update	for	Windows	Server	2012	R2	(KB3012702)|
Update	for	Windows	Server	2012	R2	(KB3013172)|
Update	for	Windows	Server	2012	R2	(KB3013410)|
Update	for	Windows	Server	2012	R2	(KB3013538)|
Update	for	Windows	Server	2012	R2	(KB3013791)|
Update	for	Windows	Server	2012	R2	(KB3024751)|
Update	for	Windows	Server	2012	R2	(KB3024755)|
Update	for	Windows	Server	2012	R2	(KB3027209)|
Update	for	Windows	Server	2012	R2	(KB3030947)|
Update	for	Windows	Server	2012	R2	(KB3033446)|
Update	for	Windows	Server	2012	R2	(KB3034348)|
Update	for	Windows	Server	2012	R2	(KB3036612)|
Update	for	Windows	Server	2012	R2	(KB3037924)|
Update	for	Windows	Server	2012	R2	(KB3038002)|
Update	for	Windows	Server	2012	R2	(KB3042085)|
Update	for	Windows	Server	2012	R2	(KB3043812)|
Update	for	Windows	Server	2012	R2	(KB3044374)|
Update	for	Windows	Server	2012	R2	(KB3044673)|
Update	for	Windows	Server	2012	R2	(KB3045634)|
Update	for	Windows	Server	2012	R2	(KB3045717)|
Update	for	Windows	Server	2012	R2	(KB3045719)|
Update	for	Windows	Server	2012	R2	(KB3046737)|
Update	for	Windows	Server	2012	R2	(KB3048043)|
Update	for	Windows	Server	2012	R2	(KB3054169)|
Update	for	Windows	Server	2012	R2	(KB3054203)|
Update	for	Windows	Server	2012	R2	(KB3054256)|
Update	for	Windows	Server	2012	R2	(KB3054464)|
Update	for	Windows	Server	2012	R2	(KB3055323)|
Update	for	Windows	Server	2012	R2	(KB3055343)|
Update	for	Windows	Server	2012	R2	(KB3060681)|
Update	for	Windows	Server	2012	R2	(KB3060793)|
Update	for	Windows	Server	2012	R2	(KB3063843)|
Update	for	Windows	Server	2012	R2	(KB3071663)|
Update	for	Windows	Server	2012	R2	(KB3077715)|
Update	for	Windows	Server	2012	R2	(KB3078405)|
Update	for	Windows	Server	2012	R2	(KB3078676)|
Update	for	Windows	Server	2012	R2	(KB3080149)|
Update	for	Windows	Server	2012	R2	(KB3087041)|
Update	for	Windows	Server	2012	R2	(KB3087137)|
Update	for	Windows	Server	2012	R2	(KB3091297)|
Update	for	Windows	Server	2012	R2	(KB3092627)|
Update	for	Windows	Server	2012	R2	(KB3094486)|
Update	for	Windows	Server	2012	R2	(KB3095701)|
Update	for	Windows	Server	2012	R2	(KB3096411)|
Update	for	Windows	Server	2012	R2	(KB3099834)|
Update	for	Windows	Server	2012	R2	(KB3100473)|
Update	for	Windows	Server	2012	R2	(KB3103616)|
Update	for	Windows	Server	2012	R2	(KB3103696)|
Update	for	Windows	Server	2012	R2	(KB3103709)|
Update	for	Windows	Server	2012	R2	(KB3109976)|
Update	for	Windows	Server	2012	R2	(KB3115224)|
Update	for	Windows	Server	2012	R2	(KB3121261)|
Update	for	Windows	Server	2012	R2	(KB3123245)|
Update	for	Windows	Server	2012	R2	(KB3132080)|
Update	for	Windows	Server	2012	R2	(KB3133690)|
Update	for	Windows	Server	2012	R2	(KB3134179)|
Update	for	Windows	Server	2012	R2	(KB3134815)|
Update	for	Windows	Server	2012	R2	(KB3137728)|
Update	for	Windows	Server	2012	R2	(KB3138602)|
Update	for	Windows	Server	2012	R2	(KB3139162)|
Update	for	Windows	Server	2012	R2	(KB3139164)|
Update	for	Windows	Server	2012	R2	(KB3140219)|
Update	for	Windows	Server	2012	R2	(KB3140234)|
Update	for	Windows	Server	2012	R2	(KB3145384)|
Update	for	Windows	Server	2012	R2	(KB3145432)|
Update	for	Windows	Server	2012	R2	(KB3146604)|
Update	for	Windows	Server	2012	R2	(KB3146751)|
Update	for	Windows	Server	2012	R2	(KB3146978)|
Update	for	Windows	Server	2012	R2	(KB3147071)|
Update	for	Windows	Server	2012	R2	(KB3149157)|
Update	for	Windows	Server	2012	R2	(KB3173424)|
Update	for	Windows	Server	2012	R2	(KB3179574)|
Update	for	Windows	Server	2012	R2	(KB4033428)|
 
 
 
 ## Antivirus
>Não foi instalado antivírus por sua licensa ser paga.
 

## Firewall
 >Está sendo usado o firewall nativo do windows, não foi instalado nenhum firewall externo. Sendo assim o firewall está configurado como padrão do Windows SErver 2012 R2 &reg;
 
## Estado das portas
> *** Todas as portas estão fechadas menos a 80 (HTTP), 443 (SSL), 21 (FTP), 3389 (Remote Desktop), [49841,49686,49671] usadas pelo sistema.

##### Log netstat:

  Proto  |Endereço local       |  Endereço externo      | Estado
 -|-|-|-
  TCP |192.168.52:49164| 23.103.189.158:https |TIME_WAIT
TCP |192.168.52:49165 |65.55.163.221:https| TIME_WAIT
TCP |192.168.52:49166 |192.16.48.200:https| ESTABILISHED

## Serviços instalados

Nome|Funçao|Instalado por
-|-|-
Remote Desktop|Permite a utilização do servidor via area de trabalho remota| Habilitado por Equipe 02







