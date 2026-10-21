# Trabalho: Integração de habilidades - 2026/2
## **Disciplina:** Redes de Computadores
### **Cursos:** Engenharia de Computação/Elétrica / Tecnologia em Análise e Desenvolvimento de Sistemas

**Nome:**
**RA:**

---

## 📑 Tarefa 1: Tabela de Sub-Redes (0,5 Ponto)

| Sub- Rede | IPv4 - Sub-Rede | IPv4 - Máscara | IPv6 - Sub-Rede/Prefixo |
| :---: | :---: | :---: | :---: |
| **Pato Branco** | `200.136.N.0` | `255.255.255.192` | `2001:DB8:CAFE:NN00::/64` |
| **Francisco Beltrão** | `200.136.N.64` | `255.255.255.224` | `2001:DB8:CAFE:NN01::/64` |
| **Dois Vizinhos** | `200.136.N.96` | `255.255.255.224` | `2001:DB8:CAFE:NN02::/64` |
| **Toledo** | `200.136.N.128` | `255.255.255.224` | `2001:DB8:CAFE:NN03::/64` |
| **Medianeira** | `200.136.N.160` | `255.255.255.224` | `2001:DB8:CAFE:NN04::/64` |
| **Santa Helena** | `200.136.N.192` | `255.255.255.224` | `2001:DB8:CAFE:NN05::/64` |
| **pb-vit** | `200.136.N.224` | `255.255.255.252` | `2001:DB8:CAFE:NNFF::/112` |
| **vit-fb** | `200.136.N.228` | `255.255.255.252` | `2001:DB8:CAFE:NNFF::1:0/112` |
| **fb-ita** | `200.136.N.232` | `255.255.255.252` | `2001:DB8:CAFE:NNFF::2:0/112` |
| **ita-pb** | `200.136.N.236` | `255.255.255.252` | `2001:DB8:CAFE:NNFF::3:0/112` |
| **ita-dv** | `200.136.N.240` | `255.255.255.252` | `2001:DB8:CAFE:NNFF::4:0/112` |

---

## 🖥️ Tarefa 2: Tabela de Endereçamento Lógico (0,5 Ponto)

| Dispositivo | Interface | IPv4 | IPv4 - Máscara | IPv4 - Gateway | IPv6/Prefixo (GUA) | IPv6 (LLA) | IPv6-Gateway |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **SRV-PB-DNS-DHCP** | NIC | `200.136.N.3` | `255.255.255.192` | `200.136.N.1` | `2001:DB8:CAFE:NN00::3/64` | EUI-64 | `FE80::1` |
| **SRV-PB-WEB** | NIC | `200.136.N.4` | `255.255.255.192` | `200.136.N.1` | `2001:DB8:CAFE:NN00::4/64` | EUI-64 | `FE80::1` |
| **SRV-FB-DNS-DHCP** | NIC | `200.136.N.67` | `255.255.255.224` | `200.136.N.65` | `2001:DB8:CAFE:NN01::3/64` | EUI-64 | `FE80::1` |
| **SRV-FB-WEB** | NIC | `200.136.N.68` | `255.255.255.224` | `200.136.N.65` | `2001:DB8:CAFE:NN01::4/64` | EUI-64 | `FE80::1` |
| **SRV-DV-DNS-DHCP** | NIC | `200.136.N.99` | `255.255.255.224` | `200.136.N.97` | `2001:DB8:CAFE:NN02::3/64` | EUI-64 | `FE80::1` |
| **SRV-DV-WEB** | NIC | `200.136.N.100` | `255.255.255.224` | `200.136.N.97` | `2001:DB8:CAFE:NN02::4/64` | EUI-64 | `FE80::1` |
| **AP-Pato Branco — futuro** | LAN (Gi1) | `200.136.N.5` | `255.255.255.192` | `200.136.N.1` | `2001:DB8:CAFE:NN00::5/64` | Automático | `FE80::1` |
| **AP-Fco. Beltrão — futuro** | LAN (Gi1) | `200.136.N.69` | `255.255.255.224` | `200.136.N.65` | `2001:DB8:CAFE:NN01::5/64` | Automático | `FE80::1` |
| **AP-Dois Vizinhos — futuro** | LAN (Gi1) | `200.136.N.101` | `255.255.255.224` | `200.136.N.97` | `2001:DB8:CAFE:NN02::5/64` | Automático | `FE80::1` |
| **Switch-Pato Branco** | SVI | `200.136.N.2` | `255.255.255.192` | `200.136.N.1` | `2001:DB8:CAFE:NN00::2/64` | EUI-64 | `FE80::1` |
| **Switch-Fco. Beltrão** | SVI | `200.136.N.66` | `255.255.255.224` | `200.136.N.65` | `2001:DB8:CAFE:NN01::2/64` | EUI-64 | `FE80::1` |
| **Switch-Dois Vizinhos** | SVI | `200.136.N.98` | `255.255.255.224` | `200.136.N.97` | `2001:DB8:CAFE:NN02::2/64` | EUI-64 | `FE80::1` |
| **Roteador-Pato Branco** | Fa0/0 | `200.136.N.1` | `255.255.255.192` | — | `2001:DB8:CAFE:NN00::1/64` | `FE80::1` | — |
| **Roteador-Pato Branco** | Se0/0/0 | `200.136.N.225` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::1/112` | EUI-64 | — |
| **Roteador-Pato Branco** | Se0/0/1 | `200.136.N.238` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::3:2/112` | EUI-64 | — |
| **Roteador-Fco. Beltrão** | Fa0/0 | `200.136.N.65` | `255.255.255.224` | — | `2001:DB8:CAFE:NN01::1/64` | `FE80::1` | — |
| **Roteador-Fco. Beltrão** | Se0/0/0 | `200.136.N.233` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::2:1/112` | EUI-64 | — |
| **Roteador-Fco. Beltrão** | Se0/0/1 | `200.136.N.230` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::1:2/112` | EUI-64 | — |
| **Roteador-Vitorino** | Se0/0/0 | `200.136.N.229` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::1:1/112` | EUI-64 | — |
| **Roteador-Vitorino** | Se0/0/1 | `200.136.N.226` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::2/112` | EUI-64 | — |
| **Roteador-Itapejara** | Se0/0/0 | `200.136.N.237` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::3:1/112` | EUI-64 | — |
| **Roteador-Itapejara** | Se0/0/1 | `200.136.N.234` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::2:2/112` | EUI-64 | — |
| **Roteador-Itapejara** | Fa0/1 | `200.136.N.241` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::4:1/112` | EUI-64 | — |
| **Roteador-Dois Vizinhos** | Fa0/0 | `200.136.N.97` | `255.255.255.224` | — | `2001:DB8:CAFE:NN02::1/64` | `FE80::1` | — |
| **Roteador-Dois Vizinhos** | Fa0/1 | `200.136.N.242` | `255.255.255.252` | — | `2001:DB8:CAFE:NNFF::4:2/112` | EUI-64 | — |

---

### Planejamento do Endereçamento dos Clientes — Entrega 1

| Clientes | IPv4 previsto | IPv6 previsto | Gateway e DNS |
| :--- | :--- | :--- | :--- |
| PCs cabeados de cada campus | DHCPv4 | SLAAC / DHCPv6 stateless | Infraestrutura da respectiva LAN |
| Futuros notebooks Wi-Fi de cada campus | DHCPv4 | SLAAC / DHCPv6 stateless | Mesmas sub-redes, gateway e DNS utilizados pelos PCs cabeados |
