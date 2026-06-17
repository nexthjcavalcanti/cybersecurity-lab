# 06 - Netstat, portas e serviços

## Comando usado

`netstat -ano`

## Objetivo

Visualizar conexões ativas, portas abertas e processos relacionados no Windows.

## O que observei

O comando mostrou conexões TCP e UDP.

Algumas conexões estavam com estado:

- LISTENING
- ESTABLISHED
- TIME_WAIT
- CLOSE_WAIT

## Significados

**LISTENING:** uma porta está aberta e aguardando conexão.

**ESTABLISHED:** existe uma conexão ativa entre meu computador e outro endereço.

**TIME_WAIT:** conexão encerrada recentemente, aguardando finalização.

**CLOSE_WAIT:** conexão em processo de encerramento.

## Cuidados de segurança

Não publiquei o resultado completo do comando, pois ele pode conter:

- IPs locais
- IPs externos
- portas abertas
- processos ativos
- informações da minha rede

## O que aprendi

O `netstat` ajuda a entender quais conexões estão acontecendo no computador.

Esse comando é útil para troubleshooting, redes e cybersecurity.
