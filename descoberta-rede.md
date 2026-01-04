# Descoberta de Rede

Este teste teve como objetivo identificar dispositivos ativos
na rede local de forma não invasiva.

## Ferramenta
- Nmap

## Comando utilizado
```bash
nmap -Pn 192.168.14.0/24

## Resultado
Foram identificados múltiplos hosts ativos na rede local.
Alguns dispositivos apresentaram portas abertas relacionadas
a serviços de gerenciamento, comunicação e serviços web.

A utilização da opção -Pn permitiu a identificação dos hosts
mesmo com possíveis bloqueios de ICMP na rede.

## Considerações de Segurança
O bloqueio de ICMP é uma prática comum para reduzir a
descoberta de ativos por atacantes. No entanto, serviços
expostos em portas TCP ainda podem ser identificados por
meio de técnicas alternativas de varredura.
