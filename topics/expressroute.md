## ExpressRoute

As conexões ExpressRoute não passam pela Internet pública. Isso permite que as conexões ExpressRoute ofereçam mais confiabilidade, velocidades mais rápidas, latências consistentes e maior segurança do que as conexões típicas pela Internet.

Você pode configurar uma VPN Site a Site como um caminho de failover seguro para o ExpressRoute ou usar VPNs Site a Site para se conectar a sites que não fazem parte de sua rede, mas estão conectados por meio do ExpressRoute. Observe que essa configuração exige dois gateways de rede virtual para a mesma rede virtual, um usando o tipo de gateway 'Vpn' e o outro usando o tipo de gateway 'ExpressRoute'.