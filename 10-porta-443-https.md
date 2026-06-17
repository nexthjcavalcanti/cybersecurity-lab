# 10 - Porta 443 e HTTPS

## Comando usado

`netstat -ano | findstr :443`

## Objetivo

Visualizar conexões relacionadas à porta 443, usada normalmente por HTTPS.

## O que observei

O comando mostrou várias conexões usando a porta 443.

Por segurança, os IPs foram mascarados.

Exemplos seguros:

`TCP 192.168.15.x:porta_local -> IP_externo_mascarado:443 ESTABLISHED PID`

`TCP IPv6_mascarado:porta_local -> IPv6_externo_mascarado:443 ESTABLISHED PID`

Também apareceram conexões UDP usando a porta 443.

## Conceitos importantes

**Porta 443:** usada por HTTPS, protocolo seguro utilizado em sites e serviços online.

**HTTPS:** comunicação HTTP com criptografia.

**ESTABLISHED:** conexão ativa.

**LISTENING:** porta aguardando conexão.

**CLOSE_WAIT:** conexão em processo de encerramento.

**PID:** identificador do processo relacionado à conexão.

## Cuidados de segurança

Não publiquei o resultado completo do comando, pois ele poderia expor:

* IP privado completo
* IPv6 público
* IPs externos conectados
* portas locais
* processos ativos
* informações da minha rede

## O que aprendi

A porta 443 aparece bastante porque muitos sites e aplicativos usam HTTPS.

Em cybersecurity, analisar portas ajuda a entender quais comunicações estão acontecendo no computador.

Também aprendi que resultados de comandos devem ser revisados e mascarados antes de serem publicados.
