# mf821_uqmi_openwrt_4g_script
4g  avantel script inicio uqmi mf821 


paso final de la configuracion de un router(mr3020) con internet por medio de red celular(4g avantel), por medio de modulo usb(mf821). 

----
ref 

http://lxr.free-electrons.com/source/drivers/net/usb/qmi_wwan.c

http://intelnuc.blogspot.com.co/2014/10/turn-your-old-wireless-router-into-lte.html

http://www.dd-wrt.com/wiki/index.php/Mobile_Broadband#ZTE

http://tiebing.blogspot.com.co/2015/03/linux-running-4g-lte-modem.html 

 http://intelnuc.blogspot.com.co/2014/10/turn-your-old-wireless-router-into-lte.html

enable

uqmi -d /dev/cdc-wdm0 --stop-network 0xffffffff --autoconnect

uqmi -d /dev/cdc-wdm0 --start-network lte.avantel.com.co --autoconnect

uqmi -d /dev/cdc-wdm0 --get-data-status

uqmi -d /dev/cdc-wdm0 --get-signal-info


