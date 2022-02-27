# Interfaces

Procure responder a estas perguntas:

1. Quais são os adaptadores de rede de seu servidor?
2. Qual, das redes onde ele está conectado, precisa de um servidor DHCP?


## Respostas

1. No caso de uma máquina Linux, estude a saída dos comandos:

    - `ip address`
    - `ip link`
    - `ls /sys/class/net`
    - ou `ip -br -c -4 a`
    - ou `ip -br -c link`

2. No caso do servidor Dybian passado, é a interface `enp0s9`.

## Denominação das interfaces de rede

Todos os nomes começam com um prefixo de dois caracteres que significam o tipo de interface, conforme tabela abaixo:

| Prefixo | Descrição                            |
| ------- | ------------------------------------ |
| `en`    | *Ethernet*                           |
| `ib`    | *InfiniBand*                         |
| `sl`    | *Serial line IP (slip)*              |
| `wl`    | *Wireless local area network (WLAN)* |
| `ww`    | *Wireless wide area network (WWAN)*  |

Para maiores informações sobre o porque o nome das interfaces de rede no Linux são desta maneira, leia:

- [systemd.net-naming-scheme](https://www.freedesktop.org/software/systemd/man/systemd.net-naming-scheme.html)


## O que fazer?

Configure um endereço IP fixo dentro da faixa de endereço IP da rede privada que você escolheu.

Para revisar o conceito de rede privada:

- Leia: <https://pt.wikipedia.org/wiki/Rede_privada>
- Assista: 

    <iframe width="560" height="315" src="https://www.youtube.com/embed/s2bv_mKEctA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Para aprender a configurar interfaces de rede no Linux:

- Leia: [pt_BR/NetworkConfiguration - Debian Wiki](https://wiki.debian.org/pt_BR/NetworkConfiguration)
- E assista:

<iframe width="560" height="315" src="https://www.youtube.com/embed/-zBx19EZ5U0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

No vídeo, o professor Fábio dos Reis utiliza o comando `ifconfig`. Você tem duas alternativas:

- Usar o comando `ip a`
- Instalar o pacote `net-tools`


