## IOS (Internet Operating System)##

### Introdução 
>
O IOS é o sistema operacional que opera nos dispositivos de rede (Switch e Roteador) da CISCO.
>

### Modos de Operação
>
A partir do terminal da CLI(Interface de Linha de Comando) é possível entrar comandos que mudam de modo de operação. Cada modo de operação possui um conjunto de comandos que lhes são pecualiares. Cada modo de operação possui um `prompt` que o caracteriza. 
>

#### Modo User EXEC Mode ou Modo de Execução do Usuário
>
O `Modo User EXEC` permite o acesso a somente um numero limitado de comandos básicos de monitoramento.
>
>
`Prompt em um Switch e em um Roteador`
>
```
Swicth>
Router>
````

#### Privileded EXEC Mode ou Modo EXEC Privilegiado
>
Nesse modo o usuário pode usar qualquer comando de monitoramento e pode executar comandos de configuração e gerenciamento. 
>

>
`Prompt em um Switch e em um Roteador`
>
```
Switch#
Router>
````

### Estrutura dos Comandos IOS
>
A figura abaixo apresenta um diagrama que onde comandos executam transições de estado e executam operações de configuração.   
>

![This is a alt text.](/99-figuras/comandos_IOS.png "Estrutura dos comandos IOS.")
