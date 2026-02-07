# RELATÓRIO EXECUTIVO  
Análise de Riscos em Segurança da Informação  

Responsável: Raydeman Santiago Sidon da Rocha  
Data: (inserir data)  

---

## 1. OBJETIVO

Apresentar de forma resumida os principais riscos identificados no ambiente de TI do hospital simulado, bem como as recomendações estratégicas para mitigação.

A análise foi conduzida com base nas boas práticas da ISO/IEC 27005 e NIST SP 800-30.

---

## 2. PRINCIPAIS RISCOS IDENTIFICADOS

Após avaliação dos ativos críticos (Servidor de Prontuário, Banco de Dados, Firewall e Sistema de Backup), foram identificados os seguintes riscos prioritários:

### 🔴 Risco Crítico
**Ransomware no Servidor de Prontuário**  
Impacto: Alto  
Probabilidade: Alta  
Consequência: Paralisação de atendimentos e possível perda de dados sensíveis.

---

### 🟠 Riscos Altos
**Vazamento de Dados Sensíveis**  
Possível exposição de informações pessoais e médicas, com impacto legal (LGPD) e reputacional.

**Falha no Sistema de Backup**  
Risco de perda permanente de dados em caso de incidente.

---

### 🟡 Risco Moderado
**Ataque DDoS ao Firewall**  
Possível indisponibilidade temporária dos serviços.

---

## 3. IMPACTOS POTENCIAIS

- Interrupção de serviços essenciais
- Comprometimento de dados sensíveis
- Sanções regulatórias
- Danos reputacionais
- Perdas financeiras indiretas

---

## 4. RECOMENDAÇÕES PRIORITÁRIAS

1. Implementação de solução EDR contra ransomware
2. Implantação obrigatória de MFA para acessos críticos
3. Política formal de backup com testes trimestrais de restauração
4. Criptografia de dados sensíveis
5. Desenvolvimento de Plano de Resposta a Incidentes

---

## 5. CONCLUSÃO EXECUTIVA

O ambiente apresenta exposição significativa a ameaças modernas, especialmente ransomware.

A adoção imediata de controles técnicos e administrativos reduzirá substancialmente o nível de risco organizacional e aumentará a maturidade em segurança da informação.

Recomenda-se priorização orçamentária para implementação das medidas propostas no curto prazo.
