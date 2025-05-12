# devops-azure-db
# Guia de Banco de Dados no Azure

## Objetivo
Documentar o processo de configuração de bancos de dados na Azure, com foco no Azure SQL Database.

## Serviços de Banco de Dados Azure
- Azure SQL Database: Banco relacional totalmente gerenciado
- Cosmos DB: Banco NoSQL multi-modelo
- Azure Database for PostgreSQL/MySQL: Bancos de código aberto gerenciados

## Passo a Passo - Azure SQL Database

### 1. Criação do Banco
1. No Portal Azure, crie um novo "SQL Database"
2. Configure:
   - Grupo de recursos dedicado
   - Nome do banco az-db-dio
   - Criar novo servidor lógico
   - Definir credenciais de admin

### 2. Configurações Importantes
- Camada de serviço: Escolha conforme necessidade (Basic para testes)
- Redundância: Backup automático configurado
- Segurança**: Firewall para permitir seu IP

### 3. Conectando ao Banco
```sql
-- Exemplo de conexão via SQL Server Management Studio
Server name: dio-sql-server.database.windows.net
Authentication: SQL Server Authentication
Login: us.jrdio
Password: ********
