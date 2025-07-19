# Cybersecurity Lab – Vinícius Moreira Soares

Este projeto é um laboratório de cibersegurança criado para fins de aprendizado prático, testes de ferramentas ofensivas e defensivas, e desenvolvimento de habilidades técnicas em um ambiente isolado e controlado.

##  Objetivo

Montar um laboratório local que simula redes e sistemas reais, utilizando máquinas virtuais (Kali Linux e Windows), para estudar:

- Testes de intrusão
- Análise de tráfego
- Técnicas de footprinting, scanning e sniffing
- Ferramentas de exploração e defesa
- Scripts e automações com Python

## Tecnologias utilizadas

- **Kali Linux XFCE** (host principal)
- **VirtualBox** (virtualização)
- **Windows 10** (máquina vítima)
- **Rede Interna (vboxnet0)** – IP range: `192.168.56.0/24`

##  Estrutura do projeto

cybersecurity-lab/
├── README.md                        # Visão geral do projeto
│
├── setup/                           # Configuração inicial do ambiente
│   └── network-setup.md            # Configuração da rede interna no VirtualBox
│
├── kali/                            # Anotações e ferramentas do Kali Linux
│   └── tools.md                    # Ferramentas utilizadas e comandos úteis
│
├── windows-lab/                     # Configuração da VM Windows
│   └── config.md                   # Serviços, IP, firewall, usuários etc.
│
├── projects/                        # Testes práticos feitos no laboratório
│   ├── sniffing-analysis/          # Ex: captura e análise de pacotes com Scapy/Wireshark
│   ├── brute-force-tests/          # Ex: Hydra, John the Ripper, Medusa
│   ├── port-scanning/              # Ex: Nmap, Rustscan
│   ├── vulnerability-exploits/     # Ex: uso do Metasploit ou scripts próprios
│   └── ...
│
└── docs/                            # Materiais de apoio
    └── screenshots/                # Evidências visuais (prints, gráficos, etc.)

##  Progresso e atualizações

**Em construção** – Este repositório será atualizado à medida que novos testes e projetos forem implementados.

##  Contato

Vinícius Moreira Soares  
[LinkedIn](www.linkedin.com/in/vinicius-moreira-soares-7896b8205)  
soares.viniciusmoreira@gmail.com
