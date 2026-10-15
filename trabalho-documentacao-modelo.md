# Trabalho: Integração de habilidades - 2026/2

## **Disciplina:** Redes de Computadores

### **Cursos:** Engenharia de Computação / Engenharia Elétrica / Tecnologia em Análise e Desenvolvimento de Sistemas

**Nome:**

**RA:**

**Curso:**

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

*Preencha na Entrega 1 o endereçamento estático de todos os dispositivos de infraestrutura, incluindo os futuros APs. Indique DHCPv4 e SLAAC/DHCPv6 stateless para PCs e futuros notebooks.*

**Planejamento dos futuros APs — obrigatório na Entrega 1:** calcule e registre os endereços exatos de gerenciamento: **IPv4, máscara e gateway**, além de **IPv6/prefixo e gateway**, se o modelo permitir. O AP utilizará o **quinto IPv4 válido** da LAN e, quando houver gerenciamento IPv6, o identificador `::5` no /64 do campus, com gateway `FE80::1`. Para recursos de gerenciamento ausentes, indique **“Não disponível no modelo”** e identifique o equipamento previsto. A inclusão física e a configuração dos APs serão realizadas na **Entrega 4**.

Modelo de roteador sem fio previsto para atuar como AP: **(preencher na Entrega 1)**.

A documentação de SSID, senha e demais parâmetros Wi-Fi será preenchida na **seção da Tarefa 9, na Entrega 4**.

| Dispositivo | Interface | IPv4 | IPv4 - Máscara | IPv4 - Gateway | IPv6/Prefixo (GUA) | IPv6 (LLA) | IPv6-Gateway |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **SRV-PB-DNS-DHCP** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-PB-WEB** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-FB-DNS-DHCP** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-FB-WEB** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-DV-DNS-DHCP** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **SRV-DV-WEB** | NIC | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | 2001:DB8:CAFE:**NN**(preencher)::(preencher)/64 | EUI-64 | *FE80::1* |
| **AP-Pato Branco — futuro** | LAN (Gi1) | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | (preencher GUA/prefixo, se permitido) | Automático, se permitido | FE80::1, se permitido |
| **AP-Fco. Beltrão — futuro** | LAN (Gi1) | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | (preencher GUA/prefixo, se permitido) | Automático, se permitido | FE80::1, se permitido |
| **AP-Dois Vizinhos — futuro** | LAN (Gi1) | 200.136.**N**.(preencher) | 255.255.255.(preencher) | 200.136.**N**.(preencher) | (preencher GUA/prefixo, se permitido) | Automático, se permitido | FE80::1, se permitido |
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

### Planejamento do Endereçamento dos Clientes — Entrega 1

| Clientes | IPv4 previsto | IPv6 previsto | Gateway e DNS |
| :--- | :--- | :--- | :--- |
| PCs cabeados de cada campus | DHCPv4 | SLAAC / DHCPv6 stateless | Infraestrutura da respectiva LAN |
| Futuros notebooks Wi-Fi de cada campus | DHCPv4 | SLAAC / DHCPv6 stateless | Mesmas sub-redes, gateway e DNS utilizados pelos PCs cabeados |

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

### Endereçamento Recebido pelos Notebooks

| Campus | IPv4 / máscara | IPv6 GUA / prefixo | Gateway IPv4 | Gateway IPv6 | DNS IPv4 / IPv6 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Pato Branco** | (preencher) | (preencher) | (preencher) | (preencher) | (preencher) |
| **Francisco Beltrão** | (preencher) | (preencher) | (preencher) | (preencher) | (preencher) |
| **Dois Vizinhos** | (preencher) | (preencher) | (preencher) | (preencher) | (preencher) |

### Resultados dos Testes da Tarefa 9

*Preencha cada célula com o resultado observado: “OK” ou a falha identificada.*

| Teste | Pato Branco | Francisco Beltrão | Dois Vizinhos |
| :--- | :--- | :--- | :--- |
| Associação com senha correta e falha com senha incorreta | (preencher) | (preencher) | (preencher) |
| IPv4/IPv6 automáticos e mesmos prefixos, gateway e DNS da LAN cabeada | (preencher) | (preencher) | (preencher) |
| Ping para PC cabeado, gateway e Servidor Web local em IPv4/IPv6 | (preencher) | (preencher) | (preencher) |
| Acesso ao Servidor Web local por nome | (preencher) | (preencher) | (preencher) |
| Ping para os Servidores Web dos outros dois campi em IPv4/IPv6 | (preencher) | (preencher) | (preencher) |
| Acesso aos Servidores Web remotos por nome | (preencher) | (preencher) | (preencher) |
| Conexão pela Gi1, DHCP do AP desativado e rede cabeada funcional | (preencher) | (preencher) | (preencher) |

---

## Conferência das Entregas

### Entrega 1 — Tarefas 1 e 2

- [ ] Nome, RA e curso preenchidos.
- [ ] Tarefa 1: sub-redes IPv4/IPv6 e reservas para expansão documentadas.
- [ ] Tarefa 2: roteadores, switches e servidores com endereçamento completo.
- [ ] Futuros APs com IPv4, máscara e gateway já calculados e registrados.
- [ ] IPv6/prefixo e gateway dos APs planejados quando o modelo permitir; limitações de gerenciamento identificadas.
- [ ] DHCPv4 e SLAAC/DHCPv6 stateless indicados para PCs e futuros notebooks.
- [ ] Documento salvo como `trabalho-documentacao-v1-NomeAluno.md`.

### Entrega 2 — Correções e Tarefa 3

- [ ] Tarefas 1 e 2 revisadas e corrigidas, quando necessário, incluindo os futuros APs.
- [ ] Tarefa 3: tabelas IPv4/IPv6 completas para todos os roteadores 2811.
- [ ] Fluxo assimétrico conforme o enunciado.
- [ ] Documento salvo como `trabalho-documentacao-v2-NomeAluno.md`.

### Entrega 3 — Rede Cabeada

- [ ] Documentação das Tarefas 1, 2 e 3 corrigida e coerente com a implementação.
- [ ] Endereços dos futuros APs mantidos no planejamento e reservados.
- [ ] Topologia cabeada da Figura 1 implementada e testes da Tarefa 8 realizados.
- [ ] Scripts dos roteadores e switches incluídos, com um `.txt` por equipamento.
- [ ] Arquivo `trabalho-entrega3-NomeAluno.zip` com documentação v3, scripts e topologia cabeada `.pkt`.

### Entrega 4 — Final com Wi-Fi

- [ ] APs e notebooks incluídos na mesma topologia, conforme a Figura 2.
- [ ] Endereços dos APs configurados conforme o planejamento inicial.
- [ ] Parâmetros Wi-Fi e resultados dos testes registrados nesta seção da Tarefa 9.
- [ ] Cabo na Gi1 do AP, DHCP desativado e WPA2-PSK/AES configurado.
- [ ] Notebooks nas mesmas sub-redes da LAN cabeada, com endereçamento automático.
- [ ] Comunicação local e remota em IPv4/IPv6 e acesso aos serviços por nome conferidos.
- [ ] Rede cabeada continua funcional após a expansão.
- [ ] Arquivo `trabalho-final-NomeAluno.zip` com documentação final, scripts e topologia completa `.pkt`.

Para conferir os itens pontuados e registrar a nota, utilize a [checklist de avaliação](checklist-avaliacao.md).