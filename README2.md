## Criando Processos de Redundância de Arquivos na Azure

### Como funciona a redundância na Azure?

- **Configuração na conta de armazenamento:** A redundância é definida na conta, e todos os arquivos dentro dela seguem essa configuração.
- **Tipos principais de redundância:**
  - **LRS (Local):** 3 cópias no mesmo data center. Mais barato, mas menos seguro.
  - **ZRS (Zona):** 3 cópias em zonas diferentes da mesma região. Mais seguro e disponível.
- **Redundância geográfica:** Copia os dados para outra região distante (GRS ou GZRS) para proteger contra desastres.

### Insights importantes

- **Escolha depende do que você precisa:** custo x segurança.
- **ZRS é ótimo para alta disponibilidade.**
- **Failover:** Se a região principal cair, dá para mudar para a secundária (mas isso pode causar uma pausa).
- **Pode mudar a redundância depois, sem perder dados.**
