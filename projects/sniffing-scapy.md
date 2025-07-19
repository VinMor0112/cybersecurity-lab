#  Sniffing com Scapy – Captura de pacotes ICMP

##  Objetivo

Capturar pacotes ICMP (ping) utilizando o Scapy, entender sua estrutura e analisar o tráfego gerado entre a máquina Kali (atacante) e a VM Windows (vítima).

---

## Ferramentas Utilizadas

- Scapy (pré-instalado no Kali Linux)
- Terminal
- VM Windows configurada na rede `vboxnet0`

---

##  Cenário do Laboratório

- **Kali Linux IP:** `192.168.56.11`
- **Windows VM IP:** `192.168.56.10`
- **Rede Interna:** `vboxnet0`

### Topologia da Rede

Kali Linux (192.168.56.11)
|
[Rede Interna: vboxnet0]
|
Windows 10 (192.168.56.10)

---

##  Etapas

### 1. Iniciar o Scapy no Kali

- Dentro do terminal do Kali:

sudo scapy

### 2. Captura de pacotes com Scapy (Kali)

- Dentro do prompt do Scapy:

packets = sniff(filter="icmp", iface="vboxnet0", prn=lambda x: x.summary(), count=10)

### 3. Envio de pacotes (Windows → Kali)

- No Windows (192.168.56.10), execute:

ping 192.168.56.11

### 4. Análise de pacote

- Dentro do prompt do Scapy:

packets[0].show()

## Resultado esperado

- Resumo dos pacotes capturados
- Visualização detalhada de cada camada do protocolo
- Compreensão prática do processo de sniffing

## Observações

- Firewall do Windows desativado para permitir ping
- Ambiente isolado para evitar interferência externa
