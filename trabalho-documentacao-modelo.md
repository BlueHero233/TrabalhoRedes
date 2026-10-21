# Trabalho: Integração de habilidades - 2026/2

## **Disciplina:** Redes de Computadores

### **Cursos:** Engenharia de Computação / Engenharia Elétrica / Tecnologia em Análise e Desenvolvimento de Sistemas

**Nome:**

**RA:**

**Curso:**

---

Este documento é cumulativo: Entrega 1 — Tarefas 1 e 2 realizadas; Entrega 2 — essas tarefas corrigidas conforme o gabarito; Entrega 3 — acréscimo das tabelas da Seção 7.1; Entrega 4 — acréscimo da documentação Wi-Fi.

## 📑 Tarefa 1: Tabela de Sub-Redes

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

## 🖥️ Tarefa 2: Tabela de Endereçamento Lógico

*Preencha na Entrega 1 o endereçamento estático de todos os dispositivos de infraestrutura, incluindo os futuros APs. Indique DHCPv4 e SLAAC/DHCPv6 stateless para PCs e futuros notebooks.*

**Planejamento dos futuros APs — obrigatório na Entrega 1:** calcule e registre os endereços exatos de gerenciamento: **IPv4, máscara e gateway**, além de **IPv6/prefixo e gateway**. O planejamento deverá reservar o **quinto IPv4 válido** da LAN e o endereço IPv6 com identificador `::5` no /64 do campus, com gateway `FE80::1`. A inclusão física e a configuração dos APs serão realizadas na **Entrega 4**.

Para PCs, notebooks e switches, indique **Automático via RA** no gateway IPv6. Nos servidores, registre **FE80::1** para a configuração manual. O planejamento exato dos gateways dos futuros APs permanece obrigatório.

A documentação de SSID, senha e demais parâmetros Wi-Fi será preenchida na **seção da Tarefa 9, na Entrega 4**.

| Dispositivo | Interface | IPv4 | IPv4 - Máscara | IPv4 - Gateway | IPv6/Prefixo (GUA) | IPv6 (LLA) | IPv6-Gateway |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **SRV-PB-DNS-DHCP** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-PB-WEB** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-FB-DNS-DHCP** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-FB-WEB** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-DV-DNS-DHCP** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-DV-WEB** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **AP-Pato Branco — futuro** | LAN (Gi1) | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | (preencher GUA/prefixo) | Automático | FE80::1 |
| **AP-Fco. Beltrão — futuro** | LAN (Gi1) | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | (preencher GUA/prefixo) | Automático | FE80::1 |
| **AP-Dois Vizinhos — futuro** | LAN (Gi1) | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | (preencher GUA/prefixo) | Automático | FE80::1 |
| **Switch-Pato Branco** | SVI | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | Automático via RA |
| **Switch-Fco. Beltrão** | SVI | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | Automático via RA |
| **Switch-Dois Vizinhos** | SVI | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | Automático via RA |
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

### Planejamento do Endereçamento dos Clientes — Entrega 1

| Clientes | IPv4 previsto | IPv6 previsto | Gateway e DNS |
| :--- | :--- | :--- | :--- |
| PCs cabeados de cada campus | DHCPv4 | SLAAC / DHCPv6 stateless | Gateway IPv4 e DNS via serviços da LAN; gateway IPv6 automático via RA |
| Futuros notebooks Wi-Fi de cada campus | DHCPv4 | SLAAC / DHCPv6 stateless | Mesmos serviços dos PCs; gateway IPv6 automático via RA |

---

## 🗺️ Seção 7.1: Tabelas de Roteamento — Entrega 3

**Preencher na Entrega 3.**

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

## 📶 Tarefa 9: Documentação da Expansão com Wi-Fi — Entrega 4

**Preencher na Entrega 4, após a aula sobre Wi-Fi.** O endereçamento dos APs já deverá constar na Tarefa 2 desde a Entrega 1. Nesta seção, registre os dados da configuração e os resultados da expansão.

### Identificação e Conexões

| Campus | Nome do AP | Modelo utilizado | Notebook | Porta do switch ligada ao AP | Porta do AP ligada ao switch |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Pato Branco** | ap-pb-(iniciais) | (preencher) | (preencher) | (preencher) | **Gi1** |
| **Francisco Beltrão** | ap-fb-(iniciais) | (preencher) | (preencher) | (preencher) | **Gi1** |
| **Dois Vizinhos** | ap-dv-(iniciais) | (preencher) | (preencher) | (preencher) | **Gi1** |

### Parâmetros Wi-Fi

| Campus | SSID configurado | Segurança | Criptografia | Senha do ambiente simulado | DHCP do AP |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Pato Branco** | (preencher) | (preencher) | (preencher) | (preencher; mínimo 10 caracteres) | (preencher) |
| **Francisco Beltrão** | (preencher) | (preencher) | (preencher) | (preencher; mínimo 10 caracteres) | (preencher) |
| **Dois Vizinhos** | (preencher) | (preencher) | (preencher) | (preencher; mínimo 10 caracteres) | (preencher) |

Outros parâmetros Wi-Fi configurados e observações sobre os modelos utilizados: **(preencher)**.

Confirmação de que os APs utilizam os endereços planejados na Tarefa 2: **(preencher)**.

**Limitações verificadas na implementação — Tarefa 9:** se o modelo de AP não permitir configurar o gerenciamento IPv6 ou outro parâmetro de gerenciamento previsto, registre aqui essa condição. Os endereços IPv4 e IPv6 deverão permanecer definidos na Tarefa 2 como parte do planejamento. A comunicação IPv6 dos notebooks continua sendo requisito da expansão.

Limitações do modelo e parâmetros efetivamente configurados: **(preencher)**.

### Endereçamento Recebido pelos Notebooks

| Campus | IPv4 / máscara | IPv6 GUA / prefixo | Gateway IPv4 | Gateway IPv6 | DNS IPv4 / IPv6 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Pato Branco** | (preencher) | (preencher) | (preencher) | (preencher) | (preencher) |
| **Francisco Beltrão** | (preencher) | (preencher) | (preencher) | (preencher) | (preencher) |
| **Dois Vizinhos** | (preencher) | (preencher) | (preencher) | (preencher) | (preencher) |

### Resultados dos Testes da Tarefa 9

Resuma os testes locais e remotos realizados com os notebooks, incluindo conectividade IPv4/IPv6, resolução de nomes e acesso às páginas Web. Informe eventuais pendências ou limitações.

**Resumo dos resultados por campus:** (preencher)

**Data da última verificação:** (preencher)

**Pendências ou limitações registradas:** (preencher)

---