# Trabalho: Integração de habilidades - 2026/2

## **Disciplina:** Redes de Computadores

### **Cursos:** Engenharia de Computação / Tecnologia em Análise e Desenvolvimento de Sistemas

**Nome:**
**RA:**

---

## 📑 Tarefa 1: Tabela de Sub-Redes (0,5 Ponto)

*Preencha o valor de **N** e **NN** com os dois últimos dígitos do seu RA.*

| Sub- Rede | IPv4 - Sub-Rede | IPv4 - Máscara | IPv6 - Sub-Rede/Prefixo |
| :---: | :---: | :---: | :---: |
| **Pato Branco** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN** *(preencher)* ::/64 |
| **Francisco Beltrão** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN** *(preencher)* ::/64 |
| **Dois Vizinhos** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN** *(preencher)* ::/64 |
| **Toledo** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN** *(preencher)* ::/64 |
| **Medianeira** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN** *(preencher)* ::/64 |
| **Santa Helena** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN** *(preencher)* ::/64 |
| **pb-vit** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN**FF:: *(preencher)* :0/112 |
| **vit-fb** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN**FF:: *(preencher)* :0/112 |
| **fb-ita** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN**FF:: *(preencher)* :0/112 |
| **ita-pb** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN**FF:: *(preencher)* :0/112 |
| **ita-dv** | 200.136.**N**.*(preencher)* | 255.255.255.*(preencher)* | 2001:DB8:CAFE:**NN**FF:: *(preencher)* :0/112 |




---

## 🖥️ Tarefa 2: Tabela de Endereçamento Lógico (0,5 Ponto)

*Preencha o endereçamento estático de todos os dispositivos de infraestrutura (Servidores, Switches, Roteadores e APs). PCs e notebooks usarão DHCPv4 e SLAAC/DHCPv6 stateless.*

*O AP utilizará o quinto endereço IPv4 válido da LAN para gerenciamento. Complete os campos IPv6 do AP somente se o modelo utilizado disponibilizar gerenciamento IPv6; caso contrário, indique “Não disponível no modelo”.*

| Dispositivo | Interface | IPv4 | IPv4 - Máscara | IPv4 - Gateway | IPv6/Prefixo (GUA) | IPv6 (LLA) | IPv6-Gateway |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **SRV-PB-DNS-DHCP** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-PB-WEB** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-FB-DNS-DHCP** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-FB-WEB** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-DV-DNS-DHCP** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-DV-WEB** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **AP-Pato Branco** | LAN (Gi1) | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | (se disponível) | (se disponível) | (se disponível) |
| **AP-Fco. Beltrão** | LAN (Gi1) | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | (se disponível) | (se disponível) | (se disponível) |
| **AP-Dois Vizinhos** | LAN (Gi1) | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | (se disponível) | (se disponível) | (se disponível) |
| **Switch-Pato Branco** | SVI | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **Switch-Fco. Beltrão** | SVI | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **Switch-Dois Vizinhos** | SVI | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **Roteador-Pato Branco** | Fa0/0 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | *FE80::1* | **-** |
| **Roteador-Pato Branco** | Se0/0/0 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Pato Branco** | Se0/0/1 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Fco. Beltrão** | Fa0/0 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | *FE80::1* | **-** |
| **Roteador-Fco. Beltrão** | Se0/0/0 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Fco. Beltrão** | Se0/0/1 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Vitorino** | Se0/0/0 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Vitorino** | Se0/0/1 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Itapejara** | Se0/0/0 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Itapejara** | Se0/0/1 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Itapejara** | Fa0/1 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
| **Roteador-Dois Vizinhos** | Fa0/0 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | *FE80::1* | **-** |
| **Roteador-Dois Vizinhos** | Fa0/1 | 200.136.**N**.(preencher) | 255.255.255.(preencher) | **-** | 2001:DB8:CAFE:**NN**FF::(preencher):(preencher)/112 | EUI-64 | **-** |
---

### Planejamento e Configuração do Wi-Fi — Tarefa 2

| Campus | Nome do AP | Porta do AP ligada ao switch | SSID | Segurança | Senha do ambiente simulado | DHCP do AP |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Pato Branco** | ap-pb-(iniciais) | **Gi1** | UTFPR-PB-(iniciais) | WPA2-PSK / AES | (preencher; mínimo 10 caracteres) | Desativado |
| **Francisco Beltrão** | ap-fb-(iniciais) | **Gi1** | UTFPR-FB-(iniciais) | WPA2-PSK / AES | (preencher; mínimo 10 caracteres) | Desativado |
| **Dois Vizinhos** | ap-dv-(iniciais) | **Gi1** | UTFPR-DV-(iniciais) | WPA2-PSK / AES | (preencher; mínimo 10 caracteres) | Desativado |

| Clientes | IPv4 | IPv6 | Gateway e DNS |
| :--- | :--- | :--- | :--- |
| PCs cabeados de cada campus | DHCPv4 | SLAAC / DHCPv6 stateless | Infraestrutura da respectiva LAN |
| Notebook Wi-Fi de cada campus | DHCPv4 | SLAAC / DHCPv6 stateless | Mesma infraestrutura utilizada pelos PCs cabeados |

*Informe a porta utilizada no switch para conectar cada AP: PB: ______; FB: ______; DV: ______. Na extremidade do roteador sem fio, utilize obrigatoriamente a Gi1.*

---

## 🗺️ Tarefa 3: Tabela de Roteamento (0,5 Ponto)

> Observação: Preencher apenas as rotas estáticas para redes remotas. Lembre-se do fluxo assimétrico (PB $\rightarrow$ VT $\rightarrow$ FB e FB $\rightarrow$ ITA $\rightarrow$ PB).

### Roteador Pato Branco

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

### Roteador Francisco Beltrão

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

### Roteador Vitorino

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

### Roteador Itapejara D'Oeste

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

### Roteador Dois Vizinhos

#### IPv4

| Rede de Destino | Máscara | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) | (preencher) |

#### IPv6

| Rede de Destino /Prefixo | Próximo Salto | Interface de Saída |
| :---: | :---: | :---: |
| (preencher) | (preencher) | (preencher) |

---

### Checklist para Entrega 1

- [ ] Tarefa 1: Tabela de Sub-Redes preenchida corretamente
- [ ] Tarefa 2: Tabela de Endereçamento preenchida corretamente para todos os dispositivos de infraestrutura
- [ ] APs incluídos no endereçamento e no planejamento do Wi-Fi
- [ ] Clientes cabeados e sem fio previstos nas mesmas sub-redes
- [ ] Documento salvo como trabalho-documentacao-v1-NomeAluno.md

### Checklist para Entrega 2

- [ ] Tarefas 1 e 2 revisadas e corrigidas, quando necessário
- [ ] Tarefa 3: Tabelas de roteamento IPv4 e IPv6 completas para todos os roteadores
- [ ] Documento salvo como trabalho-documentacao-v2-NomeAluno.md
