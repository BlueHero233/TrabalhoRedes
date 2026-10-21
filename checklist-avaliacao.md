# Checklist de Autoavaliação e Avaliação — Redes de Computadores — 2026/2

**Nome:** ____________________  
**RA:** ____________________  
**Curso:** ____________________  
**Etapa desta cópia:** Entrega 2 / Entrega 3 / Entrega 4  
**Arquivo `.pkt` efetivamente conferido:** ____________________  
**Data e horário da última conferência:** ____________________  

Este checklist acompanha o [enunciado](README.md) e o [modelo de documentação](trabalho-documentacao-modelo.md). Ele orienta os mesmos testes utilizados na correção e permite conferir todos os requisitos para a nota máxima. O professor irá registrar a nota conforme as evidências verificadas no arquivo entregue.

## Como Preencher e Entregar

- Use **A — Atendido**, **N — Não atendido** ou **T — Não testado**. As células começam com T; altere-as somente após conferir a versão final da topologia.
- Preencha as seções exigidas até a etapa atual. Na Entrega 2, as seções 3 e 4 permanecem T por ainda não serem exigidas.
- A partir da Entrega 2, entregue uma cópia preenchida: `checklist-entrega2-NomeAluno.md`, `checklist-entrega3-NomeAluno.md` ou `checklist-final-NomeAluno.md`.
- Salve as configurações e repita os testes na versão `.pkt` que será enviada. Registre o resultado observado ou a pendência, especialmente nos itens N ou T.
- Cada verificação possui um **ID da parcela pontuada**. Várias verificações podem pertencer à mesma parcela; elas não criam pontos nem descontos separados.
- Declarar uma falha ou um item não testado não gera desconto adicional por declaração incorreta. A nota é determinada pela verificação do professor.
- Uma falha confirmada em verificação marcada A gera a perda normal da parcela e **desconto adicional de igual valor**, uma única vez por parcela. Exemplo: parcela de 0,20 perdida e declarada como atendida implica perda total de 0,40. A falha deve ser confirmada após repetir o teste nas mesmas condições.
- As correções documentais da Entrega 2 possuem desconto próprio de 0,50 por tarefa ausente/incorreta. Declarar essa tarefa como corrigida quando não estiver gera adicional de mais 0,50 por tarefa.
- A nota final de cada entrega não pode ficar negativa. Arredonde apenas o total final da entrega para duas casas decimais; preserve as frações indicadas nas parcelas.
- Ao encontrar dificuldade, registre equipamento, protocolo e resultado e procure o professor com antecedência. Solicitações nas últimas horas poderão não ser respondidas antes do prazo.

## Resumo das Entregas

| Etapa | Evidência | Prazo | Máximo |
| :--- | :--- | :--- | ---: |
| 1 | Tarefas 1 e 2 efetivamente realizadas | 20/10/2026 | 1,00 |
| 2 | Documentação corrigida, LANs, enlaces diretos, endereçamento automático, DNS e HTTP | 27/10/2026, no início da aula | 3,50 |
| 3 | Tudo da etapa anterior, roteamento e segurança | 10/11/2026 | 3,50 |
| 4 | Tudo da etapa anterior e integração Wi-Fi | A definir após a aula sobre Wi-Fi | 2,00 |
| | **Total** | | **10,00** |

## 1. Entrega 1 — Evidência da Realização

Nesta etapa, erros de cálculo/endereço não retiram pontos de uma tarefa efetivamente realizada. A correção após o gabarito será obrigatória na Entrega 2. A ausência da Entrega 1 não é recuperada pela apresentação das tarefas nas etapas seguintes.

| ID | Evidência | Valor | Conferência | Nota do professor |
| :--- | :--- | :--- | :--- | :--- |
| E1-T1 | Tabela de sub-redes efetivamente preenchida e entregue no prazo | 0,50 | T |  |
| E1-T2 | Tabela de endereçamento efetivamente preenchida, incluindo futuros APs e forma de endereçamento dos clientes, entregue no prazo | 0,50 | T |  |
|  | Total da Entrega 1 | 1,00 |  |  |


## 2. Entrega 2 — Funcionamento das LANs

### 2.1. Documentação Corrigida — Pré-requisito Cumulativo

Confira cada valor usando o gabarito e o seu RA. A correção não gera novos pontos e é exigida mesmo de quem não entregou a primeira etapa.

| ID de desconto | Verificação | Desconto se ausente/incorreta | Estado | Resultado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| DOC-T1 | Tarefa 1 corrigida: LANs, WANs e reservas; N/NN adaptados ao RA | 0,50 | T |  |
| DOC-T2 | Tarefa 2 corrigida: todos os dispositivos/interfaces e futuros APs; gateways e formas automáticas coerentes com o planejamento | 0,50 | T |  |


### 2.2. Preparação dos Equipamentos e Arquivos

Estes itens apoiam a validação dos requisitos e não possuem pontuação adicional independente.

| Equipamento | Conferência preparatória | Estado | Observações |
| :--- | :--- | :--- | :--- |
| Roteador Pato Branco | Hostname, interfaces utilizadas, descrições, endereços/prefixos e link-local conforme Tarefas 2 e 4; interfaces ligadas; clock nas DCE e IPv6 habilitado; configuração salva | T |  |
| Roteador Vitorino | Hostname, interfaces utilizadas, descrições, endereços/prefixos e link-local conforme Tarefas 2 e 4; interfaces ligadas; clock nas DCE e IPv6 habilitado; configuração salva | T |  |
| Roteador Francisco Beltrão | Hostname, interfaces utilizadas, descrições, endereços/prefixos e link-local conforme Tarefas 2 e 4; interfaces ligadas; clock nas DCE e IPv6 habilitado; configuração salva | T |  |
| Roteador Itapejara D’Oeste | Hostname, interfaces utilizadas, descrições, endereços/prefixos e link-local conforme Tarefas 2 e 4; interfaces ligadas; clock nas DCE e IPv6 habilitado; configuração salva | T |  |
| Roteador Dois Vizinhos | Hostname, interfaces utilizadas, descrições, endereços/prefixos e link-local conforme Tarefas 2 e 4; interfaces ligadas; clock nas DCE e IPv6 habilitado; configuração salva | T |  |
| Switch Pato Branco | Hostname e descrição, pilha dupla, SVI IPv4/IPv6, gateway IPv4 e aprendizado do gateway IPv6 por RA; configuração salva | T |  |
| Switch Francisco Beltrão | Hostname e descrição, pilha dupla, SVI IPv4/IPv6, gateway IPv4 e aprendizado do gateway IPv6 por RA; configuração salva | T |  |
| Switch Dois Vizinhos | Hostname e descrição, pilha dupla, SVI IPv4/IPv6, gateway IPv4 e aprendizado do gateway IPv6 por RA; configuração salva | T |  |
| SRV-PB-DNS-DHCP | Endereçamento estático IPv4/IPv6, máscara/prefixo, gateways e DNS conforme a Tarefa 2 | T |  |
| SRV-PB-WEB | Endereçamento estático IPv4/IPv6, máscara/prefixo, gateways e DNS conforme a Tarefa 2 | T |  |
| SRV-FB-DNS-DHCP | Endereçamento estático IPv4/IPv6, máscara/prefixo, gateways e DNS conforme a Tarefa 2 | T |  |
| SRV-FB-WEB | Endereçamento estático IPv4/IPv6, máscara/prefixo, gateways e DNS conforme a Tarefa 2 | T |  |
| SRV-DV-DNS-DHCP | Endereçamento estático IPv4/IPv6, máscara/prefixo, gateways e DNS conforme a Tarefa 2 | T |  |
| SRV-DV-WEB | Endereçamento estático IPv4/IPv6, máscara/prefixo, gateways e DNS conforme a Tarefa 2 | T |  |


### 2.3.PB. Testes Locais — Pato Branco

**PC escolhido como origem:** ____________________  
**Nome/identificação do outro PC:** ____________________  
**Data do teste:** ____________________


#### Endereçamento Automático — Seção 6.2


| Verificação | Parcela | Resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| PC de teste: DHCPv4 selecionado | E2-D4-PB | Opção DHCP ativa | T |  |
| PC de teste: IPv4/máscara/gateway/DNS recebidos | E2-D4-PB | Faixa e parâmetros corretos da LAN; sem utilizar reservas nem endereço duplicado | T |  |
| PC de teste: Auto Config IPv6 selecionado | E2-D6-PB | Configuração automática ativa | T |  |
| PC de teste: IPv6/prefixo/gateway/DNS recebidos | E2-D6-PB | GUA do /64 correto; gateway por RA; DNS IPv6 pelo DHCPv6 stateless | T |  |
| Outro PC: DHCPv4 selecionado | E2-D4-PB | Opção DHCP ativa | T |  |
| Outro PC: IPv4/máscara/gateway/DNS recebidos | E2-D4-PB | Faixa e parâmetros corretos da LAN; sem utilizar reservas nem endereço duplicado | T |  |
| Outro PC: Auto Config IPv6 selecionado | E2-D6-PB | Configuração automática ativa | T |  |
| Outro PC: IPv6/prefixo/gateway/DNS recebidos | E2-D6-PB | GUA do /64 correto; gateway por RA; DNS IPv6 pelo DHCPv6 stateless | T |  |


#### Conectividade Local — Seção 6.3

Execute os pings a partir do PC escolhido. Todos os resultados desta tabela pertencem à mesma parcela de 0,40 ponto da LAN.


| Destino da Tarefa 2 | Parcela | IPv4 | IPv6 GUA | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| Outro PC da própria LAN | E2-C-PB | T | T |  |
| Interface LAN do roteador — gateway | E2-C-PB | T | T |  |
| SVI do switch | E2-C-PB | T | T |  |
| SRV-PB-DNS-DHCP | E2-C-PB | T | T |  |
| SRV-PB-WEB | E2-C-PB | T | T |  |


#### DNS — Seção 6.4

Servidor DNS consultado: ____________________. Cada resposta deverá corresponder ao endereço do Servidor Web previsto na Tarefa 2.


| Domínio | Parcela | A — estado | AAAA — estado | Respostas observadas/pendência |
| :--- | :--- | :--- | :--- | :--- |
| www.pb.utfpr.tec.br | E2-DNS-PB | T | T |  |
| www.fb.utfpr.tec.br | E2-DNS-PB | T | T |  |
| www.dv.utfpr.tec.br | E2-DNS-PB | T | T |  |


#### HTTP e Conteúdo — Seção 6.5


| Verificação | Parcela | Resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| HTTP local | E2-HTTP-PB | Servidor responde no navegador; testar pelo IP se o domínio falhar | T |  |
| Página personalizada | E2-PAG-PB | Nome, RA e campus corretos exibidos na página | T |  |


**Endereço utilizado no navegador (domínio ou IP):** ____________________


### 2.3.FB. Testes Locais — Francisco Beltrão

**PC escolhido como origem:** ____________________  
**Nome/identificação do outro PC:** ____________________  
**Data do teste:** ____________________


#### Endereçamento Automático — Seção 6.2


| Verificação | Parcela | Resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| PC de teste: DHCPv4 selecionado | E2-D4-FB | Opção DHCP ativa | T |  |
| PC de teste: IPv4/máscara/gateway/DNS recebidos | E2-D4-FB | Faixa e parâmetros corretos da LAN; sem utilizar reservas nem endereço duplicado | T |  |
| PC de teste: Auto Config IPv6 selecionado | E2-D6-FB | Configuração automática ativa | T |  |
| PC de teste: IPv6/prefixo/gateway/DNS recebidos | E2-D6-FB | GUA do /64 correto; gateway por RA; DNS IPv6 pelo DHCPv6 stateless | T |  |
| Outro PC: DHCPv4 selecionado | E2-D4-FB | Opção DHCP ativa | T |  |
| Outro PC: IPv4/máscara/gateway/DNS recebidos | E2-D4-FB | Faixa e parâmetros corretos da LAN; sem utilizar reservas nem endereço duplicado | T |  |
| Outro PC: Auto Config IPv6 selecionado | E2-D6-FB | Configuração automática ativa | T |  |
| Outro PC: IPv6/prefixo/gateway/DNS recebidos | E2-D6-FB | GUA do /64 correto; gateway por RA; DNS IPv6 pelo DHCPv6 stateless | T |  |


#### Conectividade Local — Seção 6.3

Execute os pings a partir do PC escolhido. Todos os resultados desta tabela pertencem à mesma parcela de 0,40 ponto da LAN.


| Destino da Tarefa 2 | Parcela | IPv4 | IPv6 GUA | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| Outro PC da própria LAN | E2-C-FB | T | T |  |
| Interface LAN do roteador — gateway | E2-C-FB | T | T |  |
| SVI do switch | E2-C-FB | T | T |  |
| SRV-FB-DNS-DHCP | E2-C-FB | T | T |  |
| SRV-FB-WEB | E2-C-FB | T | T |  |


#### DNS — Seção 6.4

Servidor DNS consultado: ____________________. Cada resposta deverá corresponder ao endereço do Servidor Web previsto na Tarefa 2.


| Domínio | Parcela | A — estado | AAAA — estado | Respostas observadas/pendência |
| :--- | :--- | :--- | :--- | :--- |
| www.pb.utfpr.tec.br | E2-DNS-FB | T | T |  |
| www.fb.utfpr.tec.br | E2-DNS-FB | T | T |  |
| www.dv.utfpr.tec.br | E2-DNS-FB | T | T |  |


#### HTTP e Conteúdo — Seção 6.5


| Verificação | Parcela | Resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| HTTP local | E2-HTTP-FB | Servidor responde no navegador; testar pelo IP se o domínio falhar | T |  |
| Página personalizada | E2-PAG-FB | Nome, RA e campus corretos exibidos na página | T |  |


**Endereço utilizado no navegador (domínio ou IP):** ____________________


### 2.3.DV. Testes Locais — Dois Vizinhos

**PC escolhido como origem:** ____________________  
**Nome/identificação do outro PC:** ____________________  
**Data do teste:** ____________________


#### Endereçamento Automático — Seção 6.2


| Verificação | Parcela | Resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| PC de teste: DHCPv4 selecionado | E2-D4-DV | Opção DHCP ativa | T |  |
| PC de teste: IPv4/máscara/gateway/DNS recebidos | E2-D4-DV | Faixa e parâmetros corretos da LAN; sem utilizar reservas nem endereço duplicado | T |  |
| PC de teste: Auto Config IPv6 selecionado | E2-D6-DV | Configuração automática ativa | T |  |
| PC de teste: IPv6/prefixo/gateway/DNS recebidos | E2-D6-DV | GUA do /64 correto; gateway por RA; DNS IPv6 pelo DHCPv6 stateless | T |  |
| Outro PC: DHCPv4 selecionado | E2-D4-DV | Opção DHCP ativa | T |  |
| Outro PC: IPv4/máscara/gateway/DNS recebidos | E2-D4-DV | Faixa e parâmetros corretos da LAN; sem utilizar reservas nem endereço duplicado | T |  |
| Outro PC: Auto Config IPv6 selecionado | E2-D6-DV | Configuração automática ativa | T |  |
| Outro PC: IPv6/prefixo/gateway/DNS recebidos | E2-D6-DV | GUA do /64 correto; gateway por RA; DNS IPv6 pelo DHCPv6 stateless | T |  |


#### Conectividade Local — Seção 6.3

Execute os pings a partir do PC escolhido. Todos os resultados desta tabela pertencem à mesma parcela de 0,40 ponto da LAN.


| Destino da Tarefa 2 | Parcela | IPv4 | IPv6 GUA | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| Outro PC da própria LAN | E2-C-DV | T | T |  |
| Interface LAN do roteador — gateway | E2-C-DV | T | T |  |
| SVI do switch | E2-C-DV | T | T |  |
| SRV-DV-DNS-DHCP | E2-C-DV | T | T |  |
| SRV-DV-WEB | E2-C-DV | T | T |  |


#### DNS — Seção 6.4

Servidor DNS consultado: ____________________. Cada resposta deverá corresponder ao endereço do Servidor Web previsto na Tarefa 2.


| Domínio | Parcela | A — estado | AAAA — estado | Respostas observadas/pendência |
| :--- | :--- | :--- | :--- | :--- |
| www.pb.utfpr.tec.br | E2-DNS-DV | T | T |  |
| www.fb.utfpr.tec.br | E2-DNS-DV | T | T |  |
| www.dv.utfpr.tec.br | E2-DNS-DV | T | T |  |


#### HTTP e Conteúdo — Seção 6.5


| Verificação | Parcela | Resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| HTTP local | E2-HTTP-DV | Servidor responde no navegador; testar pelo IP se o domínio falhar | T |  |
| Página personalizada | E2-PAG-DV | Nome, RA e campus corretos exibidos na página | T |  |


**Endereço utilizado no navegador (domínio ou IP):** ____________________


### 2.4. Enlaces Diretos entre Roteadores — Seção 6.6

Teste o alcance entre as duas extremidades pelos endereços planejados. Cada linha vale 0,06 e exige sucesso nos dois protocolos.


| Enlace / ID da parcela | Origem e destino | IPv4 | IPv6 | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| pb-vit / E2-WAN-pb-vit | PB Se0/0/0 ↔ VIT Se0/0/1 | T | T |  |
| vit-fb / E2-WAN-vit-fb | VIT Se0/0/0 ↔ FB Se0/0/1 | T | T |  |
| fb-ita / E2-WAN-fb-ita | FB Se0/0/0 ↔ ITA Se0/0/1 | T | T |  |
| ita-pb / E2-WAN-ita-pb | ITA Se0/0/0 ↔ PB Se0/0/1 | T | T |  |
| ita-dv / E2-WAN-ita-dv | ITA Fa0/1 ↔ DV Fa0/1 | T | T |  |


### 2.5. Consolidação da Autoavaliação e Nota

Marque uma parcela como A somente após conferir todas as verificações vinculadas a ela. O professor preencherá a nota e os eventuais descontos.


| Parcela | Resultado avaliado | Valor máximo | Autoavaliação A/N/T | Nota verificada | Adicional por declaração incorreta |
| :--- | :--- | :--- | :--- | :--- | :--- |
| E2-C-PB | Pato Branco — Conectividade local IPv4 e IPv6 | 0,40 | T |  |  |
| E2-D4-PB | Pato Branco — DHCPv4 nos dois PCs | 0,20 | T |  |  |
| E2-D6-PB | Pato Branco — SLAAC/RA/DHCPv6 stateless nos dois PCs | 0,20 | T |  |  |
| E2-DNS-PB | Pato Branco — Resolução A e AAAA dos três domínios | 0,10 | T |  |  |
| E2-HTTP-PB | Pato Branco — HTTP local disponível | 0,10 | T |  |  |
| E2-PAG-PB | Pato Branco — Página personalizada correta | 0,20 ÷ 3 | T |  |  |
| E2-C-FB | Francisco Beltrão — Conectividade local IPv4 e IPv6 | 0,40 | T |  |  |
| E2-D4-FB | Francisco Beltrão — DHCPv4 nos dois PCs | 0,20 | T |  |  |
| E2-D6-FB | Francisco Beltrão — SLAAC/RA/DHCPv6 stateless nos dois PCs | 0,20 | T |  |  |
| E2-DNS-FB | Francisco Beltrão — Resolução A e AAAA dos três domínios | 0,10 | T |  |  |
| E2-HTTP-FB | Francisco Beltrão — HTTP local disponível | 0,10 | T |  |  |
| E2-PAG-FB | Francisco Beltrão — Página personalizada correta | 0,20 ÷ 3 | T |  |  |
| E2-C-DV | Dois Vizinhos — Conectividade local IPv4 e IPv6 | 0,40 | T |  |  |
| E2-D4-DV | Dois Vizinhos — DHCPv4 nos dois PCs | 0,20 | T |  |  |
| E2-D6-DV | Dois Vizinhos — SLAAC/RA/DHCPv6 stateless nos dois PCs | 0,20 | T |  |  |
| E2-DNS-DV | Dois Vizinhos — Resolução A e AAAA dos três domínios | 0,10 | T |  |  |
| E2-HTTP-DV | Dois Vizinhos — HTTP local disponível | 0,10 | T |  |  |
| E2-PAG-DV | Dois Vizinhos — Página personalizada correta | 0,20 ÷ 3 | T |  |  |
| E2-WAN-pb-vit | pb-vit — IPv4 e IPv6 entre vizinhos | 0,06 | T |  |  |
| E2-WAN-vit-fb | vit-fb — IPv4 e IPv6 entre vizinhos | 0,06 | T |  |  |
| E2-WAN-fb-ita | fb-ita — IPv4 e IPv6 entre vizinhos | 0,06 | T |  |  |
| E2-WAN-ita-pb | ita-pb — IPv4 e IPv6 entre vizinhos | 0,06 | T |  |  |
| E2-WAN-ita-dv | ita-dv — IPv4 e IPv6 entre vizinhos | 0,06 | T |  |  |


**Pontuação apurada nos resultados:** ______ / 3,50

**Desconto por DOC-T1 / DOC-T2 não corrigidas:** ______

**Descontos adicionais por declarações incorretas:** ______

**Nota final da Entrega 2 (mínimo zero):** ______ / 3,50

**Pendências reconhecidas e observações do aluno:** ____________________

**Observações do professor:** ____________________


## 3. Entrega 3 — Rede Cabeada Completa

Mantenha a documentação corrigida e confira novamente os requisitos da Entrega 2 na topologia atualizada. As parcelas antigas não recebem novos pontos. Utilize um PC de teste de cada LAN para a matriz abaixo, conforme a Seção 7.3.

### 3.1. Documentação das Rotas — Seção 7.1

Para cada roteador/protocolo, confira todas as rotas remotas necessárias, próximos saltos, interfaces, coerência com a implementação e o fluxo horário exigido. Cada célula de protocolo representa 0,05 ponto.

| Roteador | Parcela IPv4 | Estado IPv4 | Parcela IPv6 | Estado IPv6 | Pendências |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Pato Branco | E3-T4-PB | T | E3-T6-PB | T |  |
| Vitorino | E3-T4-VIT | T | E3-T6-VIT | T |  |
| Francisco Beltrão | E3-T4-FB | T | E3-T6-FB | T |  |
| Itapejara D’Oeste | E3-T4-ITA | T | E3-T6-ITA | T |  |
| Dois Vizinhos | E3-T4-DV | T | E3-T6-DV | T |  |


### 3.2.PB. Conectividade Completa — Origem em Pato Branco

**PC escolhido como origem:** ____________________  
**Qual PC desta LAN é a origem (PC1 ou PC2):** ____________________

Use os endereços da Tarefa 2. Marque o próprio PC de origem como **ORIGEM**; ele não é um destino de ping para si mesmo. Todos os demais destinos devem responder. As três matrizes completas determinam E3-R4 e E3-R6. Para testes IPv6 entre redes, utilize GUA.


| Destino/interface | IPv4 — E3-R4 | IPv6 — E3-R6 | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| Roteador PB — Fa0/0 | T | T |  |
| Roteador PB — Se0/0/0 | T | T |  |
| Roteador PB — Se0/0/1 | T | T |  |
| Roteador FB — Fa0/0 | T | T |  |
| Roteador FB — Se0/0/0 | T | T |  |
| Roteador FB — Se0/0/1 | T | T |  |
| Roteador VIT — Se0/0/0 | T | T |  |
| Roteador VIT — Se0/0/1 | T | T |  |
| Roteador ITA — Se0/0/0 | T | T |  |
| Roteador ITA — Se0/0/1 | T | T |  |
| Roteador ITA — Fa0/1 | T | T |  |
| Roteador DV — Fa0/0 | T | T |  |
| Roteador DV — Fa0/1 | T | T |  |
| Switch PB — SVI | T | T |  |
| Switch FB — SVI | T | T |  |
| Switch DV — SVI | T | T |  |
| SRV-PB-DNS-DHCP | T | T |  |
| SRV-PB-WEB | T | T |  |
| SRV-FB-DNS-DHCP | T | T |  |
| SRV-FB-WEB | T | T |  |
| SRV-DV-DNS-DHCP | T | T |  |
| SRV-DV-WEB | T | T |  |
| PC1-PB | T | T |  |
| PC2-PB | T | T |  |
| PC1-FB | T | T |  |
| PC2-FB | T | T |  |
| PC1-DV | T | T |  |
| PC2-DV | T | T |  |


| Verificação complementar | Estado | Observações |
| :--- | :--- | :--- |
| Rotas documentadas e implementadas respeitam o sentido horário e os caminhos exigidos | T |  |
| Os três domínios resolvem e as páginas dos outros campi são acessíveis; se o DNS falhar, HTTP conferido por IP | T |  |


### 3.2.FB. Conectividade Completa — Origem em Francisco Beltrão

**PC escolhido como origem:** ____________________  
**Qual PC desta LAN é a origem (PC1 ou PC2):** ____________________

Use os endereços da Tarefa 2. Marque o próprio PC de origem como **ORIGEM**; ele não é um destino de ping para si mesmo. Todos os demais destinos devem responder. As três matrizes completas determinam E3-R4 e E3-R6. Para testes IPv6 entre redes, utilize GUA.


| Destino/interface | IPv4 — E3-R4 | IPv6 — E3-R6 | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| Roteador PB — Fa0/0 | T | T |  |
| Roteador PB — Se0/0/0 | T | T |  |
| Roteador PB — Se0/0/1 | T | T |  |
| Roteador FB — Fa0/0 | T | T |  |
| Roteador FB — Se0/0/0 | T | T |  |
| Roteador FB — Se0/0/1 | T | T |  |
| Roteador VIT — Se0/0/0 | T | T |  |
| Roteador VIT — Se0/0/1 | T | T |  |
| Roteador ITA — Se0/0/0 | T | T |  |
| Roteador ITA — Se0/0/1 | T | T |  |
| Roteador ITA — Fa0/1 | T | T |  |
| Roteador DV — Fa0/0 | T | T |  |
| Roteador DV — Fa0/1 | T | T |  |
| Switch PB — SVI | T | T |  |
| Switch FB — SVI | T | T |  |
| Switch DV — SVI | T | T |  |
| SRV-PB-DNS-DHCP | T | T |  |
| SRV-PB-WEB | T | T |  |
| SRV-FB-DNS-DHCP | T | T |  |
| SRV-FB-WEB | T | T |  |
| SRV-DV-DNS-DHCP | T | T |  |
| SRV-DV-WEB | T | T |  |
| PC1-PB | T | T |  |
| PC2-PB | T | T |  |
| PC1-FB | T | T |  |
| PC2-FB | T | T |  |
| PC1-DV | T | T |  |
| PC2-DV | T | T |  |


| Verificação complementar | Estado | Observações |
| :--- | :--- | :--- |
| Rotas documentadas e implementadas respeitam o sentido horário e os caminhos exigidos | T |  |
| Os três domínios resolvem e as páginas dos outros campi são acessíveis; se o DNS falhar, HTTP conferido por IP | T |  |


### 3.2.DV. Conectividade Completa — Origem em Dois Vizinhos

**PC escolhido como origem:** ____________________  
**Qual PC desta LAN é a origem (PC1 ou PC2):** ____________________

Use os endereços da Tarefa 2. Marque o próprio PC de origem como **ORIGEM**; ele não é um destino de ping para si mesmo. Todos os demais destinos devem responder. As três matrizes completas determinam E3-R4 e E3-R6. Para testes IPv6 entre redes, utilize GUA.


| Destino/interface | IPv4 — E3-R4 | IPv6 — E3-R6 | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| Roteador PB — Fa0/0 | T | T |  |
| Roteador PB — Se0/0/0 | T | T |  |
| Roteador PB — Se0/0/1 | T | T |  |
| Roteador FB — Fa0/0 | T | T |  |
| Roteador FB — Se0/0/0 | T | T |  |
| Roteador FB — Se0/0/1 | T | T |  |
| Roteador VIT — Se0/0/0 | T | T |  |
| Roteador VIT — Se0/0/1 | T | T |  |
| Roteador ITA — Se0/0/0 | T | T |  |
| Roteador ITA — Se0/0/1 | T | T |  |
| Roteador ITA — Fa0/1 | T | T |  |
| Roteador DV — Fa0/0 | T | T |  |
| Roteador DV — Fa0/1 | T | T |  |
| Switch PB — SVI | T | T |  |
| Switch FB — SVI | T | T |  |
| Switch DV — SVI | T | T |  |
| SRV-PB-DNS-DHCP | T | T |  |
| SRV-PB-WEB | T | T |  |
| SRV-FB-DNS-DHCP | T | T |  |
| SRV-FB-WEB | T | T |  |
| SRV-DV-DNS-DHCP | T | T |  |
| SRV-DV-WEB | T | T |  |
| PC1-PB | T | T |  |
| PC2-PB | T | T |  |
| PC1-FB | T | T |  |
| PC2-FB | T | T |  |
| PC1-DV | T | T |  |
| PC2-DV | T | T |  |


| Verificação complementar | Estado | Observações |
| :--- | :--- | :--- |
| Rotas documentadas e implementadas respeitam o sentido horário e os caminhos exigidos | T |  |
| Os três domínios resolvem e as páginas dos outros campi são acessíveis; se o DNS falhar, HTTP conferido por IP | T |  |


**Regra global por protocolo:** E3-R4 recebe 1,00 ou zero; E3-R6 recebe 1,00 ou zero. Uma falha persistente em qualquer destino exigido de qualquer origem implica zero naquele protocolo. A avaliação dos dois protocolos é independente.

### 3.3. Segurança e SSH — Tarefa 8

Execute os testes em todos os cinco roteadores. Cada requisito tem sua parcela por roteador: 0,02 nos itens S1 a S6 e 0,08 no item S7.

#### Pato Branco


| Parcela | Teste/resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| E3-S1-PB | Acesso exibe o MOTD personalizado conforme o enunciado | T |  |
| E3-S2-PB | Mínimo de 10 caracteres exigido e senhas em texto simples protegidas conforme a Tarefa 8 | T |  |
| E3-S3-PB | Entrada no EXEC privilegiado exige a senha secreta personalizada | T |  |
| E3-S4-PB | Console exige a senha personalizada | T |  |
| E3-S5-PB | Sessões de console e SSH encerram após mais de 5 minutos sem atividade | T |  |
| E3-S6-PB | Três falhas SSH em 60 s causam bloqueio por 120 s; estado conferido com show login | T |  |
| E3-S7-PB | SSH remoto autentica o usuário local correto; VTY aceita somente SSH; domínio, usuário, senha, RSA 1024 e VTY 0–15 conforme a Seção 8.2 | T |  |


#### Vitorino


| Parcela | Teste/resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| E3-S1-VIT | Acesso exibe o MOTD personalizado conforme o enunciado | T |  |
| E3-S2-VIT | Mínimo de 10 caracteres exigido e senhas em texto simples protegidas conforme a Tarefa 8 | T |  |
| E3-S3-VIT | Entrada no EXEC privilegiado exige a senha secreta personalizada | T |  |
| E3-S4-VIT | Console exige a senha personalizada | T |  |
| E3-S5-VIT | Sessões de console e SSH encerram após mais de 5 minutos sem atividade | T |  |
| E3-S6-VIT | Três falhas SSH em 60 s causam bloqueio por 120 s; estado conferido com show login | T |  |
| E3-S7-VIT | SSH remoto autentica o usuário local correto; VTY aceita somente SSH; domínio, usuário, senha, RSA 1024 e VTY 0–15 conforme a Seção 8.2 | T |  |


#### Francisco Beltrão


| Parcela | Teste/resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| E3-S1-FB | Acesso exibe o MOTD personalizado conforme o enunciado | T |  |
| E3-S2-FB | Mínimo de 10 caracteres exigido e senhas em texto simples protegidas conforme a Tarefa 8 | T |  |
| E3-S3-FB | Entrada no EXEC privilegiado exige a senha secreta personalizada | T |  |
| E3-S4-FB | Console exige a senha personalizada | T |  |
| E3-S5-FB | Sessões de console e SSH encerram após mais de 5 minutos sem atividade | T |  |
| E3-S6-FB | Três falhas SSH em 60 s causam bloqueio por 120 s; estado conferido com show login | T |  |
| E3-S7-FB | SSH remoto autentica o usuário local correto; VTY aceita somente SSH; domínio, usuário, senha, RSA 1024 e VTY 0–15 conforme a Seção 8.2 | T |  |


#### Itapejara D’Oeste


| Parcela | Teste/resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| E3-S1-ITA | Acesso exibe o MOTD personalizado conforme o enunciado | T |  |
| E3-S2-ITA | Mínimo de 10 caracteres exigido e senhas em texto simples protegidas conforme a Tarefa 8 | T |  |
| E3-S3-ITA | Entrada no EXEC privilegiado exige a senha secreta personalizada | T |  |
| E3-S4-ITA | Console exige a senha personalizada | T |  |
| E3-S5-ITA | Sessões de console e SSH encerram após mais de 5 minutos sem atividade | T |  |
| E3-S6-ITA | Três falhas SSH em 60 s causam bloqueio por 120 s; estado conferido com show login | T |  |
| E3-S7-ITA | SSH remoto autentica o usuário local correto; VTY aceita somente SSH; domínio, usuário, senha, RSA 1024 e VTY 0–15 conforme a Seção 8.2 | T |  |


#### Dois Vizinhos


| Parcela | Teste/resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| E3-S1-DV | Acesso exibe o MOTD personalizado conforme o enunciado | T |  |
| E3-S2-DV | Mínimo de 10 caracteres exigido e senhas em texto simples protegidas conforme a Tarefa 8 | T |  |
| E3-S3-DV | Entrada no EXEC privilegiado exige a senha secreta personalizada | T |  |
| E3-S4-DV | Console exige a senha personalizada | T |  |
| E3-S5-DV | Sessões de console e SSH encerram após mais de 5 minutos sem atividade | T |  |
| E3-S6-DV | Três falhas SSH em 60 s causam bloqueio por 120 s; estado conferido com show login | T |  |
| E3-S7-DV | SSH remoto autentica o usuário local correto; VTY aceita somente SSH; domínio, usuário, senha, RSA 1024 e VTY 0–15 conforme a Seção 8.2 | T |  |


### 3.4. Consolidação da Autoavaliação e Nota


| Parcela | Resultado avaliado | Valor máximo | Autoavaliação A/N/T | Nota verificada | Adicional por declaração incorreta |
| :--- | :--- | :--- | :--- | :--- | :--- |
| E3-T4-PB | Pato Branco — tabela de rotas IPv4 | 0,05 | T |  |  |
| E3-T6-PB | Pato Branco — tabela de rotas IPv6 | 0,05 | T |  |  |
| E3-T4-VIT | Vitorino — tabela de rotas IPv4 | 0,05 | T |  |  |
| E3-T6-VIT | Vitorino — tabela de rotas IPv6 | 0,05 | T |  |  |
| E3-T4-FB | Francisco Beltrão — tabela de rotas IPv4 | 0,05 | T |  |  |
| E3-T6-FB | Francisco Beltrão — tabela de rotas IPv6 | 0,05 | T |  |  |
| E3-T4-ITA | Itapejara D’Oeste — tabela de rotas IPv4 | 0,05 | T |  |  |
| E3-T6-ITA | Itapejara D’Oeste — tabela de rotas IPv6 | 0,05 | T |  |  |
| E3-T4-DV | Dois Vizinhos — tabela de rotas IPv4 | 0,05 | T |  |  |
| E3-T6-DV | Dois Vizinhos — tabela de rotas IPv6 | 0,05 | T |  |  |
| E3-R4 | Conectividade IPv4 completa e fluxo exigido | 1,00 | T |  |  |
| E3-R6 | Conectividade IPv6 completa e fluxo exigido | 1,00 | T |  |  |
| E3-S1-PB | Pato Branco — Banner correto exibido | 0,02 | T |  |  |
| E3-S2-PB | Pato Branco — Mínimo de 10 caracteres e proteção das senhas | 0,02 | T |  |  |
| E3-S3-PB | Pato Branco — Senha secreta do EXEC privilegiado | 0,02 | T |  |  |
| E3-S4-PB | Pato Branco — Senha do console | 0,02 | T |  |  |
| E3-S5-PB | Pato Branco — Console/SSH encerrados após 5 min sem atividade | 0,02 | T |  |  |
| E3-S6-PB | Pato Branco — Bloqueio 120 s após 3 falhas em 60 s | 0,02 | T |  |  |
| E3-S7-PB | Pato Branco — SSH remoto/autenticação local/VTY somente SSH | 0,08 | T |  |  |
| E3-S1-VIT | Vitorino — Banner correto exibido | 0,02 | T |  |  |
| E3-S2-VIT | Vitorino — Mínimo de 10 caracteres e proteção das senhas | 0,02 | T |  |  |
| E3-S3-VIT | Vitorino — Senha secreta do EXEC privilegiado | 0,02 | T |  |  |
| E3-S4-VIT | Vitorino — Senha do console | 0,02 | T |  |  |
| E3-S5-VIT | Vitorino — Console/SSH encerrados após 5 min sem atividade | 0,02 | T |  |  |
| E3-S6-VIT | Vitorino — Bloqueio 120 s após 3 falhas em 60 s | 0,02 | T |  |  |
| E3-S7-VIT | Vitorino — SSH remoto/autenticação local/VTY somente SSH | 0,08 | T |  |  |
| E3-S1-FB | Francisco Beltrão — Banner correto exibido | 0,02 | T |  |  |
| E3-S2-FB | Francisco Beltrão — Mínimo de 10 caracteres e proteção das senhas | 0,02 | T |  |  |
| E3-S3-FB | Francisco Beltrão — Senha secreta do EXEC privilegiado | 0,02 | T |  |  |
| E3-S4-FB | Francisco Beltrão — Senha do console | 0,02 | T |  |  |
| E3-S5-FB | Francisco Beltrão — Console/SSH encerrados após 5 min sem atividade | 0,02 | T |  |  |
| E3-S6-FB | Francisco Beltrão — Bloqueio 120 s após 3 falhas em 60 s | 0,02 | T |  |  |
| E3-S7-FB | Francisco Beltrão — SSH remoto/autenticação local/VTY somente SSH | 0,08 | T |  |  |
| E3-S1-ITA | Itapejara D’Oeste — Banner correto exibido | 0,02 | T |  |  |
| E3-S2-ITA | Itapejara D’Oeste — Mínimo de 10 caracteres e proteção das senhas | 0,02 | T |  |  |
| E3-S3-ITA | Itapejara D’Oeste — Senha secreta do EXEC privilegiado | 0,02 | T |  |  |
| E3-S4-ITA | Itapejara D’Oeste — Senha do console | 0,02 | T |  |  |
| E3-S5-ITA | Itapejara D’Oeste — Console/SSH encerrados após 5 min sem atividade | 0,02 | T |  |  |
| E3-S6-ITA | Itapejara D’Oeste — Bloqueio 120 s após 3 falhas em 60 s | 0,02 | T |  |  |
| E3-S7-ITA | Itapejara D’Oeste — SSH remoto/autenticação local/VTY somente SSH | 0,08 | T |  |  |
| E3-S1-DV | Dois Vizinhos — Banner correto exibido | 0,02 | T |  |  |
| E3-S2-DV | Dois Vizinhos — Mínimo de 10 caracteres e proteção das senhas | 0,02 | T |  |  |
| E3-S3-DV | Dois Vizinhos — Senha secreta do EXEC privilegiado | 0,02 | T |  |  |
| E3-S4-DV | Dois Vizinhos — Senha do console | 0,02 | T |  |  |
| E3-S5-DV | Dois Vizinhos — Console/SSH encerrados após 5 min sem atividade | 0,02 | T |  |  |
| E3-S6-DV | Dois Vizinhos — Bloqueio 120 s após 3 falhas em 60 s | 0,02 | T |  |  |
| E3-S7-DV | Dois Vizinhos — SSH remoto/autenticação local/VTY somente SSH | 0,08 | T |  |  |


**Pontuação apurada nos resultados:** ______ / 3,50

**Descontos adicionais por declarações incorretas:** ______

**Nota final da Entrega 3 (mínimo zero):** ______ / 3,50

**Pendências reconhecidas e observações do aluno:** ____________________

**Observações do professor:** ____________________


## 4. Entrega 4 — Integração Wi-Fi

Confira novamente os requisitos das Entregas 2 e 3 na topologia final. Mantenha os registros anteriores e atualize as pendências. Em cada LAN, execute a Seção 9.4 a partir do notebook do campus.

### 4.1.PB. Testes Wi-Fi — Pato Branco

**AP:** ____________________  
**Modelo:** ____________________  
**Notebook de origem:** ____________________  
**Data da verificação:** ____________________


| Parcela | Verificação | Resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| E4-AP-PB | Conexão ao switch | Cabo Ethernet na porta LAN Gi1 do AP; porta Internet/WAN sem conexão | T |  |
| E4-AP-PB | Gerenciamento | Endereço IPv4 planejado acessível; parâmetros IPv6 aplicados quando disponíveis, com limitações registradas | T |  |
| E4-AP-PB | Integração aos serviços da LAN | DHCP/RA próprios do AP desativados quando disponíveis; clientes usam os serviços e gateway do campus | T |  |
| E4-ASS-PB | SSID/segurança | Notebook associa ao SSID do campus com WPA2-PSK/AES e senha válida de no mínimo 10 caracteres | T |  |
| E4-ASS-PB | Senha incorreta | Associação recusada com senha incorreta; ao concluir, restaurada a senha válida | T |  |
| E4-AUTO-PB | IPv4 automático | Notebook recebe IP/máscara/gateway/DNS corretos por DHCPv4, na mesma sub-rede dos PCs | T |  |
| E4-AUTO-PB | IPv6 automático | GUA/prefixo por SLAAC, gateway por RA e DNS por DHCPv6 stateless, conforme o campus | T |  |
| E4-DOC-PB | Documentação Wi-Fi | Modelo, identificação, portas, SSID, segurança, senha, DHCP, endereços e limitações registrados e coerentes com a implementação | T |  |
| E4-DOC-PB | Documentação cumulativa | Tarefas 1 e 2 corrigidas, Seção 7.1 e scripts atualizados preservados; resultados no checklist final | T |  |


#### Conectividade Local e Remota — E4-CON-PB

Todos os destinos abaixo deverão responder em IPv4 e IPv6. Mantenha a rede cabeada funcional.


| Destino/interface | IPv4 | IPv6 GUA | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| Roteador PB — Fa0/0 | T | T |  |
| Roteador PB — Se0/0/0 | T | T |  |
| Roteador PB — Se0/0/1 | T | T |  |
| Roteador FB — Fa0/0 | T | T |  |
| Roteador FB — Se0/0/0 | T | T |  |
| Roteador FB — Se0/0/1 | T | T |  |
| Roteador VIT — Se0/0/0 | T | T |  |
| Roteador VIT — Se0/0/1 | T | T |  |
| Roteador ITA — Se0/0/0 | T | T |  |
| Roteador ITA — Se0/0/1 | T | T |  |
| Roteador ITA — Fa0/1 | T | T |  |
| Roteador DV — Fa0/0 | T | T |  |
| Roteador DV — Fa0/1 | T | T |  |
| Switch PB — SVI | T | T |  |
| Switch FB — SVI | T | T |  |
| Switch DV — SVI | T | T |  |
| SRV-PB-DNS-DHCP | T | T |  |
| SRV-PB-WEB | T | T |  |
| SRV-FB-DNS-DHCP | T | T |  |
| SRV-FB-WEB | T | T |  |
| SRV-DV-DNS-DHCP | T | T |  |
| SRV-DV-WEB | T | T |  |
| PC1-PB | T | T |  |
| PC2-PB | T | T |  |
| PC1-FB | T | T |  |
| PC2-FB | T | T |  |
| PC1-DV | T | T |  |
| PC2-DV | T | T |  |
| Notebook FB | T | T |  |
| Notebook DV | T | T |  |


#### DNS e Web — E4-DNS-PB / E4-WEB-PB

Consulte o DNS da LAN. As respostas A/AAAA devem corresponder à Tarefa 2. Acesse as três páginas pelo nome; se o DNS falhar, teste HTTP pelo IP para registrar o serviço separadamente. O resultado Web inclui a página personalizada correta.


| Domínio/campus | A — E4-DNS | AAAA — E4-DNS | HTTP/página — E4-WEB | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| www.pb.utfpr.tec.br | T | T | T |  |
| www.fb.utfpr.tec.br | T | T | T |  |
| www.dv.utfpr.tec.br | T | T | T |  |


### 4.1.FB. Testes Wi-Fi — Francisco Beltrão

**AP:** ____________________  
**Modelo:** ____________________  
**Notebook de origem:** ____________________  
**Data da verificação:** ____________________


| Parcela | Verificação | Resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| E4-AP-FB | Conexão ao switch | Cabo Ethernet na porta LAN Gi1 do AP; porta Internet/WAN sem conexão | T |  |
| E4-AP-FB | Gerenciamento | Endereço IPv4 planejado acessível; parâmetros IPv6 aplicados quando disponíveis, com limitações registradas | T |  |
| E4-AP-FB | Integração aos serviços da LAN | DHCP/RA próprios do AP desativados quando disponíveis; clientes usam os serviços e gateway do campus | T |  |
| E4-ASS-FB | SSID/segurança | Notebook associa ao SSID do campus com WPA2-PSK/AES e senha válida de no mínimo 10 caracteres | T |  |
| E4-ASS-FB | Senha incorreta | Associação recusada com senha incorreta; ao concluir, restaurada a senha válida | T |  |
| E4-AUTO-FB | IPv4 automático | Notebook recebe IP/máscara/gateway/DNS corretos por DHCPv4, na mesma sub-rede dos PCs | T |  |
| E4-AUTO-FB | IPv6 automático | GUA/prefixo por SLAAC, gateway por RA e DNS por DHCPv6 stateless, conforme o campus | T |  |
| E4-DOC-FB | Documentação Wi-Fi | Modelo, identificação, portas, SSID, segurança, senha, DHCP, endereços e limitações registrados e coerentes com a implementação | T |  |
| E4-DOC-FB | Documentação cumulativa | Tarefas 1 e 2 corrigidas, Seção 7.1 e scripts atualizados preservados; resultados no checklist final | T |  |


#### Conectividade Local e Remota — E4-CON-FB

Todos os destinos abaixo deverão responder em IPv4 e IPv6. Mantenha a rede cabeada funcional.


| Destino/interface | IPv4 | IPv6 GUA | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| Roteador PB — Fa0/0 | T | T |  |
| Roteador PB — Se0/0/0 | T | T |  |
| Roteador PB — Se0/0/1 | T | T |  |
| Roteador FB — Fa0/0 | T | T |  |
| Roteador FB — Se0/0/0 | T | T |  |
| Roteador FB — Se0/0/1 | T | T |  |
| Roteador VIT — Se0/0/0 | T | T |  |
| Roteador VIT — Se0/0/1 | T | T |  |
| Roteador ITA — Se0/0/0 | T | T |  |
| Roteador ITA — Se0/0/1 | T | T |  |
| Roteador ITA — Fa0/1 | T | T |  |
| Roteador DV — Fa0/0 | T | T |  |
| Roteador DV — Fa0/1 | T | T |  |
| Switch PB — SVI | T | T |  |
| Switch FB — SVI | T | T |  |
| Switch DV — SVI | T | T |  |
| SRV-PB-DNS-DHCP | T | T |  |
| SRV-PB-WEB | T | T |  |
| SRV-FB-DNS-DHCP | T | T |  |
| SRV-FB-WEB | T | T |  |
| SRV-DV-DNS-DHCP | T | T |  |
| SRV-DV-WEB | T | T |  |
| PC1-PB | T | T |  |
| PC2-PB | T | T |  |
| PC1-FB | T | T |  |
| PC2-FB | T | T |  |
| PC1-DV | T | T |  |
| PC2-DV | T | T |  |
| Notebook PB | T | T |  |
| Notebook DV | T | T |  |


#### DNS e Web — E4-DNS-FB / E4-WEB-FB

Consulte o DNS da LAN. As respostas A/AAAA devem corresponder à Tarefa 2. Acesse as três páginas pelo nome; se o DNS falhar, teste HTTP pelo IP para registrar o serviço separadamente. O resultado Web inclui a página personalizada correta.


| Domínio/campus | A — E4-DNS | AAAA — E4-DNS | HTTP/página — E4-WEB | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| www.pb.utfpr.tec.br | T | T | T |  |
| www.fb.utfpr.tec.br | T | T | T |  |
| www.dv.utfpr.tec.br | T | T | T |  |


### 4.1.DV. Testes Wi-Fi — Dois Vizinhos

**AP:** ____________________  
**Modelo:** ____________________  
**Notebook de origem:** ____________________  
**Data da verificação:** ____________________


| Parcela | Verificação | Resultado esperado | Estado | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| E4-AP-DV | Conexão ao switch | Cabo Ethernet na porta LAN Gi1 do AP; porta Internet/WAN sem conexão | T |  |
| E4-AP-DV | Gerenciamento | Endereço IPv4 planejado acessível; parâmetros IPv6 aplicados quando disponíveis, com limitações registradas | T |  |
| E4-AP-DV | Integração aos serviços da LAN | DHCP/RA próprios do AP desativados quando disponíveis; clientes usam os serviços e gateway do campus | T |  |
| E4-ASS-DV | SSID/segurança | Notebook associa ao SSID do campus com WPA2-PSK/AES e senha válida de no mínimo 10 caracteres | T |  |
| E4-ASS-DV | Senha incorreta | Associação recusada com senha incorreta; ao concluir, restaurada a senha válida | T |  |
| E4-AUTO-DV | IPv4 automático | Notebook recebe IP/máscara/gateway/DNS corretos por DHCPv4, na mesma sub-rede dos PCs | T |  |
| E4-AUTO-DV | IPv6 automático | GUA/prefixo por SLAAC, gateway por RA e DNS por DHCPv6 stateless, conforme o campus | T |  |
| E4-DOC-DV | Documentação Wi-Fi | Modelo, identificação, portas, SSID, segurança, senha, DHCP, endereços e limitações registrados e coerentes com a implementação | T |  |
| E4-DOC-DV | Documentação cumulativa | Tarefas 1 e 2 corrigidas, Seção 7.1 e scripts atualizados preservados; resultados no checklist final | T |  |


#### Conectividade Local e Remota — E4-CON-DV

Todos os destinos abaixo deverão responder em IPv4 e IPv6. Mantenha a rede cabeada funcional.


| Destino/interface | IPv4 | IPv6 GUA | Resultado observado/pendência |
| :--- | :--- | :--- | :--- |
| Roteador PB — Fa0/0 | T | T |  |
| Roteador PB — Se0/0/0 | T | T |  |
| Roteador PB — Se0/0/1 | T | T |  |
| Roteador FB — Fa0/0 | T | T |  |
| Roteador FB — Se0/0/0 | T | T |  |
| Roteador FB — Se0/0/1 | T | T |  |
| Roteador VIT — Se0/0/0 | T | T |  |
| Roteador VIT — Se0/0/1 | T | T |  |
| Roteador ITA — Se0/0/0 | T | T |  |
| Roteador ITA — Se0/0/1 | T | T |  |
| Roteador ITA — Fa0/1 | T | T |  |
| Roteador DV — Fa0/0 | T | T |  |
| Roteador DV — Fa0/1 | T | T |  |
| Switch PB — SVI | T | T |  |
| Switch FB — SVI | T | T |  |
| Switch DV — SVI | T | T |  |
| SRV-PB-DNS-DHCP | T | T |  |
| SRV-PB-WEB | T | T |  |
| SRV-FB-DNS-DHCP | T | T |  |
| SRV-FB-WEB | T | T |  |
| SRV-DV-DNS-DHCP | T | T |  |
| SRV-DV-WEB | T | T |  |
| PC1-PB | T | T |  |
| PC2-PB | T | T |  |
| PC1-FB | T | T |  |
| PC2-FB | T | T |  |
| PC1-DV | T | T |  |
| PC2-DV | T | T |  |
| Notebook PB | T | T |  |
| Notebook FB | T | T |  |


#### DNS e Web — E4-DNS-DV / E4-WEB-DV

Consulte o DNS da LAN. As respostas A/AAAA devem corresponder à Tarefa 2. Acesse as três páginas pelo nome; se o DNS falhar, teste HTTP pelo IP para registrar o serviço separadamente. O resultado Web inclui a página personalizada correta.


| Domínio/campus | A — E4-DNS | AAAA — E4-DNS | HTTP/página — E4-WEB | Resultado observado/pendência |
| :--- | :--- | :--- | :--- | :--- |
| www.pb.utfpr.tec.br | T | T | T |  |
| www.fb.utfpr.tec.br | T | T | T |  |
| www.dv.utfpr.tec.br | T | T | T |  |


### 4.2. Consolidação da Autoavaliação e Nota


| Parcela | Resultado avaliado | Valor máximo | Autoavaliação A/N/T | Nota verificada | Adicional por declaração incorreta |
| :--- | :--- | :--- | :--- | :--- | :--- |
| E4-AP-PB | Pato Branco — Integração e gerenciamento do AP | 0,40 ÷ 3 | T |  |  |
| E4-ASS-PB | Pato Branco — Associação e segurança Wi-Fi | 0,40 ÷ 3 | T |  |  |
| E4-AUTO-PB | Pato Branco — Endereçamento automático do notebook | 0,40 ÷ 3 | T |  |  |
| E4-CON-PB | Pato Branco — Conectividade local/remota IPv4 e IPv6 | 0,40 ÷ 3 | T |  |  |
| E4-DNS-PB | Pato Branco — DNS dos três domínios | 0,05 | T |  |  |
| E4-WEB-PB | Pato Branco — HTTP e páginas dos três campi | 0,05 | T |  |  |
| E4-DOC-PB | Pato Branco — Documentação Wi-Fi coerente | 0,10 ÷ 3 | T |  |  |
| E4-AP-FB | Francisco Beltrão — Integração e gerenciamento do AP | 0,40 ÷ 3 | T |  |  |
| E4-ASS-FB | Francisco Beltrão — Associação e segurança Wi-Fi | 0,40 ÷ 3 | T |  |  |
| E4-AUTO-FB | Francisco Beltrão — Endereçamento automático do notebook | 0,40 ÷ 3 | T |  |  |
| E4-CON-FB | Francisco Beltrão — Conectividade local/remota IPv4 e IPv6 | 0,40 ÷ 3 | T |  |  |
| E4-DNS-FB | Francisco Beltrão — DNS dos três domínios | 0,05 | T |  |  |
| E4-WEB-FB | Francisco Beltrão — HTTP e páginas dos três campi | 0,05 | T |  |  |
| E4-DOC-FB | Francisco Beltrão — Documentação Wi-Fi coerente | 0,10 ÷ 3 | T |  |  |
| E4-AP-DV | Dois Vizinhos — Integração e gerenciamento do AP | 0,40 ÷ 3 | T |  |  |
| E4-ASS-DV | Dois Vizinhos — Associação e segurança Wi-Fi | 0,40 ÷ 3 | T |  |  |
| E4-AUTO-DV | Dois Vizinhos — Endereçamento automático do notebook | 0,40 ÷ 3 | T |  |  |
| E4-CON-DV | Dois Vizinhos — Conectividade local/remota IPv4 e IPv6 | 0,40 ÷ 3 | T |  |  |
| E4-DNS-DV | Dois Vizinhos — DNS dos três domínios | 0,05 | T |  |  |
| E4-WEB-DV | Dois Vizinhos — HTTP e páginas dos três campi | 0,05 | T |  |  |
| E4-DOC-DV | Dois Vizinhos — Documentação Wi-Fi coerente | 0,10 ÷ 3 | T |  |  |


**Pontuação apurada nos resultados:** ______ / 2,00

**Descontos adicionais por declarações incorretas:** ______

**Nota final da Entrega 4 (mínimo zero):** ______ / 2,00

**Pendências reconhecidas e observações do aluno:** ____________________

**Observações do professor:** ____________________


## 5. Conferência dos Arquivos e Declaração Final

| Verificação | Estado | Observações |
| :--- | :--- | :--- |
| Nome, RA e curso no documento; nome e RA na topologia | T | |
| Documentação cumulativa da etapa correta e coerente com o `.pkt` | T | |
| Um script `.txt` por roteador/switch, atualizado e nomeado pelo hostname | T | |
| Checklist da etapa preenchido, salvo com o nome exigido | T | |
| Topologia salva e versão entregue identificada no cabeçalho deste checklist | T | |
| Arquivos exigidos no ZIP enviado pelo Moodle ou no mesmo repositório individual já informado | T | |
| Envio no Moodle ou commits concluídos dentro do prazo da etapa | T | |
| Todas as pendências ainda existentes registradas, sem marcar A em itens não testados | T | |

**Declaração do aluno:** os resultados registrados correspondem às verificações que realizei na versão `.pkt` entregue. Conheço as regras de avaliação, os descontos por declarações incorretas e as orientações de autoria e uso de IA do enunciado.

**Nome / data:** ____________________

**Registro do professor — notas finais:** Entrega 1: ____ / 1,00; Entrega 2: ____ / 3,50; Entrega 3: ____ / 3,50; Entrega 4: ____ / 2,00. **Total: ____ / 10,00.**