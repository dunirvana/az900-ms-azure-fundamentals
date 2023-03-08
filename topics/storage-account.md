## Conta de armazenamento

Uma conta de armazenamento do Azure ([Storage account](https://learn.microsoft.com/pt-br/azure/storage/common/storage-account-overview)) contém todos os seus objetos de dados do Armazenamento do Azure: blobs, arquivos, filas, tabelas e discos. A conta de armazenamento fornece um namespace exclusivo para os dados do armazenamento do Azure que podem ser acessados de qualquer lugar do mundo por HTTP ou HTTPS. Os dados em sua conta de armazenamento do Azure são duráveis e altamente disponíveis, seguros e amplamente escalonáveis.

### Redundância

É possível configurar a forma como se deseja que a redundancia dos dados ocorra da seguinte forma:

- Armazenamento com redundância local (Locally-redundant storage - LRS): a conta de armazenamento é replicada três vezes no mesmo data center;
- Armazenamento com redundância de zona (Zone-redundant storage - ZRS): a conta de armazenamento é replicada de modo síncrono em três zonas de disponibilidade do Azure distintas;
- Armazenamento co mredundância geográfica (Geo-redundant storage - GRS): copia seus dados de forma síncrona três vezes em um único local físico na região primária usando o LRS. Em seguida, ele copia seus dados de forma assíncrona para um único local físico em uma região secundária que está a centenas de quilômetros de distância da região primária
- Armazenamento com redundância de zona geográfica (Geo-zone-redundant storage - GZRS):  combina a alta disponibilidade fornecida pela redundância entre zonas de disponibilidade com a proteção contra interrupções regionais fornecidas pela replicação geográfica. Os dados em uma conta de armazenamento GZRS são copiados entre três zonas de disponibilidade do Azure na região primária e também são replicados para uma região geográfica secundária para proteção contra desastres regionais.
- Acesso de leitura (Read-Access): O armazenamento com redundância geográfica (com GRS ou GZRS) replica seus dados para outro local físico na região secundária para proteger contra interrupções regionais. Com uma conta configurada para GRS ou GZRS, os dados na região secundária não são diretamente acessíveis para usuários ou aplicativos, a menos que ocorra um failover. O processo de failover atualiza a entrada DNS fornecida pelo armazenamento do Azure para que o ponto de extremidade secundário se torne o novo ponto de extremidade primário de sua conta de armazenamento. Durante o processo de failover, seus dados são inacessíveis. Após a conclusão do failover, você pode fazer a leitura e gravar dados na nova região primária.

