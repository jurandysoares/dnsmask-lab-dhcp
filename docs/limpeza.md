# Limpeza

O arquivo de configuração padrão do `dnsmasq` possui muitos comentários. Sugiro fortemente que zere o arquivo. Estude a saída dos seguintes comandos:

- `wc -l /etc/dnsmasq.conf`
- `> /etc/dnsmasq.conf`
- `wc -l /etc/dnsmasq.conf`

O `wc -l` irá contar a quantidade de linhas antes e depois da execução do `>`, que irá deixar o arquivo com conteúdo vazio.
