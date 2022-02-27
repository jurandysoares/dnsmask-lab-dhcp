# Pacote

O pacote a ser instalado é o `dnsmasq`.

Segue um resumo do pacote:

```yaml
Package: dnsmasq
Version: 2.80-1.1ubuntu1.4
Priority: optional
Section: universe/net
Origin: Ubuntu
Maintainer: Ubuntu Developers <ubuntu-devel-discuss@lists.ubuntu.com>
Original-Maintainer: Simon Kelley <simon@thekelleys.org.uk>
Bugs: https://bugs.launchpad.net/ubuntu/+filebug
Installed-Size: 75,8 kB
Depends: netbase, dnsmasq-base, init-system-helpers (>= 1.18~), lsb-base (>= 3.0-6)
Suggests: resolvconf
Conflicts: resolvconf (<< 1.15)
Homepage: http://www.thekelleys.org.uk/dnsmasq/doc.html
Download-Size: 16,5 kB
APT-Sources: http://us.archive.ubuntu.com/ubuntu focal-updates/universe amd64 Packages
Descrição curta: pequeno proxy de DNS com cache e servidor de DHCP/TFTP
Descrição longa: Dnsmasq é um servidor de DHCP e encaminhador de DNS leve e fácil de
   configurar. Ele é feito para fornecer DNS e, opcionalmente, DHCP a uma
   pequena rede. Ele pode servir os nomes de máquinas locais que não estão no
   DNS global. O servidor DHCP se integra com o servidor de DNS e permite que
   máquinas com endereços alocados por DHCP apareçam no DNS com nomes
   configurados em cada host ou em um arquivo de configuração central.
   Dnsmasq suporta leases DHCP estáticos ou dinâmicos e BOOTP/TFTP para
   inicialização pela rede de máquinas que não tem disco.

```

No Debian, a instalação, como de costume, é super simples:

1. Atualizar o catálogo: 
   
      - `apt update`


2. Instalar o pacote: 

      - `apt install -y dnsmasq`