## Load Balancer

O Azure Load Balancer opera na camada quatro do modelo OSI (Interconexão de Sistemas Abertos),  (camada OSI 4). É o ponto de contato único para clientes. O Load Balancer distribui fluxos de entrada que chegam nas instâncias de pool de front-end a back-end do balanceador de carga. Esses fluxos ocorrem de acordo com as investigações de integridade e regras de balanceamento de carga especificadas. As instâncias do pool de back-end podem ser Máquinas Virtuais ou instâncias do Azure em um conjunto de dimensionamento de máquinas virtuais.

Load balancing se refere a distribuição de carga (trafego de rede) entre os servidores.

Um balanceador de carga público pode fornecer conexões de saída para máquinas virtuais (VMs) dentro de sua rede virtual. Essas conexões são realizadas traduzindo seus endereços IP privados para endereços IP públicos. Os balanceadores de carga pública são usados para carregar o tráfego da Internet para balançar suas VMs.

Um balanceador de carga interno (ou privado) é usado onde os IPs privados são necessários apenas no front-end. Os balanceadores de carga internos são usados para carregar o tráfego de equilíbrio dentro de uma rede virtual. Um front-end de balanceador de carga pode ser acessado a partir de uma rede local em um cenário híbrido.