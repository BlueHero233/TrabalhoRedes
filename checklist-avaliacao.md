# Checklist de Avaliação — Trabalho de Redes de Computadores — 2026/2

**Cursos:** Engenharia de Computação / Engenharia Elétrica / Tecnologia em Análise e Desenvolvimento de Sistemas

**Aluno:** ____________________

**RA:** ____________________

**Curso:** ____________________

**Professor / data da avaliação:** ____________________

Esta checklist acompanha o [enunciado](README.md) e o [modelo de documentação](trabalho-documentacao-modelo.md). O aluno pode utilizá-la para conferir o trabalho antes das entregas. O professor utilizará os mesmos critérios para registrar a nota.

**Aluno:** substitua ☐ por ☑ após conferir o critério. **Professor:** registre a pontuação obtida na coluna Nota e utilize o campo de observações para indicar pendências. As marcas do aluno representam sua conferência; a pontuação será atribuída na avaliação.

Os valores são totais para o **conjunto das três LANs**, quando aplicável. Verifique cada critério em Pato Branco, Francisco Beltrão e Dois Vizinhos.

## Resumo da Pontuação

| Entrega | Prazo | Valor máximo | Nota obtida |
| :--- | :--- | ---: | :---: |
| **1 — Tarefas 1 e 2** | 20/10/2026 | 1,00 | |
| **2 — Correções e Tarefa 3** | 27/10/2026 | 0,50 | |
| **3 — Rede cabeada** | 10/11/2026 | 7,50 | |
| **4 — Final com Wi-Fi** | A definir após a aula sobre Wi-Fi | 1,00 | |
| **Total** | | **10,00** | |

## Entrega 1 — Planejamento

**Os endereços dos futuros APs devem estar calculados e documentados nesta entrega.** Os parâmetros SSID, senha e demais configurações Wi-Fi serão documentados na Entrega 4.

| Aluno conferiu | Item | Critério de avaliação | Valor máximo | Nota |
| :---: | :---: | :--- | ---: | :---: |
| ☐ | 1.1 | Sub-redes IPv4/IPv6 corretas, com prefixos, blocos LAN/WAN e reservas para expansão conforme a Tarefa 1. | 0,50 | |
| ☐ | 1.2 | Endereçamento completo dos dispositivos, incluindo os futuros APs: IPv4, máscara e gateway; IPv6/prefixo e gateway. Forma automática dos clientes indicada. | 0,50 | |
| | | **Subtotal da entrega 1** | **1,00** | |

**Observações / pendências:**

________________________________________________________________________________

## Entrega 2 — Roteamento

| Aluno conferiu | Item | Critério de avaliação | Valor máximo | Nota |
| :---: | :---: | :--- | ---: | :---: |
| ☐ | 2.1 | Tabelas de roteamento IPv4/IPv6 dos cinco roteadores completas e coerentes com as redes remotas e o fluxo assimétrico exigido. | 0,50 | |
| | | **Subtotal da entrega 2** | **0,50** | |

**Observações / pendências:**

________________________________________________________________________________

## Entrega 3 — Rede Cabeada

**Escopo:** topologia cabeada da Figura 1. Os endereços reservados para os futuros APs permanecem no planejamento; os testes dos APs e notebooks pertencem à Entrega 4.

**Tudo-ou-nada:** nos itens 3.4 e 3.5, atribua os 2,00 pontos somente se todas as interfaces avaliadas estiverem acessíveis no respectivo protocolo. Uma falha implica nota zero naquele item. Para IPv6 entre redes, utilize GUA; teste link-local apenas no enlace correspondente.

| Aluno conferiu | Item | Critério de avaliação | Valor máximo | Nota |
| :---: | :---: | :--- | ---: | :---: |
| ☐ | 3.1 | DHCP/DNS nas três LANs: DHCPv4, SLAAC com gateway por RA, DNS por DHCPv6 stateless, registros A/AAAA dos três campi e resolução de nomes. | 1,00 | |
| ☐ | 3.2 | Servidores Web endereçados em IPv4/IPv6, HTTP ativo e páginas personalizadas com nome, RA e campus, acessíveis conforme a Tarefa 8. | 0,80 | |
| ☐ | 3.3 | Comunicação local cabeada em IPv4/IPv6: PCs, gateway, SVI e servidores locais acessíveis. | 0,70 | |
| ☐ | 3.4 | Comunicação em IPv4 de um PC de PB com todas as demais interfaces endereçadas da topologia cabeada — regra tudo-ou-nada. | 2,00 | |
| ☐ | 3.5 | Comunicação em IPv6 GUA de um PC de PB com todas as demais interfaces endereçadas da topologia cabeada — regra tudo-ou-nada. | 2,00 | |
| ☐ | 3.6 | Banner MOTD personalizado em todos os roteadores 2811. | 0,10 | |
| ☐ | 3.7 | Senhas com mínimo de 10 caracteres e proteção das senhas em texto simples conforme a Tarefa 7. | 0,10 | |
| ☐ | 3.8 | EXEC privilegiado protegido por senha secreta personalizada. | 0,10 | |
| ☐ | 3.9 | Acesso pelo console protegido conforme o enunciado. | 0,10 | |
| ☐ | 3.10 | Sessões de console e VTY encerradas após 5 minutos de inatividade. | 0,10 | |
| ☐ | 3.11 | Bloqueio por 120 segundos após três falhas de autenticação SSH em 60 segundos; comportamento verificado. | 0,10 | |
| ☐ | 3.12 | SSH conforme a Tarefa 7: domínio, usuário local, chave RSA e VTY 0 a 15 com autenticação local e somente SSH; acesso remoto testado. | 0,40 | |
| | | **Subtotal da entrega 3** | **7,50** | |

**Observações / pendências:**

________________________________________________________________________________

## Entrega 4 — Expansão com Wi-Fi

**Escopo:** topologia completa da Figura 2, com os três APs e notebooks, configuração e documentação da Tarefa 9.

| Aluno conferiu | Item | Critério de avaliação | Valor máximo | Nota |
| :---: | :---: | :--- | ---: | :---: |
| ☐ | 4.1 | AP e notebook incluídos e identificados em cada LAN; cabo do switch conectado à Gi1 do AP. | 0,20 | |
| ☐ | 4.2 | Endereços de gerenciamento dos APs conforme o planejamento inicial; DHCP do roteador sem fio desativado. | 0,20 | |
| ☐ | 4.3 | SSID e WPA2-PSK/AES corretos; associação com senha válida e falha com senha incorreta nas três LANs. | 0,20 | |
| ☐ | 4.4 | Notebooks com IPv4/IPv6 automáticos, nos mesmos prefixos e com gateway e DNS do campus. | 0,20 | |
| ☐ | 4.5 | Ping e serviços locais/remotos em IPv4/IPv6, acesso por nome e documentação Wi-Fi completa, mantendo a rede cabeada funcional. | 0,20 | |
| | | **Subtotal da entrega 4** | **1,00** | |

**Observações / pendências:**

________________________________________________________________________________

## Conferência dos Arquivos

Esta conferência apoia a entrega dos arquivos previstos no enunciado.

- [ ] Nome, RA e curso informados na documentação; nome e RA informados na topologia.
- [ ] Arquivos nomeados conforme a entrega correspondente.
- [ ] Documentação coerente com os endereços e as rotas implementados.
- [ ] Scripts dos roteadores e switches incluídos nas entregas 3 e 4, com um `.txt` por equipamento.
- [ ] Arquivo `.pkt` da versão correta incluído no ZIP de cada etapa de implementação.
- [ ] Na entrega 3, topologia cabeada funcional e endereços dos futuros APs preservados no planejamento.
- [ ] Na entrega 4, topologia completa com APs e notebooks, parâmetros Wi-Fi e testes documentados.
- [ ] Conferência realizada antes do envio pelo Moodle.

## Registro Final

**Entrega 1:** ______ / 1,00

**Entrega 2:** ______ / 0,50

**Entrega 3:** ______ / 7,50

**Entrega 4:** ______ / 1,00

**Nota total:** ______ / 10,00

**Teste de autoria, quando solicitado:** ____________________

**Observações finais do professor:**

________________________________________________________________________________