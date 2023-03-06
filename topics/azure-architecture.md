## Arquitetura Azure

### Infraestrutura global

A infraestrutura global do Azure é composta por dois componentes principais, sendo elas física e de componentes de rede. O componente físico é composto por mais de 160 datacenters físicos, organizados em regiões e conectados por uma das maiores redes do planeta.

### Como a infraestrutura é organizada?

- **Geografia**: Uma área do mundo que contém pelo menos uma região do Azure, são tolerantes a falhas para resistir à falha de uma região completa por meio de sua conexão à infraestrutura de rede de alta capacidade dedicada.

- **Região**: Uma região é um conjunto de data centers implantados em um perímetro definido por latência e conectados por meio de uma rede regional de baixa latência. 

- **Zonas de disponibilidade**: As Zonas de Disponibilidade são locais físicos exclusivos em uma região do Azure. Cada zona é composta por um ou mais datacenters equipados com energia, resfriamento e rede independentes. Para garantir a resiliência, há um mínimo de três zonas separadas em todas as regiões habilitadas. A separação física das Zonas de Disponibilidade dentro de uma região protege os aplicativos e dados contra falhas do datacenter.

### Regiões de emparelhamento

Cada região do Azure é sempre emparelhada com outra região na mesma geografia (como EUA, Europa ou Ásia) a pelo menos 300 milhas de distância. Essa abordagem permite a replicação de recursos (como armazenamento de VM) em uma geografia que ajuda a reduzir a probabilidade de interrupções devido a eventos como desastres naturais, distúrbios civis, quedas de energia ou interrupções de rede física que afetam ambas as regiões ao mesmo tempo. Se uma região em um par for afetada por um desastre natural, por exemplo, os serviços farão failover automaticamente para a outra região em seu par de regiões.

### Marketplace

Contém aplicativos e serviços prontos para serem utilizados, construidos pela própria Microsoft e parceiros.

### Precificação

- **Pay-as-you-go**: Pague pela capacidade de computação por segundo, sem compromisso de longo prazo ou pagamentos adiantados. Aumente ou diminua a capacidade de computação sob demanda. Comece ou pare a qualquer momento e pague apenas pelo que usar.

- **Instâncias de máquina virtual reservadas**: Uma instância de máquina virtual reservada do Azure é uma compra avançada de uma máquina virtual por um ou três anos em uma região especificada. O compromisso é feito desde o início e, em troca, você obtém uma economia de preço de até 72% em comparação com o preço pré-pago. As Instâncias de Máquina Virtual Reservadas são flexíveis e podem ser facilmente trocadas ou devolvidas.

- **Preço Spot**: Compre capacidade de computação não utilizada com grandes descontos - até 90 por cento em comparação com os preços pré-pagos. Se sua carga de trabalho pode tolerar interrupções e seu tempo de execução é flexível, o uso de VMs pontuais pode reduzir significativamente o custo de execução de sua carga de trabalho no Azure. Execute suas cargas de trabalho em máquinas virtuais ou conjuntos de escala de máquina virtual.

### Assinaturas

Uma assinatura do Azure é um contêiner lógico usado para provisionar recursos no Azure. Ele contém os detalhes de todos os seus recursos, como máquinas virtuais (VMs), bancos de dados e muito mais. Ao criar um recurso do Azure como uma VM, você identifica a assinatura à qual ele pertence. Qualquer conta do Azure pode ter várias assinaturas.

### Grupo de recursos

Um grupo de recursos é um contêiner que contém recursos relacionados para uma solução do Azure. O grupo de recursos pode incluir todos os recursos da solução ou apenas os recursos que você deseja gerenciar como um grupo. Você decide como deseja alocar recursos para grupos de recursos com base no que faz mais sentido para sua organização. Geralmente, adicione recursos que compartilham o mesmo ciclo de vida ao mesmo grupo de recursos para que você possa implementá-los, atualizá-los e excluí-los facilmente como um grupo.






