# PLANO DE RESPOSTA A INCIDENTES (PRI)

Projeto Integrado à Análise de Riscos  
Responsável: Raydeman Santiago Sidon da Rocha  
Data: (inserir data)

---

## 1. OBJETIVO

Estabelecer diretrizes formais para identificação, contenção, erradicação e recuperação de incidentes de segurança da informação, reduzindo impactos operacionais, financeiros e reputacionais.

---

## 2. ESCOPO

Aplica-se aos seguintes ativos críticos:

- Servidor de Prontuário Eletrônico
- Banco de Dados
- Firewall de Borda
- Sistema de Backup
- Estações Administrativas

---

## 3. CLASSIFICAÇÃO DE INCIDENTES

| Nível | Descrição |
|--------|-----------|
| Baixo | Incidente com impacto limitado e facilmente contornável |
| Médio | Interrupção parcial de serviços |
| Alto | Comprometimento de dados ou indisponibilidade significativa |
| Crítico | Paralisação total ou vazamento de dados sensíveis |

---

## 4. EQUIPE DE RESPOSTA (CSIRT INTERNO SIMULADO)

- Coordenador de Segurança
- Analista de TI
- Administrador de Redes
- Responsável Jurídico (quando aplicável)
- Comunicação Institucional

---

## 5. FASES DO PROCESSO (Baseado no NIST 800-61)

### 5.1 Preparação

- Implementação de EDR
- Backup offline validado
- Política de acesso com MFA
- Treinamento de equipe

---

### 5.2 Identificação

- Monitoramento de logs
- Alertas de antivírus/EDR
- Detecção de tráfego anômalo
- Relato de usuários

---

### 5.3 Contenção

Curto prazo:
- Isolamento do equipamento afetado
- Bloqueio de contas comprometidas

Longo prazo:
- Segmentação de rede
- Atualização de regras de firewall

---

### 5.4 Erradicação

- Remoção de malware
- Correção de vulnerabilidades
- Aplicação de patches
- Reconfiguração segura

---

### 5.5 Recuperação

- Restauração de backup validado
- Monitoramento reforçado
- Testes de integridade

---

### 5.6 Lições Aprendidas

- Revisão do incidente
- Atualização da matriz de risco
- Ajuste de controles preventivos
- Relatório executivo para diretoria

---

## 6. PROCEDIMENTO ESPECÍFICO – RANSOMWARE (RISCO CRÍTICO)

1. Isolar servidor imediatamente
2. Desconectar da rede
3. Validar integridade dos backups
4. Notificar gestão
5. Preservar evidências para análise forense
6. Restaurar ambiente somente após validação completa

---

## 7. INTEGRAÇÃO COM A ANÁLISE DE RISCOS

Os incidentes tratados neste plano estão diretamente relacionados aos riscos identificados anteriormente:

- Ransomware → Risco Crítico
- Vazamento de Dados → Risco Alto
- Falha de Backup → Risco Alto
- DDoS → Risco Moderado

A cada incidente confirmado, a matriz de risco deve ser revisada.

---

## 8. COMUNICAÇÃO

Em caso de incidente relevante:

- Comunicação interna imediata
- Notificação à direção
- Avaliação de necessidade de comunicação externa
- Avaliação de obrigação legal (LGPD)

---

## 9. CONCLUSÃO

Este Plano de Resposta a Incidentes fortalece a maturidade de segurança do ambiente, reduzindo o tempo de resposta e mitigando impactos organizacionais.

Sua aplicação contínua contribui para melhoria da governança e conformidade com boas práticas internacionais.
