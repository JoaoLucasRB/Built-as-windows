# Documentação Servidor

Esse documento descreve como foi feita a configuração do servidor e porque tais configurações foram escolhidas bem como as ferramentas nela instaladas. Tambem é descrito no mesmo todo processo (checklist) do handering para promover segurança e estabilidade no servidor.

## Hardware e Sistema Operacional
Para este servidor em especifico foi utilizado o hardware ofercido pela instituição e como se trata de um laboratorio Windows&trade; será usado servidor da Microsoft &reg;.

Processador | Descrição | Motivo
-|-|-
?|?|Fornecido pela instiuição para desenvolver as atividades 

Memória| Descrição | Paginação
-|-|-
Memoria xGB com yMHz| Marca tal, usa tecnologia DDRz,  foram usados k placas para formar essa quantidade de memória | Das ? quantidade de memória estão disponiveis ? para uso e foi definido ? como quantidade de memória virtual
  
  
Memória secundária|Descrição| Motivo
-|-|-
?|?|?
  
  
Sistema| Versão | Particionamento
-|-|-
Windows Server X &reg;| 1803| Utilizamos duas partições, uma contendo o padrão para instalar o sistema e a segunda para acomodar a memória virtual.
## Atualizações do sistema

 > Ultima atualização 01/09/2018 via Windows update.
 
 ## Antivirus
 
  Está sendo usado o Kaspersky versão de avaliação indicada pelo professor mas apenas para teste pois a licensa é paga.
 >Versão: ????
 

## Firewall
 Está sendo usado o firewall nativo do windows, não foi instalado nenhum firewall externo em outros dispositivos ou para.
> Versão do firewall: ????
## Estado das portas
> Todas as portas estão fechadas menos a 80 (HTTP), 443 (SSL), 21 (FTP), 3389 (Remote Desktop), [49841,49686,49671] usadas pelo sistema.

##### Log netstat:

  Proto  |Endereço local       |  Endereço externo      | Estado
 -|-|-|-
  TCP  |  192.168.15.123:3389  |  DESKTOP-DTF118I:51112|  ESTABLISHED
  TCP|    192.168.15.123:49671 |  13.89.217.116:https |   ESTABLISHED
  TCP   | 192.168.15.123:49686 |  52.173.28.179:https|    ESTABLISHED
  TCP |   192.168.15.123:49841  | 64.4.54.254:https   |   TIME_WAIT
  TCP  |  [::1]:49842        |    WIN-FEDRIF0MEGQ:47001 | TIME_WAIT

## Serviços instalados

Nome|Funçao|Instalado por
-|-|-
Remote Desktop|Permite a utilização do servidor via area de trabalho remota| Habilitado por Almir







