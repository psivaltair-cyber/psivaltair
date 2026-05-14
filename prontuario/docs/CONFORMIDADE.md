# Conformidade Legal - Prontuário Psicológico

## LGPD (Lei Geral de Proteção de Dados - Brasil)

### Princípios Implementados
- ✅ **Legalidade e Boa Fé**: Consentimento explícito do paciente
- ✅ **Finalidade**: Dados usados apenas para atendimento psicológico
- ✅ **Necessidade**: Coleta apenas de dados essenciais
- ✅ **Segurança**: Criptografia AES-256 em dados sensíveis
- ✅ **Não discriminação**: Proibição de uso para discriminação

### Direitos do Titular (Paciente)
1. **Direito de Acesso**: Endpoint `/api/auditoria/exportar-dados`
2. **Direito de Retificação**: PUT em endpoints de paciente
3. **Direito ao Esquecimento**: DELETE com soft delete
4. **Direito à Portabilidade**: Export em JSON/PDF
5. **Direito à Oposição**: Opt-out de marketing
6. **Não Submissão**: Sem perfilamento automático

### Armazenamento
- Retenção máxima: Até 5 anos após término do tratamento
- Backup automático em servidor seguro
- Deletion de backups após período de retenção
- Logs de todos os acessos (auditoria)

## Sigilo Profissional

### Proteções Implementadas
- Apenas psicólogo responsável pode acessar prontuário
- Acessos registrados e auditáveis
- Sem compartilhamento com terceiros sem consentimento
- Comunicação segura (HTTPS TLS 1.3+)
- Senhas hasheadas com bcrypt

## Consentimento

```
[ ] Autorizo o uso de meus dados para atendimento psicológico
[ ] Autorizo comunicações sobre meus atendimentos
[ ] Autorizo armazenamento seguro dos dados
[ ] Autorizo pesquisa científica (anônima)
[ ] Autorizo compartilhamento com equipe multidisciplinar
```

## Documentação Obrigatória

- ✅ Política de Privacidade
- ✅ Termo de Consentimento (TCLE)
- ✅ Política de Cookies
- ✅ Aviso de Segurança
- ✅ Contato DPO (Data Protection Officer)

## Conformidade CFP (Conselho Federal de Psicologia)

- Respeito à Resolução CFP nº 01/2009 (sigilo)
- Respeito à Resolução CFP nº 12/2020 (teleatendimento)
- Responsabilidade e competência técnica
- Segurança de informações

## Certificações Recomendadas

- [ ] ISO 27001 (Information Security Management)
- [ ] SOC 2 (Service Organization Control)
- [ ] Certificado SSL/TLS válido
- [ ] Backup e Disaster Recovery Plan

## Auditoria e Compliance

Logs armazenam:
- Usuário que acessou
- Recurso acessado (qual prontuário)
- Tipo de acesso (leitura, escrita, deleção)
- Timestamp
- IP address
- Resultado (sucesso/falha)

Retenção de logs: 2 anos (legislação exigida)
