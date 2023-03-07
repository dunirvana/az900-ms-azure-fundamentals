## Rede Virtual

- A Rede Virtual do Azure (VNet) é o bloco de construção fundamental para sua rede privada no Azure. A VNet permite que muitos tipos de recursos do Azure, como as Máquinas Virtuais do Azure (VM), se comuniquem com segurança uns com os outros, com a Internet e com redes locais.

- Espaço de endereço: ao criar uma VNet, você deve especificar um espaço de endereço IP privado personalizado usando endereços públicos e privados (RFC 1918).

- Sub-redes: as sub-redes permitem que você segmente a rede virtual em uma ou mais sub-redes e aloque uma parte do espaço de endereço da rede virtual para cada sub-rede. 

- Regiões: a VNet tem como escopo uma única região / local; entretanto, várias redes virtuais de diferentes regiões podem ser conectadas usando o peering de rede virtual.

- VNet tem como escopo uma assinatura. Você pode implementar várias redes virtuais em cada assinatura e região do Azure. - Relacionado com o AD