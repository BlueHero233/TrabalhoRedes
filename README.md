# Trabalho: Integração de habilidades - 2026/2

## Disciplina: Redes de Computadores

### Cursos: Engenharia de Computação / Tecnologia em Análise e Desenvolvimento de Sistemas

## Objetivo

Este trabalho prático tem como objetivo proporcionar aos alunos a aplicação dos conceitos de redes de computadores por meio do desenvolvimento de uma topologia de rede que simula um cenário real de interligação de campi, serviços de infraestrutura e integração entre redes cabeadas e Wi-Fi.

Ao concluir esta atividade, você será capaz de demonstrar que obteve as seguintes habilidades:

  * **Projetar a Rede Lógica:** Aplicar **VLSM em IPv4** e sub-redes em **IPv6** para criar um esquema de endereçamento eficiente para a topologia.
  * **Configurar Serviços de Rede:** Implementar e integrar serviços essenciais de infraestrutura (**DHCP, DNS e HTTP**) em uma arquitetura distribuída.
  * **Definir e Implementar Rotas:** Criar e configurar **rotas estáticas** para viabilizar a comunicação entre redes remotas, utilizando fluxo assimétrico em IPv4 e IPv6.
  * **Configurar Topologia:** Configurar roteadores e switches utilizando **interface de linha de comando (CLI)** e configurar servidores, PCs, notebooks e pontos de acesso pelas interfaces disponíveis no Packet Tracer.
  * **Integrar o Acesso Wi-Fi:** Configurar um **ponto de acesso (AP)** em cada LAN, com autenticação **WPA2-PSK/AES**, permitindo que clientes sem fio utilizem a mesma sub-rede e os mesmos serviços dos computadores cabeados.
  * **Verificar a Conectividade:** Garantir a comunicação plena entre todos os elementos da rede, validando a conectividade em IPv4, IPv6 e a **resolução de nomes de domínio (DNS)**.
  * **Definir e Implementar Segurança:** Configurar e validar **medidas básicas de segurança** e acesso remoto seguro (SSH) nos equipamentos intermediários.
  * **Documentar a Rede:** Realizar a documentação completa do projeto de rede.

## Descrição da Atividade e Topologia

Neste trabalho, você deverá projetar e implementar uma topologia de rede que interliga centros de pesquisa associados aos campi da UTFPR localizados na região sudoeste do Paraná, nas cidades de Pato Branco, Francisco Beltrão e Dois Vizinhos. A topologia a ser utilizada como referência está apresentada na [Figura 1](#figura1).

<a id="figura1"></a>

![Figura 1: Topologia física do trabalho, com servidores, computadores cabeados e acesso Wi-Fi em cada campus.](topologia-trabalho.png "Topologia física do trabalho")

*Figura 1 — Topologia física de referência para o trabalho.*


Durante o desenvolvimento da atividade, será necessário realizar o planejamento da rede, configurar os equipamentos de interconexão (roteadores, switches e APs), além dos dispositivos finais (servidores, PCs e notebooks), e assegurar que todos os centros estejam corretamente interligados, com roteamento funcional tanto em IPv4 quanto em IPv6. Além disso, cada campus deverá ter sua própria infraestrutura de serviços, conforme apresentado no [Quadro 1](#quadro-1-infraestrutura-de-serviços-por-campus):

<a id="quadro-1-infraestrutura-de-serviços-por-campus"></a>

#### **Quadro 1: Infraestrutura de Serviços por Campus**

| Campus | Servidor DNS/DHCP | Servidor Web | Subdomínio |
| :--- | :--- | :--- | :--- |
| **Pato Branco** | `SRV-PB-DNS-DHCP` | `SRV-PB-WEB` | `www.pb.utfpr.tec.br` |
| **Francisco Beltrão** | `SRV-FB-DNS-DHCP` | `SRV-FB-WEB` | `www.fb.utfpr.tec.br` |
| **Dois Vizinhos** | `SRV-DV-DNS-DHCP` | `SRV-DV-WEB` | `www.dv.utfpr.tec.br` |

Cada LAN deverá conter **2 PCs cabeados, 2 servidores, 1 AP e 1 notebook com interface Wi-Fi**, conforme a Figura 1. O AP será implementado utilizando um **roteador sem fio**, conectado ao switch da respectiva LAN.

> **Conexão obrigatória do AP:** conecte o cabo que vem do switch à porta **Gi1 (Gigabit Ethernet 1) do roteador sem fio**. Essa é uma porta LAN do equipamento. Com essa conexão e o servidor DHCP do roteador sem fio desativado, os clientes Wi-Fi deverão pertencer à **mesma sub-rede dos computadores cabeados**, utilizando o gateway e os servidores do campus. A porta Internet/WAN do roteador sem fio deverá permanecer sem conexão.

A entrega deste trabalho deverá contemplar a documentação detalhada do projeto de rede e a topologia configurada e funcional no Packet Tracer, incluindo os clientes cabeados e sem fio.

-----

## 📑 Tarefa 1: Projetar e Documentar as Sub-redes (0,5 Ponto)

Utilize o bloco de endereços **IPv4 200.136.N.0/24** e **IPv6 2001:DB8:CAFE:NN00::/56** (em que **N** e **NN** são os dois últimos dígitos do seu RA) para criar as sub-redes, de acordo com as seguintes especificações:

1.  **Prefixos IPv4:** /26 para Pato Branco, /27 para Francisco Beltrão/Dois Vizinhos e futuros centros, /30 para enlaces WAN.
    - Deve-se prever a expansão da rede com três novos centros de pesquisa, localizados na região oeste do Paraná, nas cidades de Toledo, Medianeira e Santa Helena, as sub-redes para esses três centros deve utilizar o prefixo **/27**.
2.  **Prefixos IPv6:** /64 para todas as LANs, /112 para enlaces WAN.
3.  **Alocação das sub-redes para LANs:**
    - Utilize a **primeira sub-rede** para a LAN de **Pato Branco**.
    - Utilize a **segunda sub-rede** para a LAN de **Francisco Beltrão**.
    - Utilize a **terceira sub-rede** para a LAN de **Dois Vizinhos**.
    - Reserve a **quarta, quinta e sexta sub-redes** para os futuros centros de pesquisa que estão em implantação na região oeste do estado
4.  **Alocação das sub-redes para WANs:**
    - No IPv4, utilize a **última sub-rede /27 disponível** para subdividir em blocos **/30**, destinados aos enlaces entre roteadores (**pb-vit, vit-fb, fb-ita, ita-pb, ita-dv**, e também os enlaces para os novos centros de pesquisa).
    - No IPv6, utilize a **última sub-rede /64 disponível** para subdividir em blocos **/112**, destinados aos mesmos enlaces entre roteadores.


> **Integração do Wi-Fi:** o AP e seu notebook pertencem à LAN do respectivo campus. Portanto, a inclusão do Wi-Fi utiliza as sub-redes IPv4 e IPv6 já previstas para PB, FB e DV.

> 💡 **Dica:** Você pode incluir as informações de sub-redes diretamente na topologia (no Packet Tracer) para facilitar a visualização e organização do projeto.

  * **Documentar** todas as sub-redes (IPv4 e IPv6) conforme o [modelo](trabalho-documentacao-modelo.md).


-----

<a id="tarefa-2"></a>

## 🖥️ Tarefa 2: Plano de Endereçamento Lógico (Documentação) (0,5 Ponto)

Esta tarefa exige a documentação completa do esquema de endereçamento lógico, definindo os endereços IPv4 e IPv6 (Global Unicast Address-GUA e Link-Local) para a infraestrutura e o uso de endereçamento automático para os clientes cabeados (PCs) e sem fio (notebooks). O endereço de gerenciamento do AP também deverá ser documentado.

### 2.1. Endereçamento Estático (LANs e WANs)

Os endereços IPv4 e os endereços IPv6 GUA devem ser atribuídos **manualmente** aos dispositivos de infraestrutura (roteadores, switches e servidores), seguindo a ordem de host válido da respectiva sub-rede. Para os APs, configure manualmente o IPv4 de gerenciamento da LAN; o IPv6 de gerenciamento será exigido somente se o modelo de roteador sem fio permitir essa configuração.

#### A. Endereçamento nas LANs (Pato Branco, Francisco Beltrão e Dois Vizinhos)

Em cada LAN, os **cinco primeiros** endereços de host válidos são reservados para a infraestrutura de serviços conforme descrito no [**Quadro 2**](#quadro-2-regras-de-endereçamento-estático-fixo-nas-lans):

<a id="quadro-2-regras-de-endereçamento-estático-fixo-nas-lans"></a>

#### **Quadro 2: Regras de Endereçamento Estático Fixo nas LANs**

| Endereço de Host Válido | Dispositivo e Função | Endereçamento (Manual/Estático) |
| :--- | :--- | :--- |
| **Primeiro** | Interface **Fa0/0 do Roteador** (Default Gateway) | IPv4 e IPv6 GUA |
| **Segundo** | **SVI do Switch** (Gerenciamento) | IPv4 e IPv6 GUA |
| **Terceiro** | Servidor **DHCP/DNS** | IPv4 e IPv6 GUA |
| **Quarto** | Servidor **Web** | IPv4 e IPv6 GUA |
| **Quinto** | **AP** (gerenciamento da LAN do roteador sem fio) | IPv4; IPv6 GUA, se o modelo permitir |


#### B. Endereçamento nos Enlaces WAN (Seriais e Fa0/1)

  * **Interfaces Seriais (Se0/0/0 e Se0/0/1):**
      * A interface **Se0/0/0** de cada roteador (que será a **DCE**,  com clock rate de **56000**) usará o **primeiro endereço de host válido** para **IPv4** e o **primeiro GUA** para **IPv6**
      * A interface **Se0/0/1** de cada roteador usará o **segundo endereço de host válido** para **IPv4** e o **segundo GUA** para **IPv6**.
  * **Enlace Ethernet (Itapejara D'Oeste - Dois Vizinhos):**
      * Interface **Fa0/1** do roteador **Itapejara D’Oeste** usará o **primeiro** endereço de host válido (IPv4 e IPv6 GUA) da sub-rede.
      * Interface **Fa0/1** do roteador **Dois Vizinhos** usará o **segundo** endereço de host válido (IPv4 e IPv6 GUA) da sub-rede.

### 2.2. Endereçamento Dinâmico para Clientes (DHCP)

Os clientes cabeados (**PCs**) e sem fio (**notebooks**) deverão obter o endereçamento **automaticamente via DHCPv4**, para IPv4, e **SLAAC/DHCPv6 stateless**, para IPv6. O endereço IPv6 GUA será formado por SLAAC, o gateway será aprendido por Router Advertisement (RA) e as informações adicionais de DNS serão obtidas por DHCPv6 stateless.

Os notebooks deverão receber essas configurações dos **mesmos equipamentos que atendem os PCs cabeados** da respectiva LAN. O servidor DHCP do roteador sem fio deverá permanecer **desativado**.

### 2.3. Regras de Endereçamento Link-Local (IPv6)

O endereçamento **Link-Local (`FE80::/10`)** deve seguir as seguintes regras específicas:

  * **Interfaces LAN (Fa0/0) dos Roteadores:** O endereço de Link-Local deve ser especificado **manualmente** como **`FE80::1`**.
  * **Interfaces WAN (Seriais/Fa0/1) dos Roteadores:** O endereço de Link-Local deve ser configurado automaticamente via **EUI-64**.
  * **Computadores (PCs), Notebooks e Servidores:** Os endereços de Link-Local devem ser configurados automaticamente via **EUI-64**.


### 2.4. Detalhamento do Endereçamento IPv6 (Requisito de Gateway)

Ao documentar o endereçamento dos PCs, Notebooks, Servidores e Switches, o **Default Gateway IPv6** deve ser especificado como o endereço Link-Local do roteador: **`FE80::1`**.

-----

  * **Documentar** o endereçamento *estático* completo (IPv4/IPv6, máscaras/prefixos e Endereço Link-Local) de **TODOS** os roteadores, switches e servidores conforme o [modelo](trabalho-documentacao-modelo.md).
  * **Documentar** o IPv4 de gerenciamento, máscara e gateway de cada AP. Registrar também o IPv6 de gerenciamento, caso esteja disponível no modelo utilizado.
  * **Documentar** o planejamento do Wi-Fi de cada campus: nome do AP, SSID, segurança WPA2-PSK/AES, senha e porta de conexão **Gi1**. Para PCs e notebooks, indicar o uso de **DHCPv4 e SLAAC/DHCPv6 stateless**.


-----

## 🗺️ Tarefa 3: Roteamento Estático (Tabelas - Documentação) (0,5 Ponto)

Esta tarefa consiste em definir e documentar as rotas estáticas necessárias em **TODOS** os roteadores modelo 2811 para garantir a conectividade entre as LANs. O fluxo de pacotes entre as LANs deve percorrer o anel no **sentido horário**, produzindo caminhos distintos de ida e volta. Por exemplo:
- **Ida:** Pato Branco $\rightarrow$ Vitorino $\rightarrow$ Francisco Beltrão.
- **Volta:** Francisco Beltrão $\rightarrow$ Itapejara D’Oeste $\rightarrow$ Pato Branco. 

Para cada roteador, identifique as redes remotas que precisam de rotas estáticas, documente as **Tabelas de Roteamento** para IPv4 e IPv6 conforme o [modelo](trabalho-documentacao-modelo.md).
  - Neste trabalho, rotas para redes diretamente conectadas não precisam ser documentadas, mas lembre-se que essas rotas existem nos roteadores e são configuradas automaticamente pelo sistema operacional do roteador.

## 💻 Tarefa 4: Criação da Topologia no Packet Tracer (0,0 Ponto)

Criar a topologia no Packet Tracer, conforme ilustrado na [Figura 1](#figura1):

* Cada LAN deverá conter **2 PCs cabeados, 2 servidores, 1 roteador sem fio atuando como AP e 1 notebook com interface Wi-Fi**.
* Conecte o switch de cada LAN à porta **Gi1 (Gigabit Ethernet 1) do AP** utilizando cabo Ethernet direto. A identificação **Gi1 refere-se à porta do roteador sem fio**; no switch, utilize uma porta Ethernet disponível.
* O notebook deverá se conectar ao AP por **Wi-Fi**, utilizando o SSID e a senha definidos para o campus.
* Utilize *roteadores modelo 2811* (adicione uma interface WIC-2T no slot 0 para as conexões WAN) e *switches modelo 2960*, equipamentos disponíveis no laboratório de redes.
* Na área de trabalho de cada topologia, informe o **RA + Nome do aluno**.
* Recomenda-se inserir as informações de endereçamento na área de trabalho do Packet Tracer para facilitar a visualização.

## ⚙️ Tarefa 5: Configuração dos Dispositivos Intermediários (Switches, Roteadores e APs)

Esta tarefa consiste na configuração, via *command line interface* (CLI), do endereçamento dos switches e roteadores modelo 2811, assim como das rotas estáticas nos roteadores, conforme a documentação das Tarefas 2 e 3. Os roteadores sem fio utilizados como APs deverão ser configurados pela interface gráfica do Packet Tracer, conforme a seção 5.3.

### 5.1. Configuração Básica e Endereçamento de Interfaces

1.  **Nomes dos Dispositivos (Hostname):**
    Nomear os roteadores e switches no IOS conforme o padrão: `r-pb-nnn`, `sw-pb-nnn`, etc., em que `nnn` são as iniciais do seu nome (Ex: `r-pb-ff`).
    * Roteador Pato Branco: `r-pb-nnn`
    * Roteador Francisco Beltrão: `r-fb-nnn`
    * Roteador Itapejara: `r-ita-nnn`
    * Roteador Vitorino: `r-vit-nnn`
    * Roteador Dois Vizinhos: `r-dv-nnn`
    * Switch Pato Branco: `sw-pb-nnn`
    * Switch Francisco Beltrão: `sw-fb-nnn`
    * Switch Dois Vizinhos: `sw-dv-nnn`

    Nos roteadores sem fio, defina o nome de exibição no Packet Tracer:
    * AP Pato Branco: `ap-pb-nnn`
    * AP Francisco Beltrão: `ap-fb-nnn`
    * AP Dois Vizinhos: `ap-dv-nnn`

2.  **Endereçamento Estático:**
    Atribuir os endereços IP (IPv4/Máscara e IPv6/Prefixos) a **TODAS** as interfaces de switches (SVI) e roteadores, conforme documentado na Tarefa 2.
     > **💡 Lembrete**: Para IPv6 nos switches, lembre-se de configurar o template dual-stack conforme visto em aula.


3.  **Descrições de Interfaces:**
    Inserir descrições em todas as interfaces dos roteadores, indicando a rede ou enlace ao qual estão conectadas:
    * Exemplo: `description LAN Pato Branco`
    * Exemplo: `description Enlace pb-vit`

4.  **Sincronização (Clock Rate):**
    A interface serial `Se0/0/0` de cada enlace será o DCE e deve ser configurada com o comando:
    * `clock rate 56000`
    * *Nota: Este comando deve ser aplicado apenas nas interfaces seriais designadas como DCE.*

### 5.2. Configuração de Roteamento Estático

Implementar as rotas estáticas definidas na Tarefa 3 em todos os roteadores.
> *Lembre-se:* somente é necessário configurar rotas estáticas para redes remotas; rotas para redes diretamente conectadas são configuradas **automaticamente** pelos roteadores.

> **💡 Configuração IPv6 em Roteadores**: É necessário ativar o roteamento IPv6 com o comando `ipv6 unicast-routing` no modo de configuração global.



### 5.3. Configuração dos Pontos de Acesso Wi-Fi

Em cada campus, configure o roteador sem fio para atuar como **ponto de acesso da LAN**, seguindo os requisitos abaixo:

1. **Conexão à rede cabeada:** mantenha o cabo do switch conectado à porta **Gi1 (Gigabit Ethernet 1) do roteador sem fio**. Essa conexão integra o segmento Wi-Fi à LAN cabeada do campus.
2. **Endereçamento de gerenciamento:** configure, na LAN do roteador sem fio, o **quinto endereço IPv4 válido** da sub-rede, com a máscara correspondente. Quando houver os respectivos campos, configure o gateway como o **primeiro endereço válido** da LAN e o DNS como o **terceiro endereço válido**. Registre essas informações na documentação. Se o equipamento permitir IPv6 de gerenciamento, utilize o identificador de interface `::5` dentro do prefixo /64 do campus e o gateway `FE80::1`.
3. **DHCP do roteador sem fio:** desative o servidor **DHCPv4** desse equipamento. Os notebooks deverão receber endereços do servidor `SRV-[CAMPUS]-DNS-DHCP`. Se o modelo oferecer servidor DHCPv6 ou anúncios IPv6 próprios (RA), desative também essas funções no AP; os anúncios da LAN deverão ser fornecidos pelo roteador 2811 do campus.
4. **SSID:** configure um SSID específico para cada campus, incluindo suas iniciais, conforme o padrão:
   * Pato Branco: `UTFPR-PB-nnn`.
   * Francisco Beltrão: `UTFPR-FB-nnn`.
   * Dois Vizinhos: `UTFPR-DV-nnn`.
5. **Segurança Wi-Fi:** utilize **WPA2-PSK (WPA2 Personal)** com criptografia **AES** e uma senha com, no mínimo, **10 caracteres**. Documente a senha utilizada no ambiente simulado.
6. **Clientes Wi-Fi:** associe o notebook ao SSID do campus e configure-o para receber IPv4 por **DHCP** e IPv6 por **Auto Config (SLAAC/DHCPv6 stateless)**. Verifique se ele utiliza a mesma sub-rede, gateway e servidores DNS dos PCs cabeados.

> O endereço IP do AP é destinado ao gerenciamento. O **gateway dos clientes cabeados e sem fio continua sendo o roteador 2811 da LAN**. A comunicação dos notebooks com a infraestrutura deverá funcionar em IPv4 e IPv6, inclusive quando o modelo de AP disponibilizar gerenciamento apenas em IPv4.

## 💻 Tarefa 6: Configuração dos Serviços, PCs e Notebooks

Esta tarefa exige configurar o endereçamento estático dos servidores, ativar os serviços DHCP, DNS e Web e configurar os PCs cabeados e notebooks sem fio para receberem endereçamento automático. Todos os clientes de uma LAN deverão utilizar os serviços do respectivo campus.

### 6.1. Configuração do Endereçamento Estático nos Servidores

Atribua manualmente os endereços IPv4 e IPv6 aos Servidores no Packet Tracer (Desktop $\rightarrow$ IP Configuration), utilizando as regras de endereçamento fixo definidas na [**Tarefa 2**](#tarefa-2):

* **Servidores DNS/DHCP:**
    * **IPv4:** Atribua o endereço IPv4, Máscara, Default Gateway (Primeiro IP da LAN) e o Servidor DNS.
    * **IPv6:** Atribua o endereço **IPv6 (Global com Prefix)** e o **Gateway Padrão (Link-Local do Roteador: `FE80::1`)**.
* **Servidores Web:**
    * **IPv4:** Atribua o endereço IPv4, Máscara, Default Gateway e o Servidor DNS.
    * **IPv6:** Atribua o endereço IPv6 (Global com Prefix) e o **Gateway Padrão (Link-Local do Roteador: `FE80::1`)**.

### 6.2. Configuração do Serviço Web (Nos Servidores Web)

Ative o serviço **HTTP** e substitua o arquivo `index.html` com o código HTML fornecido ([**Apêndice**](#apêndice-código-html-padrão-para-servidores-web)), personalizando o **Nome, RA e o Campus** correto.

### 6.3. Configuração do Serviço DNS (Nos Servidores DNS/DHCP)

Ative o serviço **DNS** e configure o registro Tipo A (IPv4) e Tipo AAAA (IPv6) em cada um dos três servidores DNS para **todos os servidores WEB**, garantindo que a resolução de nomes de campi remotos funcione.

> *Instrução:* **CADA UM** dos três Servidores DNS deve ser configurado com o registro Tipo A e Tipo AAAA para **todos os três subdomínios** (Pato Branco, Francisco Beltrão e Dois Vizinhos), apontando para o IPv4 (registro A) e para o IPv6 GUA (registro AAAA) do respectivo Servidor Web,  conforme o [**Quadro 3**](#quadro-3-arquitetura-de-serviços-por-campus-subdomínios-e-ips),

<a id="quadro-3-arquitetura-de-serviços-por-campus-subdomínios-e-ips"></a>

#### **Quadro 3: Arquitetura de Serviços por Campus (Subdomínios e IPs)**

| Campus | Subdomínio | Servidor Web (IP GUA de Destino) |
| :--- | :--- | :--- |
| **Pato Branco** | `www.pb.utfpr.tec.br` | IPv4 e IPv6 GUA do SRV-PB-WEB (4º IP de PB) |
| **Francisco Beltrão** | `www.fb.utfpr.tec.br` | IPv4 e IPv6 GUA do SRV-FB-WEB (4º IP de FB) |
| **Dois Vizinhos** | `www.dv.utfpr.tec.br` | IPv4 e IPv6 GUA do SRV-DV-WEB (4º IP de DV) |

### 6.4. Configuração do Serviço DHCP (Nos Servidores DNS/DHCP)

Ative e configure os serviços de **DHCPv4** e **DHCPv6 Stateless** em cada servidor DNS/DHCP para atender os PCs cabeados e notebooks sem fio de sua respectiva LAN.

#### 6.4.1. Configuração do Serviço DHCPv4

Configure o serviço DHCP para distribuir endereços IPv4 automaticamente.

##### Procedimento para Cada Servidor DNS/DHCP:

1.  **Ativação do Serviço DHCPv4:**
    * Abra o servidor no Packet Tracer
    * Vá em `Services` → `DHCP`
    * Ative o serviço **ON**

2.  **Configuração do Pool DHCPv4:**
    * **Pool Name**: `LAN-[CAMPUS]` (Ex: `LAN-PB`, `LAN-FB`, `LAN-DV`)
    * **Default Gateway**: **Primeiro endereço válido** da sub-rede (Interface Fa0/0 do roteador - consulte Tarefa 2)
    * **DNS Server**: **Terceiro endereço válido** da sub-rede (IP do próprio servidor DNS/DHCP - consulte Tarefa 2)
    * **Start IP Address**: **Sexto endereço válido** da sub-rede
    * **Subnet Mask**: Máscara correspondente à sub-rede (consulte Tarefa 1)
    * **Maximum Number of Users**: **Total de hosts da sub-rede menos 5** (reservas: Gateway, Switch, Servidor DNS/DHCP, Servidor Web e AP)

##### Referência para cálculos:

| Campus | Prefixo | Total Hosts | Máscara | Max Users (Total - 5) |
| :--- | :--- | :--- | :--- | :--- |
| **Pato Branco** | /26 | 62 | 255.255.255.192 | 57 |
| **Francisco Beltrão** | /27 | 30 | 255.255.255.224 | 25 |
| **Dois Vizinhos** | /27 | 30 | 255.255.255.224 | 25 |

#### 6.4.2. Configuração do Serviço DHCPv6 Stateless

Configure o serviço DHCPv6 Stateless para fornecer informações de DNS IPv6 automaticamente.

##### Procedimento para Cada Servidor DNS/DHCP:

1.  **Ativação do Serviço DHCPv6:**
    * Vá em `Services` → `DHCPv6`
    * Ative o serviço **ON**

2.  **Configuração do Pool DHCPv6 Stateless:**
    * **Pool Name**: `LAN-[CAMPUS]-v6` (Ex: `LAN-PB-v6`, `LAN-FB-v6`, `LAN-DV-v6`)
    * **DNS Server**: **IPv6 GUA do próprio servidor DNS/DHCP** (consulte Tarefa 2)

##### Configuração adicional nos roteadores:

Para habilitar o DHCPv6 Stateless, configure em **cada roteador** na interface Fa0/0:

```cisco
interface FastEthernet0/0
 ipv6 nd other-config-flag
```

> **💡 Nota**: O comando `ipv6 nd other-config-flag` informa aos clientes para obter configurações adicionais (DNS) via DHCPv6 Stateless.

### 6.5. Configuração dos PCs e Notebooks

Configure os PCs e notebooks para receberem endereçamento automático. Antes de configurar o endereçamento dos notebooks, confirme a associação ao SSID correto e a autenticação WPA2-PSK/AES, conforme a seção 5.3.

#### Procedimento para cada PC e notebook

1.  **Ativação do DHCP/SLAAC:**
    - Abra o PC ou notebook no Packet Tracer.
    - Vá em `Desktop` $\rightarrow$ `IP Configuration`.
    - Selecione a opção **DHCP**.
    - Aguarde a mensagem "DHCP Request Successful" para IPv4.
    - **IPv6 Configuration**: `Auto Config`
    - **IPv6 Gateway**: **Deixar em branco** (obtido automaticamente via Router Advertisement)

2.  **Verificação do Endereçamento (DHCPv4 e SLAAC):**
    * Após receber o IP, abra o `Command Prompt` no PC ou notebook.
    * Execute o comando: `ipconfig /all`
    * **Valide se o PC ou notebook recebeu corretamente:**
        * Um endereço IPv4 e Máscara.
        * O **Default Gateway IPv4** (Primeiro IP da LAN).
        * O **DNS Server IPv4** (Terceiro IP da LAN).
        * Um endereço **IPv6 GUA** (SLAAC), pertencente ao /64 do campus.
        * O **DNS Server IPv6** fornecido por DHCPv6 stateless.
        * O **Link-Local** do Roteador como **Gateway IPv6** (`FE80::1`).


3.  **Teste de Conectividade e Serviço Local:**
    * **Teste 1 (Servidor Local):** No `Command Prompt`, execute `ping` para o IP IPv4 do Servidor Web local.
    * **Teste 2 (Acesso Web):** No `Web Browser` do PC ou notebook, acesse o domínio local (`http://www.pb.utfpr.tec.br`) para confirmar se a página personalizada é exibida.




## 🔒 Tarefa 7: Configuração de Segurança Básica

Esta tarefa consiste na implementação de medidas de segurança e acesso seguro, via CLI, em **TODOS os roteadores modelo 2811**. A segurança dos roteadores sem fio utilizados como APs será configurada conforme a seção 5.3. 

### 7.1. Implementação de Medidas de Segurança

Implemente as seguintes configurações em **TODOS os roteadores modelo 2811**:

1.  **Banner de Aviso:** 
    - Configure o **Banner MOTD** conforme a seguir, personalizado com seu nome.

```
--------------------------------------------------------------------------
|                                                                        |
|                          Roteador [NOME DO ROTEADOR]                   |
|                                                                        |
|               ATENÇÃO Acesso Restrito a pessoas autorizadas!           |
|                                                                        |
|          Administrador: SEU NOME COMPLETO (email@seuemail.com)         |
|                                                                        |
--------------------------------------------------------------------------
```

2.  **Segurança de Senhas:**
    - Exigir que as senhas tenham comprimento mínimo de **10 caracteres**.
    - Ativar o serviço de **criptografia de senhas** em texto simples.
3.  **Proteção de Acesso:**
    - Proteger o acesso ao modo EXEC privilegiado com a senha secreta **`@dmin-nome`** (sendo `nome` o seu primeiro nome).
    - Proteger o acesso via console com a senha **`@Cons-nome`** (sendo `nome` o seu primeiro nome).
    - Se necessário, acrescente dígitos ao final das senhas personalizadas para atender ao mínimo de **10 caracteres**.
4.  **Controle de Acesso:**
    - Encerrar as conexões via console e VTY após **5 minutos** de inatividade.
    - Implementar a proteção contra ataques de força bruta: bloquear tentativas de login por **120 segundos** se houver **3 tentativas** de login com falha dentro de **60 segundos**.

### 7.2. Acesso Remoto Seguro (SSH)

Configure o acesso remoto seguro (SSH) nas linhas VTY 0 15, exigindo autenticação via usuário local:

1.  **Nome de Domínio:** Configurar **`nome.sobrenome.com.br`** como nome de domínio local.
2.  **Usuário Local:** Criar um usuário com o seu primeiro nome (`nome`) e a senha **`ssh@Network1ng`**.
3.  **Geração de Chave:** Gerar a chave RSA para o SSH com tamanho de **1024 bits**.
4.  **Configuração VTY:** Limitar o acesso nas linhas VTY 0 15 apenas ao protocolo **SSH** e com autenticação local.


---

## ✅ Tarefa 8: Testes e Validação de Conectividade e Serviços

Esta tarefa consiste na comprovação da funcionalidade da rede em três estágios: serviços e conectividade local (cabeada e Wi-Fi), comunicação de ponta a ponta (roteamento WAN) e segurança básica.

### 8.1. Estágio 1: Serviços e Conectividade Local (Verificação de LAN)

Para cada LAN, realize os seguintes testes:

1. **Teste de DHCP/SLAAC:** em um PC cabeado e no notebook, execute `ipconfig /all` e valide o IPv4, máscara, IPv6 GUA, gateways e servidores DNS recebidos. Confirme que os dois clientes pertencem às mesmas sub-redes IPv4 e IPv6 do campus.
2. **Teste de conectividade local:** execute **`ping`**, em IPv4 e IPv6, do PC e do notebook para o Servidor Web local. Teste também a comunicação entre o notebook e um PC cabeado.
3. **Teste de serviço local:** no `Web Browser` do PC e do notebook, acesse o domínio do campus (por exemplo, `http://www.pb.utfpr.tec.br`) para confirmar o funcionamento do DNS e HTTP.
4. **Teste de autenticação Wi-Fi:** confirme que o notebook se conecta ao SSID correto com a senha configurada e que a tentativa com senha incorreta falha. Ao concluir, restaure a senha correta e mantenha o notebook conectado.
5. **Verificação do AP:** confira a conexão pela **Gi1**, o IPv4 de gerenciamento e a desativação do DHCP do roteador sem fio.

### 8.2. Estágio 2: Comunicação Inter-Redes (Roteamento WAN)

Esta etapa comprova o funcionamento das rotas estáticas e a integração total dos serviços.

1.  **Teste de Conectividade Total (`ping`):**
    Execute o comando **`ping`** a partir de um PC de Pato Branco para **todas as outras interfaces endereçadas da topologia** (dispositivos finais e intermediários, incluindo os notebooks) em:
    * **IPv4**
    * **IPv6**, utilizando os endereços GUA. Os endereços link-local serão testados somente no respectivo enlace. O gerenciamento IPv6 do AP será incluído apenas se estiver disponível no modelo utilizado.

2.  **Teste de Resolução e Acesso Remoto:**
    * Em um PC de Pato Branco, execute `nslookup www.fb.utfpr.tec.br` para confirmar a resolução de nomes.
    * No `Web Browser`, acesse o domínio remoto (`http://www.fb.utfpr.tec.br`) para provar o sucesso do roteamento e dos serviços.
    * A partir do **notebook de cada campus**, teste `ping` em IPv4 e IPv6 para um Servidor Web remoto e acesse sua página pelo nome de domínio.


### 8.3: Estágio 3: Testes de Funcionamento da Segurança Básica

Esta etapa é crucial para confirmar que as regras de segurança configuradas na Tarefa 7 estão ativas e protegendo os roteadores conforme o esperado.

1.  **Teste de Proteção contra Força Bruta:**
    * A partir de um PC, provoque **três falhas de autenticação no acesso SSH** a um roteador (por exemplo, o de Pato Branco), dentro de **60 segundos**.
    * **Verifique:** Confirme se o roteador bloqueia novas tentativas de login por **120 segundos**, verificando também o estado com `show login`.

2.  **Teste de Acesso Remoto Seguro (SSH):**
    * A partir de um PC, utilize o cliente **SSH** para acessar um roteador remoto, por meio de uma das interfaces do roteador.
    * **Comando:** `ssh -l usuario ip_do_roteador`
    * **Verifique:** Confirme se o acesso é estabelecido com sucesso e se é exigida a autenticação (senha).

3.  **Teste de Timeout de Inatividade:**
    * Inicie uma sessão de console ou SSH em um roteador.
    * **Verifique:** Deixe a sessão inativa por mais de 5 minutos e confirme se a conexão é automaticamente encerrada.

## Critérios de Avaliação

- **Tarefa 1**: 0,50 Ponto
- **Tarefa 2**: 0,50 Ponto
- **Tarefa 3**: 0,50 Ponto
- **Tarefa 8**:
  - Estágio 1: Serviços e Conectividade Local (2,5 Pontos)  
    - Funcionamento dos serviços DHCP/DNS (IPv4 e IPv6) - 1,00 Ponto, considerando o conjunto das três LANs
    - Funcionamento do Servidor Web (IPv4 e IPv6) - 0,80 Ponto
    - Funcionamento da conectividade local cabeada e Wi-Fi (IPv4 e IPv6), incluindo associação ao SSID, WPA2-PSK/AES e integração do notebook à LAN - 0,70 Ponto
  - Estágio 2: Conectividade Inter-Redes (5 Pontos)  
    - Funcionamento da Conectividade para todas as interfaces (IPv4) - 2,50 Pontos
    - Funcionamento da Conectividade para todas as interfaces (IPv6) - 2,50 Pontos
    > A pontuação será dada apenas se a funcionalidade inter-redes estiver 100% correta para todas as sub-redes, aplicando a regra TUDO-OU-NADA para cada protocolo, isto é, se falhar a conectividade para uma interface, não receberá nenhuma pontuação.

  - Estágio 3:  Funcionamento da Segurança Básica (1 Ponto)
    - Banner MOTD Configurado - 0,10 Ponto
    - Tamanho da Senha - 0,10 ponto
    - Senha Exec Privilegiado - 0,10 Ponto
    - Senha Console - 0,10 Ponto
    - Encerrar conexões após inatividade - 0,10 Ponto
    - Proteção contra ataque de força bruta - 0,10 Ponto
    - Acesso Remoto via SSH - 0,40 Ponto

## Disponibilização e Entregas

A atividade é **individual** e será disponibilizada em **15/10/2026 (quinta-feira)**. Todas as entregas deverão ser realizadas pelo **Moodle**.

| Etapa | Prazo | Conteúdo |
| :--- | :--- | :--- |
| Disponibilização | **15/10/2026 (quinta-feira)** | Enunciado, topologia física e modelo de documentação. |
| **Entrega 1** | **20/10/2026 (terça-feira)** | Documentação das sub-redes e do endereçamento dos dispositivos — **Tarefas 1 e 2**. |
| **Entrega 2** | **27/10/2026 (terça-feira)** | Correção das **Tarefas 1 e 2** e documentação das tabelas de roteamento — **Tarefa 3**. |
| **Entrega 3 — Final** | **10/11/2026 (terça-feira)** | Documentação corrigida, scripts dos equipamentos configurados via CLI e topologia completa e funcional no Packet Tracer. |

### Entrega 1 — Sub-redes e Endereçamento

Entregar o arquivo **`trabalho-documentacao-v1-NomeAluno.md`**, seguindo o [modelo de documentação](trabalho-documentacao-modelo.md), contendo:

- RA e nome do aluno.
- **Tarefa 1:** documentação das sub-redes IPv4 e IPv6, incluindo as reservas para expansão.
- **Tarefa 2:** planejamento do endereçamento dos dispositivos, incluindo o gerenciamento dos APs e a indicação de endereçamento automático para PCs e notebooks.
- Planejamento do Wi-Fi de cada campus, conforme solicitado na Tarefa 2.

**Prazo: 20/10/2026.** Após o encerramento do prazo, será disponibilizado o gabarito correspondente para conferência e correções.

### Entrega 2 — Correções e Roteamento

Entregar o arquivo **`trabalho-documentacao-v2-NomeAluno.md`**, seguindo o mesmo [modelo de documentação](trabalho-documentacao-modelo.md), contendo:

- **Tarefas 1 e 2 corrigidas**, quando necessário.
- **Tarefa 3:** tabelas de roteamento estático IPv4 e IPv6 de todos os roteadores, respeitando o fluxo assimétrico exigido.

**Prazo: 27/10/2026.** Após o encerramento do prazo, será disponibilizado o gabarito correspondente para conferência e correções.

### Entrega 3 — Entrega Final

Entregar o arquivo compactado **`trabalho-final-NomeAluno.zip`**, contendo:

- **`trabalho-documentacao-final-NomeAluno.md`**: documentação das **Tarefas 1, 2 e 3**, corrigida e coerente com a implementação final, incluindo os dados dos APs e das redes Wi-Fi.
- **Scripts de configuração dos roteadores 2811 e switches**, com um arquivo `.txt` por equipamento, nomeado com o respectivo nome (por exemplo, `r-pb-nnn.txt` e `sw-pb-nnn.txt`). As configurações dos APs realizadas pela interface gráfica deverão estar registradas na documentação.
- **`trabalho-topologia-final-NomeAluno.pkt`**: topologia com as **Tarefas 4 a 7 implementadas** e os **testes da Tarefa 8 realizados**, incluindo os três APs e notebooks, com comunicação local e entre campi em IPv4 e IPv6.

**Prazo: 10/11/2026.**

**Não serão aceitas entregas após os respectivos prazos.**

## Teste de autoria

- Não gera nota, mas é critério obrigatório para validar a autoria do trabalho, caso necessário.
- Será agendado individualmente até o último dia letivo do semestre.

---
<a id="apêndice-código-html-padrão-para-servidores-web"></a>

### Apêndice: Código HTML Padrão para Servidores WEB

```html
<html>
<head>
    <title>Centro de Pesquisa - UTFPR</title>
    <style>
        body { 
            font-family: Arial, sans-serif; 
            text-align: center; 
            margin-top: 50px; 
            background-color: #f4f4f9;
        }
        .container {
            border: 2px solid #005296; /* Cor azul UTFPR */
            padding: 20px;
            display: inline-block;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #005296;
            border-bottom: 3px solid #ffcc00; /* Cor amarela/dourada UTFPR */
            padding-bottom: 10px;
            margin-bottom: 20px;
        }
        .info {
            font-size: 1.1em;
            text-align: left;
            margin-top: 15px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Centro de Pesquisa - Campus [NOME DO CAMPUS]</h1>
        <p>A página WEB do centro de pesquisa está funcionando corretamente na rede local!</p>
        
        <div class="info">
            <p><strong>Domínio Acessado:</strong> www.[pb/fb/dv].utfpr.tec.br</p>
            <p><strong>Aluno(a):</strong> SEU NOME COMPLETO</p>
            <p><strong>RA:</strong> SEU RA</p>
        </div>
    </div>
</body>
</html>
```