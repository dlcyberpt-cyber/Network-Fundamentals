# 🖧 Fundamentos de Redes (Networking Basics)

Este repositório contém meus estudos e anotações sobre os principais fundamentos de redes de computadores.  
O objetivo é criar uma base sólida para aprofundar em áreas como segurança ofensiva, análise de tráfego e pentesting.

---

## 📌 O que é uma rede?

Uma rede é um conjunto de dispositivos interconectados (computadores, celulares, servidores, roteadores, switches) que trocam dados entre si.

Ela permite:
- comunicação
- acesso à internet
- compartilhamento de informações
- serviços como sites, apps, jogos online, etc.

---

## 🏛️ Modelos de Referência

### 🔹 Modelo OSI
Organiza a comunicação em **7 camadas**, cada uma com responsabilidade própria.

Resumo:
1. Física — bits na rede
2. Enlace — quadro, MAC
3. Rede — IP, roteamento
4. Transporte — portas TCP/UDP
5. Sessão — gerenciamento de sessão
6. Apresentação — formatos e criptografia
7. Aplicação — o usuário interage

### 🔹 Modelo TCP/IP
Mais simples e usado na prática.

4 camadas:
1. Acesso à rede
2. Internet
3. Transporte
4. Aplicação

---

## 🌍 IPv4

Um endereço IPv4 identifica um host dentro de uma rede.

Exemplo:
192.168.1.1


Formatado em 4 octetos.

---

## 🎯 Máscara e CIDR

A máscara define:
- qual parte é rede
- qual parte é host

Exemplo:
/24 = 255.255.255.0

CIDR é a forma simplificada de representar a máscara.

---

## 🔀 Subnetting

Subnetting = dividir uma rede grande em redes menores.

Exemplo estudado:
/24 dividido em /26 → 4 sub-redes  
Cada sub-rede com 64 endereços

---

## 🔎 ARP e MAC

### MAC
Endereço físico da placa de rede.

### ARP
Mapeia:
**IP ↔ MAC**

Permite que você encontre o dispositivo correto dentro da LAN.

Comando útil:
arp -a

---

## 🔧 DHCP vs Static

### DHCP
IP automático fornecido pelo roteador.

### IP estático
Configuração manual.

---

## 🚚 Camada de Transporte

Principais protocolos usados pela internet:

### TCP
- confiável
- conexão
- 3-way handshake (SYN, SYN+ACK, ACK)

### UDP
- rápido
- sem conexão
- sem garantia de entrega

---

## 📡 ICMP (ex: ping)

Verifica se um host está ativo e responde.

ping

Envia pacotes ICMP Echo Request e recebe Echo Reply.

Serve para:
- testar conectividade
- medir latência
- identificar perda de pacotes

---

## 📂 Objetivo do repositório

✔ documentar o que estou aprendendo  
✔ reforçar fundamentos  
✔ criar base para estudos de cybersecurity  
✔ compartilhar conhecimento  

---

📡 IP do Roteador (Gateway)

O IP do roteador é o endereço usado dentro da rede local (LAN) para que os dispositivos consigam se comunicar com ele.
Ele funciona como o gateway padrão, ou seja, o caminho de saída da rede interna para a internet.

Exemplos comuns:
192.168.0.1
192.168.1.1
10.0.0.1

Esse IP é usado para:

entregar internet aos dispositivos

fornecer IP via DHCP

encaminhar pacotes para fora da rede

acessar o painel de configuração do roteador

Internamente, seu roteador tem:

✔ um IP privado (LAN) → exemplo: 192.168.1.1
✔ um IP público (WAN) → fornecido pelo provedor (ISP)

O IP privado é o “ponto central” da sua rede doméstica.
