# Estado

É de bom grado verificar o estado do serviço. Seguem alguns comandos que podem nos auxiliar:

1. `systemctl is-active dnsmasq.service`
2. `systemctl status dnsmasq.service`
3. `ss -ul`
4. `ss -unl`

Resumo dos comandos:

1. O dnsmasql está ativo?
2. Qual é o estado do dnsmasq?
3. Quais são as portas de serviço abertas do UDP? Deve aparecer a `bootps` (Servidor BOOTP).
4. Quais são os números de porta de *sockets* abertas do UDP? Deve aparecer a `67` (Servidor BOOTP).
