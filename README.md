# resumo-dio-lab-criando-maquinas-virtuais-azure

### Acordos de Nível de Serviço (SLAs)

O SLA representa o tempo garantido de disponibilidade de um serviço na nuvem. Diferentes níveis de SLA oferecem diferentes períodos aceitáveis de inatividade:

- 99% SLA: 1,68 horas por semana, 7,2 horas por mês, 3,65 dias por ano
- 99,9% SLA: 10,1 minutos por semana
- 99,99% SLA: Aproximadamente 1 minuto por semana
- 99,999% SLA: Apenas 6 segundos por semana

Quanto mais "noves" no SLA, menor o tempo de inatividade permitido. Se a Microsoft não cumprir o SLA prometido para recursos nativos, o cliente deve ser ressarcido.

### Opções de Disponibilidade no Azure

O Azure oferece várias opções para garantir alta disponibilidade:

- **Zonas de Disponibilidade**: Permitem implantar VMs em diferentes zonas físicas dentro da mesma região
- **Conjuntos de Disponibilidade**: Agrupam VMs para proteger contra falhas localizadas
- **Conjuntos de Dimensionamento**: Recomendados para gerenciar múltiplas VMs em zonas diferentes

### Redundância de Armazenamento

O Azure oferece diversas opções de redundância para contas de armazenamento:

- LRS: Redundância local
- ZRS: Redundância de zona
- GRS: Redundância geográfica
- GZRS: Redundância geográfica com redundância de zona
- Opções RA: Redundância com acesso somente leitura

### Considerações Importantes

- Todo aumento de disponibilidade e redundância implica em aumento de custos
- É essencial questionar qual SLA é necessário antes de criar arquiteturas
- Entender o propósito do recurso (teste ou produção) é fundamental para definir a estratégia correta
- Planejamento adequado evita problemas de orçamento causados por configurações desnecessariamente robustas
