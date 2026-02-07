# RELATÓRIO DE ANÁLISE DE RISCOS  
Projeto: Análise de Riscos em Segurança da Informação  
Data: (inserir data)  
Responsável: Raydeman Santiago Sidon da Rocha  

---

## 1. INTRODUÇÃO

Este relatório apresenta os resultados da análise de riscos realizada em ambiente corporativo simulado (Hospital Público com infraestrutura de TI), com base nas diretrizes da ISO/IEC 27005 e NIST SP 800-30 Rev.1.

O objetivo foi identificar ativos críticos, ameaças associadas, avaliar o nível de risco e propor estratégias de tratamento.

---

## 2. ESCOPO

O escopo da análise compreende os seguintes componentes do ambiente:

- Servidor de Prontuário Eletrônico
- Banco de Dados Institucional
- Firewall de Borda
- Estações Administrativas
- Sistema de Backup

A análise considera riscos relacionados à confidencialidade, integridade e disponibilidade das informações.

---

## 3. METODOLOGIA

A metodologia aplicada seguiu as seguintes etapas:

1. Definição do contexto organizacional
2. Identificação e classificação de ativos
3. Identificação de ameaças e vulnerabilidades
4. Avaliação de impacto (1 a 3)
5. Avaliação de probabilidade (1 a 3)
6. Cálculo do risco (Impacto x Probabilidade)
7. Classificação do nível de risco
8. Definição de plano de tratamento

Critério de classificação:

- 1–3: Baixo  
- 4–6: Médio/Alto  
- 7–9: Crítico  

---

## 4. IDENTIFICAÇÃO DE ATIVOS CRÍTICOS

| ID | Ativo | Criticidade |
|----|--------|------------|
| A1 | Servidor de Prontuário | Alta |
| A2 | Banco de Dados | Alta |
| A3 | Firewall | Alta |
| A4 | Estações Administrativas | Média |
| A5 | Sistema de Backup | Alta |

Os ativos A1, A2 e A5 foram considerados críticos por armazenarem dados sensíveis de pacientes e informações institucionais.

---

## 5. AVALIAÇÃO DE RISCOS

### 5.1 Risco 1 – Ransomware no Servidor de Prontuário

Impacto: 3 (Alto)  
Probabilidade: 3 (Alta)  
Nível de Risco: 9 (Crítico)

Justificativa:
A indisponibilidade do prontuário eletrônico comprometeria atendimentos médicos, podendo gerar impacto operacional grave e risco à continuidade do serviço.

---

### 5.2 Risco 2 – Vazamento de Dados do Banco de Dados

Impacto: 3 (Alto)  
Probabilidade: 2 (Média)  
Nível de Risco: 6 (Alto)

Justificativa:
O banco contém dados pessoais e médicos sensíveis. Um vazamento pode gerar sanções legais (LGPD) e dano reputacional.

---

### 5.3 Risco 3 – Ataque DDoS ao Firewall

Impacto: 2 (Médio)  
Probabilidade: 2 (Média)  
Nível de Risco: 4 (Moderado)

Justificativa:
Pode causar indisponibilidade temporária, mas há possibilidade de mitigação por provedores externos.

---

### 5.4 Risco 4 – Falha no Sistema de Backup

Impacto: 3 (Alto)  
Probabilidade: 2 (Média)  
Nível de Risco: 6 (Alto)

Justificativa:
Caso o backup não esteja íntegro, um incidente pode resultar em perda permanente de dados críticos.

---

## 6. PLANO DE TRATAMENTO

| Risco | Estratégia | Ação Recomendada |
|--------|------------|------------------|
| Ransomware | Mitigar | Implementar EDR, backup offline e segmentação de rede |
| Vazamento de Dados | Mitigar | Implementar criptografia em repouso e MFA |
| DDoS | Mitigar | Contratar proteção anti-DDoS junto ao ISP |
| Falha de Backup | Mitigar | Testes trimestrais de restauração e verificação automática |

Prioridade imediata: Ransomware (Risco Crítico).

---

## 7. CONCLUSÃO

A análise identificou um risco crítico relacionado a ransomware, exigindo priorização imediata de controles técnicos.

Foram identificados dois riscos de nível alto (vazamento de dados e falha de backup), que demandam medidas estruturais de mitigação.

O ambiente apresenta maturidade intermediária em segurança, porém necessita fortalecimento de controles preventivos e processos formais de governança.

Recomenda-se:

- Implantação de MFA institucional
- Política formal de backup testado
- Plano de resposta a incidentes
- Monitoramento contínuo de vulnerabilidades

A aplicação sistemática da gestão de riscos permitirá redução progressiva da exposição organizacional.

---

## 8. REFERÊNCIAS

- ISO/IEC 27005 – Information Security Risk Management
- ISO/IEC 27001:2022 – Information Security Management Systems
- NIST SP 800-30 Rev.1 – Guide for Conducting Risk Assessments
