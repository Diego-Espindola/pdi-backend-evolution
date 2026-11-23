# Redes & WebSockets

Estudei sobre o protocolo HTTP.
Um protocolo é um sistema de regras que define como os dados serão trafegados.

Existe já HTTPs acima, como /2.0, porém hoje o node http utiliza como padrão o HTTP/1.1

Ele ta no topo da camada de aplicação, se relaciona com o servidor através de proxys na camada de rede e transporte.

É um protocolo client-server, stateless (sem estado), cada requisição é uma nova, no máximo terá um cache ou proxys que guardarão informações de conexão, etc, mas a requisição é sempre uma nova.O http não tem estado, mas tem sessões.
O fundamento básico do http é não manter estados, são os cookies http que permitem que as sessões tenham estado, através de cabeçalhos.

O cliente geralmente é a aplicação Web, mas pode ser outras coisas, uma automação, etc.

# Correção da IA sobre meu texto:
Relação com as camadas abaixo: O HTTP fica na camada de Aplicação e roda diretamente em cima da camada de Transporte (TCP — ou QUIC/UDP no HTTP/3). Os proxies ficam no meio do caminho intermediando a comunicação, mas o "trilho" obrigatório por onde os pacotes do HTTP/1.1 viajam é o TCP.