# Habilitação

É de bom grado verficar se o serviço instalado e configurado está habilitado para início automático quando seu servidor for ligado. Em distribuições baseadas em `systemd`, como Debian, Ubuntu e CentOS, execute:

- `systemctl is-enabled dnsmasq.service`

Se o serviço estiver desabilitado, habilite-o:

- `systemctl enable dnsmasq.service`

Nas distribuições Alpine e Gentoo, o comando é:

- `rc-update add dnsmasq`
