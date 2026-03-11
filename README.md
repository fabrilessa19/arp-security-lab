# ARP Security Lab

Este projeto documenta meus estudos sobre o funcionamento do ARP em redes locais
e demonstrações práticas usando máquinas virtuais.

## Objetivo

Entender como dispositivos em uma rede local descobrem endereços MAC a partir
de endereços IP usando o protocolo ARP.

## Ambiente do laboratório

- Kali Linux
- AlmaLinux
- VirtualBox

## Topologia

AlmaLinux (192.168.56.102)
        |
        |
   Virtual Switch
        |
        |
Kali Linux (192.168.56.100)

## Experimentos realizados

- Captura de pacotes ARP
- Observação de ARP request
- Observação de ARP reply
- Análise da tabela ARP

## Ferramentas utilizadas

- tcpdump
- ip command

## Conclusão

O ARP é essencial para comunicação em redes Ethernet, mas também apresenta
vulnerabilidades que podem ser exploradas em ataques como ARP Spoofing.
