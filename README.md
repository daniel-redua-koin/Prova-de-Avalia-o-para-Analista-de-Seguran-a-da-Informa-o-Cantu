Prova de Avaliação – Analista de Segurança da Informação

Candidato
**Nome:** Daniel Redua  
**Cargo Pretendido:** Analista de Segurança da Informação  

---

 Cenário
A prova aborda um ambiente híbrido de uma **empresa de pneus**, que possui:
- **Ambiente Cloud Pública:** e-commerce crítico (80% da receita) com backend em **.NET Core**, frontend em **Node.js** e banco de dados **MongoDB ReplicaSet**.  
- **Infraestrutura On-Premise:** ambiente **VMWare** com **FileServer**, **Active Directory** e **PrintServer** utilizados por 250 colaboradores híbridos.  
- **Comunicação:** via **e-mail corporativo**, com envio de informações confidenciais internas e externas.  

---

 Objetivo
Projetar as **fortalezas do ambiente** considerando os **três pilares da Segurança da Informação (CIA)** — Confidencialidade, Integridade e Disponibilidade — incluindo práticas de **resiliência de dados** e propostas de **melhoria contínua** tanto em **cloud** quanto **on-premise**.

---

 Estrutura do Projeto
| Arquivo | Descrição |
|----------|------------|
| `diagrama.drawio` | Diagrama técnico do ambiente híbrido |
| `diagrama.png` | Versão visual do diagrama (para visualização rápida) |
| `descricao.md` | Documento técnico descritivo dos pilares e medidas de segurança |
| `README.md` | Apresentação geral e instruções de entrega |

---

 Principais Medidas Implementadas
 Cloud Pública
- Autenticação **MFA** e tokens **JWT**  
- **Criptografia TLS 1.3** e **AES-256**  
- **WAF**, **API Gateway** e controle de acesso **IAM/RBAC**  
- **Backup em nuvem imutável (MFA Delete)**  

🏠 On-Premise
- **Active Directory** com GPOs e políticas de senha  
- **VPN SSL** para acesso remoto seguro  
- **DLP e MDM** para prevenção de vazamento de dados  
- **VMWare HA** e **backup 3-2-1**  

### 📧 Comunicação
- **SPF**, **DKIM**, **DMARC** e **TLS** para e-mails corporativos  
- **Treinamentos anti-phishing** e campanhas de conscientização  

---

Pilares CIA
- **Confidencialidade:** controle de acesso, criptografia e DLP  
- **Integridade:** logs assinados, checagem de integridade e SIEM  
- **Disponibilidade:** alta disponibilidade, redundância e DRP  

---

Resiliência de Dados
- Backups diários automáticos testados semanalmente  
- Snapshots imutáveis com retenção configurada  
- Plano de Disaster Recovery com **RTO ≤ 4h / RPO ≤ 15min**  
- Integração de **SIEM (Wazuh)** para correlação de eventos e alertas  

---

🚀 Melhorias Propostas
- Adoção de **Zero Trust Architecture**  
- Centralização de logs com **ELK/Wazuh**  
- **Infraestrutura como Código (IaC)**  
- **Monitoramento físico** do armazém integrado ao SIEM  

---

Prova de Avaliação | Analista de Segurança da Informação
