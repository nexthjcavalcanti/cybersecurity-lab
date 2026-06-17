# 08 - Conexões externas

## Comando usado

`netstat -ano | findstr ESTABLISHED | findstr /v 127.0.0.1`

## Objetivo

Filtrar conexões ativas externas, removendo conexões locais com localhost.

## O que observei

O comando mostrou conexões ativas entre meu computador e endereços externos.

Por segurança, os IPs foram mascarados.

Exemplo:

`192.168.15.x:porta_local -> IP_externo:443 ESTABLISHED PID`

## Conceitos importantes

**ESTABLISHED:** conexão ativa.

**127.0.0.1:** localhost, comunicação interna do próprio computador.

**Porta 443:** usada por HTTPS, comum em sites e serviços seguros.

**PID:** identificador do processo que está usando a conexão.

## Cuidados de segurança

Não publiquei o resultado completo porque ele pode expor:

- IP privado completo
- IPv6 público
- conexões externas
- portas em uso
- processos ativos

## O que aprendi

Conexões externas mostram comunicação entre meu computador e servidores na internet.

Em cybersecurity, é importante analisar conexões, mas também proteger informações sensíveis ao documentar estudos.
