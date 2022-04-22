## IOS (Internet Operating System)

### Introdução 
>
O IOS é o sistema operacional que opera nos dispositivos de rede (Switch e Roteador) da CISCO.
>

### Modos de Operação
>
A partir do terminal da CLI (Interface de Linha de Comando) é possível entrar comandos que mudam o modo de operação. Cada modo de operação possui um conjunto de comandos que lhes são pecualiares. Cada modo de operação possui um `prompt` que o caracteriza. 
>

#### Modo User EXEC Mode ou Modo de Execução do Usuário
>
O `Modo User EXEC` é o modo de operação inicial. A partir desse modo de execução é possível ter acesso a um numero limitado de comandos básicos de monitoramento. Para avançar para o `Modo EXEC Privilegiado` entrar com o comando `enable`.
>
>
`Prompt em um Switch ou em um Roteador`
>
```
Switch>
Router>
````

#### Privileded EXEC Mode ou Modo EXEC Privilegiado
>
Nesse modo o usuário pode usar qualquer comando de monitoramento e pode executar comandos de configuração e gerenciamento. 
>
>
Para retornar para o `Modo User EXEC` digitar o comando `disable`.
>
```
Switch#disable 
Switch>

Router#disable
Router>
````
>
Para entrar no `Modo Configuração Global` digitar o comando `configure terminal`.
>
```
Switch#configure terminal
Switch(config)#

Router#configure terminal
Router(config)# 
````
>
`Prompt em um Switch ou em um Roteador`
>
```
Switch#
Router# 
````

#### Global Configuration Mode ou Modo de Configuração Global
>
Nesse modo o usuário pode configurar um dispositivo. 
>
>
`Prompt em um Switch ou em um Roteador`
>
```
Switch(config)#
Router(config)# 
````
>
Para retornar para o `Modo EXEC Privilegiado` digitar o comando `exit`.
>
>
Para entrar no `Modo EXEC Privilegiado` digitar o comando `exit`.
>

#### Interface Subconfiguration Mode ou Modo de Configuração de Interface
>
Nesse Modo o usuário configura a porta de um Switch ou uma interface de um roteador.
>

`Prompt em um Switch ou em um Roteador
Switch(config-if)#
Router(config-if)#
>
Para entrar no `Modo de Subconfiguração de Interface` digitar o comando `interface <nome_da_interface><numero da interface`
>

`Prompt de uma configuração de interface em um Roteador
```
R1(config)# interface gigabitEthernet 0/1
R1(config-if)# ip address 192.168.10.1 255.255.255.0
R1(config-if)# no shutdown
```


`Prompt de uma configuração de uma VLAN em um Switch
```
S1(config)#interface vlan 1
S1(config-if)#ip address 192.168.1.253 255.255.255.0
S1(config-if)#no sh
S1(config-if)#exit
S1(config)#exit
```

>
`Prompt de uma configuração de interface de console
```
Switch>enable
Switch#configure terminal
Switch(config)#hostname S1
S1(config)#line console 0
S1(config-line)#password cisco
S1(config-line)#login
S1(config-line)#exit
```

>
Para entrar no
Switch(config-if)#
Router(config-if)#

>
Para entrar no
Router(config-if)#
>
Para entrar no

### Transição dos Comandos IOS
>
A figura abaixo apresenta um diagrama que onde comandos executam transições de estado e executam operações de configuração.   
>

![This is a alt text.](/99-figuras/comandos_IOS.png "Estrutura dos comandos IOS.")
