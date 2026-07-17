Certificaciones activas/disponibles/futuras (con los cambios del 1 de Julio) https://training.fortinet.com/local/cert/my/roadmap.php
Nueva herramienta de upgrade https://docs.fortinet.com/upgrade-tool/fortigate
FortiOS 7.6.7 liberado el 2 de junio https://docs.fortinet.com/document/fortigate/7.6.7/fortios-release-notes/743723
[Ojo con autoupgrade] FortiGuard DNS over TLS (96.45.45.45 / 96.45.46.46) roto en FortiOS 7.4.10, 7.4.11, 7.4.12 https://community.fortinet.com/fortigate-3/troubleshooting-tip-dns-unreachable-when-configured-with-dns-over-tls-on-fortigate-after-upgarde-to-v7-4-10-223784 Workaround Importar como CA https://cacerts.digicert.com/DigiCertHighAssuranceEVRootCA.crt
Nuevo bundle SDWAN (profundizar)

Auto Firmware Upgrade:
https://docs.fortinet.com/document/fortigate/7.6.4/administration-guide/369092/enabling-automatic-firmware-upgrades
https://docs.fortinet.com/document/fortigate/7.6.4/administration-guide/320693/required-firmware-upgrades-for-fortigate-appliances-with-invalid-support-contracts-or-that-have-reached-eoes

  - Equipos Sin licencia O En versión fin de soporte que alcancen fortiguard y versión superior a 7.4.8/7.6.4/8.0.0 - Se actualizan automáticamente al último patch (el último número)
  - Nos manda un correo, genera un evento y tenemos la opción de postponer 14 días
  - diagnose test application forticldd 13​ Es nuestro amigo.
  - Deshabilitado si: FMG o Fabric

Workaround 1: https://community.fortinet.com/t5/FortiGate/Technical-Tip-Auto-Firmware-Upgrade-feature-behavior-related-to/ta-p/360506

Workaround 2:

config system central-management 
    set type fortimanager
end

  

Auto Firmware Upgrade (por defecto) para entry level - https://docs.fortinet.com/document/fortigate/7.2.0/new-features/580180/enable-automatic-firmware-upgrades-by-default-on-entry-level-fortigates-7-2-6
Split Brain cuando actualizamos con Private Data Encryption - Sumar al proceso de upgrade la verificación de la variable:
https://community.fortinet.com/fortigate-3/troubleshooting-tip-failed-upgrade-to-7-6-6-on-ha-cluster-when-private-data-encryption-is-enabled-and-ha-password-is-set-227844
 
(Con FMG) Pérdida parcial de configuración de interfaces tras upgrade a FortiOS 7.6.4 https://community.fortinet.com/fortigate-3/troubleshooting-tip-partial-interface-configuration-loss-after-upgrading-fortigate-to-fortios-7-6-4-227678
Estamos en Mythos y hemos hecho público nuestro partnership con NVIDIA https://www.fortinet.com/corporate/about-us/newsroom/press-releases/2026/fortinet-deepens-integration-to-uniquely-secure-enterprise-ai-at-scale-with-nvidia
7.6.6 como versión recomendada para varios modelos https://community.fortinet.com/fortigate-3/technical-tip-recommended-release-for-fortios-116639
También para FMG y FAZ https://community.fortinet.com/fortimanager-27/technical-tip-recommended-release-for-fortimanager-and-fortianalyzer-119379
P2Pinfect (análisis) https://www.fortinet.com/blog/threat-research/misconfigured-enrolled-and-dormant-anatomy-of-a-p2pinfect-kubernetes-compromise

Debido a la renovación de certificados de los servidores FortiGuard Anycast que tendrá lugar el 14 de Abril, será necesario actualizar las versiones de FortiClient y FortiClient EMS a las versiones indicadas en los Customer Support Bulletins CSB-260303-1 y CSB-260320-1.
Version 7.4.10, 7.6.5, 8.0.0, allow-traffic-redirect esta disabled por defecto  https://community.fortinet.com/fortigate-3/technical-tip-how-icmp-redirect-works-in-fortigate-168404
Lanzamiento FortiOS 8.0 https://docs.fortinet.com/product/fortigate/8.0
Vulnerabilidad crítica en FortiClient EMS versiones 7.4.5 y 7.4.6 https://fortiguard.fortinet.com/psirt/FG-IR-26-099,
Ciclo de vida FortiOS 7.4 y 7.6 se extiende 1 año. Se ha extendido el ciclo de vida de ambas versiones en 1 año. Adicionalmente, FortiOS 7.6 se ha marcado como LTS (Long Term Support) con FortiCare Elite. FortiManager y FortiAnalyzer reflejan las fechas originales.
Cambios modelo certificación NSE desde 15 Julio 2026  https://www.fortinet.com/nse-training-update
Tentativa Q22026 FortiClient 8.0 para móviles con soporte IPSec
FortiManager 7.4.8 errores en la BBDD – Pasar a 7.4.11 o 7.6.últimaAAG (Agentless Application Gateway) en FortiADC https://docs.fortinet.com/document/fortiadc/8.0.0/new-features/219914/agentless-application-gateway-aag
LDAP connectivity fails after upgrade to v7.4.9  https://community.fortinet.com/t5/FortiGate/Troubleshooting-Tip-LDAP-connectivity-fails-with-error-This/ta-p/424025
FortiCloud SSO Login Authentication Bypass (CVE-2025-59718) on 7.4.9  https://www.reddit.com/r/fortinet/s/AbfoN66Qdf  
Conflictos con Cisco Ethertypes  https://docs.fortinet.com/document/fortigate/7.6.4/administration-guide/849059/ha-heartbeat-interface
Backup-hbdev  https://docs.fortinet.com/document/fortigate/7.6.0/new-features/474848/backup-heartbeat-interface-mitigates-split-brain-scenarios
Migración VPN SSL – IPSEC  https://docs.fortinet.com/document/fortigate/7.6.0/new-features/155142/migration-from-ssl-vpn-tunnel-mode-to-ipsec-vpn-7-6-3
FortiClient 7.4.4 IKEv2 only  https://docs.fortinet.com/document/forticlient/7.4.4/administration-guide/269675/forticlient-feature-comparison
VPNSSL to ZTNA Clientless  https://docs.fortinet.com/document/fortigate/7.6.0/new-features/545125/ztna-agentless-web-based-application-access-7-6-1
Flash de Imagen para equipos sin licencia  https://community.fortinet.com/t5/FortiGate/Technical-Tip-Formatting-and-loading-FortiGate-firmware-image/ta-p/197617
Enforcement FortiCloud Account  https://community.fortinet.com/t5/FortiGate/Technical-Tip-Enforcing-FortiCare-Registration-Starting-From-v7/ta-p/385926
SKUs y vouchers de Training  https://training.fortinet.com/local/staticpage/view.php?page=purchasing_process
LLM en el código del Malware  https://www.bleepingcomputer.com/news/security/google-warns-of-new-ai-powered-malware-families-deployed-in-the-wild/•	FortiClient 7.4.4 sin Cliente Gratuito https://docs.fortinet.com/document/forticlient/7.4.4/windows-release-notes/683433/special-notices
•	Gratis! Forticonverter de FGT a FGT https://docs.fortinet.com/document/forticonverter-service/25.1.0/online-help/724941/get-free-license-for-fortigate-conversion
•	FortiGate 7.4.8 GA altamente recomendable. Relevante cantidad de bugs resueltos.
-	Cambios funcionalidades equipos físicos 7.4.4 https://docs.fortinet.com/document/fortigate/7.4.0/new-features/519079/proxy-related-features-no-longer-supported-on-fortigate-2gb-ram-models-7-4-4
-	VPNSSL deshabilitado en 7.6 equipos físicos de menos de 2GB https://fndn.fortinet.net/index.php?/fortinetbeta/releases/main/&do=download&releaseid=98&id=5352&csrfKey=b39f2fdf21c75437cb87f517b56d8250
-	Migración VPNSSL a ZTNA https://docs.fortinet.com/document/fortigate/7.2.5/ssl-vpn-to-ztna-migration-guide/813800/deployment-overview
-	Comportamiento IPPools y VIPs: https://community.fortinet.com/t5/FortiGate/Technical-Tip-IP-pool-and-virtual-IP-behavior-changes-in-FortiOS/ta-p/277823
-	TENEMOS FORTIDEMO! https://fndn.fortinet.net/index.php?/one-click-demo/
-	Problemas con cuentas Training/Partner/FNDN – emea_partners@fortinet.com
-	Mantainer: Desde 7.2 en adelante no se puede utilizar el procedimiento de password recovery https://docs.fortinet.com/document/fortigate/7.2.0/new-features/482897/remove-maintainer-account-7-2-4
-	FAZ en cloud o por device: https://fortixpert.blogspot.com/2020/12/forticloud-premium-subscription.html
-	VPNSSL. En WebMode descontinuado – Apostar por ZTNA
-	Problemas complejos con FortiClient equipo de Endpoint, LUCIA ANTA RODRIGUEZ lucia.antarodriguez@telefonica.com
-	VirtualWire no permite asimetría de tráfico.
-	Nuevo Programa de certificaciones https://helpdesk.training.fortinet.com/support/solutions/articles/73000615006-transitioning-from-nse-4-5-and-6-to-the-fcp-certifications
-	Solicitud BUGS – Caso con soporte con ID de bugs – Si no obtenemos el nivel de detalle hgarciagil@fortinet.com ademercadocri@fortinet.com
-	Balanceo en cloud necesita resolver Google API. Si se cae el firewall los DNSs no resuelven. Solución: Conectar los DNS con Google Private Access para que accedan a Google API sin atravesar el firewall (políticas)
-	Logs FAZ FGT Cloud: Activar reliable para que se comunique por 514 TCP o modificar Security Group para que admita UDP
-	Fallo estético FQDNs https://community.fortinet.com/t5/FortiGate/Troubleshooting-Tip-FQDN-address-object-shows-unresolved-in-GUI/ta-p/278559
-	Upgrade 7.4.x, tomar medida en versión previa del consumo RAM y contrastar (además de chequeos habituales)
-	Herramienta iperf integrada en FortiGate - https://fortixpert.blogspot.com/2023/03/casos-de-uso-para-el-comando-diagnose.html y https://fortixpert.blogspot.com/2019/08/iperf-en-fortigate.html
-	Migración licencias EMS
-	Enlace correspondencia certificaciones https://helpdesk.training.fortinet.com/support/solutions/articles/73000625958-how-to-find-nse-certification-courses-on-the-fortinet-training-institute
-	Información certificaciones https://www.fortinet.com/lat/training-certification
-	FortiManager HA 7.0 no admite módulo de FAZ https://docs.fortinet.com/document/fortimanager/7.0.12/administration-guide/478954/enable-or-disable-fortianalyzer-features
-	Casos de uso FortiSOAR https://www.youtube.com/@SOCCSE
-	Debug autenticación/autorización https://community.fortinet.com/t5/FortiGate/Troubleshooting-Note-LDAP-FortiGate-error-message-Query-Failed/ta-p/189943
-	Guía integración FortiEDR con AD https://docs.fortinet.com/document/fortiedr/6.2.0/active-directory-integration/58917/overview
-	FAZ físico no permite cargar backup ni licencias si no accede a FortiGuard
-	HA con FortiManager https://docs.fortinet.com/document/fortimanager/7.4.3/administration-guide/981082/configuring-geo-redundant-ha-with-vrrp-failover
-	HA FortiManager en Azure, Templates y doc https://github.com/40net-cloud/fortinet-azure-solutions/tree/main/FortiManager/ha
-	FortiClient IPsec VPN Pre-Logon Video (Overview + Configuration & Demo).
-	FortiGate Cloud Automatic Upgrade https://community.fortinet.com/t5/FortiGate/Technical-Tip-How-to-disable-management-tunnel-to-FortiGate/ta-p/348924
-	Problemas Upgrade Clúster serie G https://community.fortinet.com/t5/FortiGate/Technical-Tip-FortiGate-90G-91G-120G-121G-HA-cluster-unable-to/ta-p/370831
-	ADJUNTO 14/02 – Transfer de equipos entre cuentas de FortiCloud sin ticket
-	Política de registro https://www.fortinet.com/corporate/about-us/legal/service-contract-activation-grace-period-policy
-	Problemas sonda Certificados en 7.2.11 – 7.4.5 https://community.fortinet.com/t5/FortiGate/Troubleshooting-Tip-How-to-fix-SSL-connection-is-blocked-due-to/ta-p/362052 set cert-probe-failure allow

-	Fasttracks! https://training.fortinet.com/local/staticpage/view.php?page=fast-track-workshop-abstracts
- Nuevo Laboratorio OT (the thinx, Oeste3 3ra planta):
- ACME Certs con FortiADC http://docs.fortinet.com/document/fortiadc/8.0.0/cli-reference/320309/execute-certificate-local-import-automate
- Nuevos Partner Roles https://docs.fortinet.com/document/forticloud/latest/identity-access-management-iam/600414/partner-roles
  *  Si generas partner role, el sub-user se borra 2:40
  *  Migrando a Partner role 3:45

