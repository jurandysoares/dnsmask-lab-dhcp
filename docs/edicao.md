# Edição

Edite o arquivo de configuração do `dnsmasq` com seu editor de texto predileto para terminal (`nano`, `vim` ou `micro`?). Exemplo de comandos para testar a existência de alguns editores:

- `micro --version`
- `nano --version`
- `vim --version`

Conteúdo a inserir no arquivo de configuração do dnsmasq:

```python
# Desabilita a função DNS
port=0

# Configurações do DHCP
dhcp-authoritative
interface=<Interface>
dhcp-range=<End. IP inicial>,<End. IP final>,<Tempo>
dhcp-host=<End. MAC>,<End. IP desejado>,<Tempo>
dhcp-host=<End. MAC>,<Hostname>,<Tempo>
```

Tudo que está entre colchetes angulares `<>` deve ser substituído. No primeiro exemplo da diretiva `dhcp-host`, o endereço IP é informado. No segundo exemplo, o endereço IP é extraído do arquivo `/etc/hosts`. Faça a configuração que você achar mais conveniente e fácil de manter.

