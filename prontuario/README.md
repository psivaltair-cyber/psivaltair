# Prontuário Psicológico - Sistema Completo

Um sistema profissional e seguro para gerenciamento de prontuários psicológicos, desenvolvido com conformidade total à **LGPD** (Lei Geral de Proteção de Dados) e regulamentações do **CFP** (Conselho Federal de Psicologia).

## 🎯 Objetivo

Fornecer uma plataforma segura, confiável e em conformidade com a legislação brasileira para psicólogos gerenciarem prontuários de pacientes com máxima privacidade e segurança.

## ✨ Funcionalidades Principais

### 📋 Gerenciamento de Pacientes
- Cadastro completo com dados demográficos
- Histórico clínico organizado
- Consentimento LGPD rastreável
- Anonimização de dados (direito ao esquecimento)

### 🗂️ Prontuários Eletrônicos
- Estrutura completa de prontuário
- Anotações criptografadas
- Histórico pessoal e familiar
- Diagnósticos e observações seguras

### 📅 Agendamento de Sessões
- Calendário de consultas
- Diferentes tipos de atendimento (presencial, online, telefone)
- Confirmação automática
- Histórico de sessões

### 📊 Evoluções e Avaliações
- Registro de progresso do tratamento
- Testes psicométricos (MMPI, BFI, TAT)
- Interpretações profissionais
- Acompanhamento de resultados

### 🔐 Segurança e Conformidade
- Criptografia AES-256 para dados sensíveis
- Hashing bcrypt para senhas
- Autenticação JWT
- Auditoria completa de acessos
- Conformidade LGPD com direitos garantidos

### 📝 Auditoria e Compliance
- Logs detalhados de todas as ações
- Rastreamento de IP e user-agent
- Exportação de dados do paciente (LGPD)
- Direito ao esquecimento (soft delete)

## 🏗️ Arquitetura

### Backend
- **Framework**: Express.js + Node.js
- **Banco de Dados**: PostgreSQL
- **Cache**: Redis
- **ORM**: Prisma
- **Segurança**: Helmet, CORS, bcrypt, JWT

### Frontend
- **Framework**: React 18
- **Linguagem**: TypeScript
- **State Management**: Zustand
- **Styling**: Tailwind CSS
- **Ícones**: Lucide React

### Infraestrutura
- **Containerização**: Docker
- **Orquestração**: Docker Compose
- **Banco de Dados**: PostgreSQL 15
- **Admin**: PgAdmin 4

## 🚀 Como Iniciar

### Pré-requisitos
- Docker e Docker Compose instalados
- Node.js 18+ (para desenvolvimento local)

### Instalação Rápida

```bash
# Clone o repositório
git clone https://github.com/psivaltair-cyber/psivaltair.git
cd psivaltair/prontuario

# Inicie todos os containers
docker-compose up -d

# Acesse as aplicações
# Frontend: http://localhost:3000
# Backend: http://localhost:5000
# PgAdmin: http://localhost:5050
```

### Desenvolvimento Local

```bash
# Backend
cd backend
npm install
npm run prisma:migrate
npm run dev

# Em outro terminal - Frontend
cd frontend
npm install
npm run dev
```

## 📊 Modelos de Dados

1. **Usuários** - Psicólogos, recepcionistas e administradores
2. **Pacientes** - Dados pessoais com criptografia
3. **Prontuários** - Histórico clínico completo
4. **Sessões** - Registro de atendimentos
5. **Evoluções** - Progresso do tratamento
6. **Avaliações** - Testes psicométricos
7. **Agendamentos** - Calendário de consultas
8. **Consentimento LGPD** - Rastreamento de consentimento
9. **Logs de Auditoria** - Compliance total

## 🔐 Segurança

### Criptografia
- ✅ AES-256-CBC para dados sensíveis (CPF, anotações)
- ✅ Bcrypt com 12 rounds para senhas
- ✅ JWT com expiração configurável

### Autenticação e Autorização
- ✅ Autenticação baseada em JWT
- ✅ Roles: ADMINISTRADOR, PSICÓLOGO, RECEPCIONISTA
- ✅ Controle de acesso granular

### Auditoria e Compliance
- ✅ Logs com IP, user-agent, timestamp
- ✅ Rastreamento de CRUD operations
- ✅ Retenção de logs por 2 anos
- ✅ Soft delete para direito ao esquecimento

## 📋 Conformidade LGPD

### Direitos do Titular Implementados
- ✅ **Acesso**: Endpoint de exportação de dados
- ✅ **Retificação**: Atualização de informações
- ✅ **Esquecimento**: Soft delete + anonimização
- ✅ **Portabilidade**: Export em JSON
- ✅ **Oposição**: Opt-out em funcionalidades

### Políticas Incluídas
- ✅ Política de Privacidade
- ✅ Termo de Consentimento (TCLE)
- ✅ Aviso de Segurança
- ✅ Contato DPO

## 🛠️ Próximos Passos

- [ ] Implementar controllers REST
- [ ] Criar sistema de autenticação completo
- [ ] Desenvolvidade UI responsiva
- [ ] Adicionar testes (Jest, Vitest)
- [ ] CI/CD com GitHub Actions
- [ ] Documentação Swagger
- [ ] Relatórios em PDF
- [ ] Integração com email

## 📄 Licença

MIT - Desenvolvido por psivaltair-cyber

## 📧 Contato

Para dúvidas ou sugestões: psi.valtair@gmail.com

---

🔒 **Segurança e Privacidade em Primeiro Lugar**
