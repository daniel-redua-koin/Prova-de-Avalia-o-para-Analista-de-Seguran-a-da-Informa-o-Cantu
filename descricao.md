# Descritivo Técnico – Empresa de Pneus (Segurança da Informação)

## Cenário Geral
Ambiente híbrido com e-commerce em cloud pública e infraestrutura on-premise com 250 funcionários.

### Cloud
- Backend em .NET Core
- Frontend em Node.js
- Banco MongoDB em ReplicaSet (3 nós)

### On-Premise
- VMWare com FileServer, AD e PrintServer
- VPN e DLP para acesso remoto
- Backup local + cloud imutável

## Pilares CIA
**Confidencialidade:** MFA, JWT, TLS, DLP e IAM  
**Integridade:** Logs assinados, SAST/DAST, checksums e SIEM  
**Disponibilidade:** ReplicaSet, VMWare HA, balanceamento e backups 3-2-1  

## Resiliência de Dados
Backups automáticos testados, snapshots imutáveis e DRP com RTO ≤ 4h / RPO ≤ 15min.

## Melhorias Sugeridas
- Zero Trust Architecture
- ELK/Wazuh unificado
- Infra as Code (IaC)
- Treinamentos de phishing
