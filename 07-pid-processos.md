# 07 - PID e processos

## Comando usado

`tasklist | findstr 19316`

## Objetivo

Descobrir qual programa estava usando um PID visto no comando `netstat`.

## Resultado

O PID analisado estava relacionado ao processo:

`chrome.exe`

## O que aprendi

PID é um identificador de processo.

O `netstat -ano` mostra conexões e PIDs.

O `tasklist` permite descobrir qual programa está usando aquele PID.

## Relação com Cybersecurity

Relacionar portas, conexões e processos ajuda a investigar atividades suspeitas no computador.
