## Gateway de Aplicativo

O Gateway de Aplicativo pode tomar decisões de roteamento com base em atributos adicionais de uma solicitação HTTP, por exemplo, caminho URI ou cabeçalhos de host. Por exemplo, você pode rotear o tráfego com base na URL de entrada. Portanto, se /images estiver na URL de entrada, você pode rotear o tráfego para um conjunto específico de servidores (conhecido como pool) configurado para imagens. Se /video estiver no URL, esse tráfego é encaminhado para outro pool otimizado para vídeos.

Esse tipo de roteamento é conhecido como balanceamento de carga da camada de aplicativo (camada OSI 7). O Gateway de Aplicativo do Azure pode fazer o roteamento baseado em URL e muito mais.