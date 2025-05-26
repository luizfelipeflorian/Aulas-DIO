## Github e Azure Devops para Versionamento e Backups

### Processo Básico

- **Versionamento:**  
  Use Git para controlar versões do código no GitHub ou Azure DevOps. Faça commits, crie branches para recursos e use pull requests para revisar o código.  

- **Backup Automatizado:**  
  Use scripts (como Bash) que clonam seus repositórios do GitHub e espelham no Azure DevOps. Isso cria uma cópia segura em outra plataforma.  

- **Pipeline no Azure DevOps:**  
  Configure um pipeline para rodar o script automaticamente, seja agendado ou manual, garantindo backups regulares.  

### Insights Importantes

- **Exclusão e Inclusão:**  
  O script pode ignorar repositórios que você não quer copiar, facilitando o controle.  

- **Suporte a Git LFS:**  
  Arquivos grandes são tratados corretamente, garantindo backup completo.  

- **Segurança:**  
  Tokens de acesso (PATs) são guardados como variáveis secretas no Azure DevOps para proteger as credenciais.  

- **Verificação:**  
  Você pode conferir no Azure DevOps se os repositórios foram criados/atualizados e ver logs do pipeline para garantir que tudo funcionou.  

### Possibilidades

- **Migração e Sincronização:**  
  Mantenha GitHub e Azure DevOps sincronizados, facilitando migração ou backup cruzado.  

- **Recuperação Rápida:**  
  Em caso de perda ou exclusão acidental, restaure o código rapidamente a partir do backup no Azure DevOps.
