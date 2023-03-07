## VPN Gateway

Um gateway de VPN é um tipo específico de gateway de rede virtual usado para enviar tráfego criptografado entre uma rede virtual do Azure e um local pela Internet pública. Você também pode usar um gateway de VPN para enviar tráfego criptografado entre as redes virtuais do Azure pela rede da Microsoft.

### VPN de site a site

Uma conexão de gateway VPN Site a Site (S2S) é uma conexão por túnel VPN IPsec/IKE (IKEv1 ou IKEv2). As conexões S2S podem ser usadas para configurações entre instalações e híbridas. Uma conexão site a site exige um dispositivo VPN local com um endereço IP público atribuído a ele. Para saber mais sobre como selecionar um dispositivo VPN, confira as Perguntas Frequentes de Gateway de VPN - dispositivos VPN.

### VPN multi site

Você pode criar mais de uma conexão de VPN em seu gateway de rede virtual, normalmente se conectando a vários sites locais. Ao trabalhar com várias conexões, você deve usar um tipo de VPN baseado em rota (conhecido como gateway dinâmico ao trabalhar com redes virtuais clássicas). Como cada rede virtual pode ter apenas um gateway de VPN, todas as conexões por meio do gateway compartilham a largura de banda disponível. Esse tipo de conexão é frequentemente chamado de conexão de "vários sites".

### VPN ponto a site

Uma conexão de gateway de VPN Ponto a Site (P2S) permite que você crie uma conexão segura para sua rede virtual a partir de um computador cliente individual. Uma conexão P2S é estabelecida iniciando-a do computador cliente. Essa solução é útil para pessoas que trabalham remotamente que querem se conectar às VNets do Azure de um local remoto, como de casa ou de uma conferência. A VPN P2S também é uma solução útil para usar em vez de uma VPN S2S, quando você tiver apenas alguns clientes que precisam se conectar a uma rede virtual.

### Conexões de VNet para VNet (túnel VPN IPsec/IKE)

Conectar uma rede virtual a outra rede virtual é semelhante a conectar uma rede virtual (Rede Virtual para Rede Virtual) a um site local. Os dois tipos de conectividade usam um gateway de VPN para fornecer um túnel seguro usando IPsec/IKE. Você pode até combinar a comunicação VNet a VNet com as configurações de conexão de vários sites. Isso permite estabelecer topologias de rede que combinam conectividade entre instalações a conectividade de rede intervirtual.