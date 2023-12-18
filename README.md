arrynrob - for OBi200/OBi202/OBi212/OBi300/OBi302
If your current firmware version is less than 5853, just flash arrynrob directly.
If your firmware is 6259 or greater, you must install stock 5921EX first, then install bypass-uboot-mod.
If your firmware is >= 5853 and < 6259, you must bypass uboot by installing bypass-uboot-mod. Then, you can install arrynrob. DO NOT flash bypass-uboot-mod from 6259 or above, or you will be going to recovery mode (which also allows you to flash any firmware you want, but it just doesn't look as cool).
md5sum OBi302-3-2-2-6259-signed-fw-bypass-uboot-mod.fw = 59229dd211edb52d9f2e49729cee9794

Please read above installation instructions before install arrynrob!
Download - OBi2xx-3-2-2-8680EX-arrynrob11.fw
md5sum OBi2xx-3-2-2-8680EX-arrynrob11.fw = 7ef2a2d316e42c9c3d010ba7ec5deee3
Changes:
update clear_zt_params and param_dump to support hw_vers 1.5
the changes from arrynrob10:
enable dropbear ssh server. default root passwd = "obi".
(NEW) included a version of wget that supports https
patch OBiapp to bypass "zero touch" forced configuration. added clear_zt_params util to clear old zero touch params
patch OBiapp to use /scratch/contacts.xml for caller id number to name translation lookup.
patch OBiapp to bypass signed firmware check when loading new fw
patch OBiapp to bypass GVSIP provisioning lock
patch OBiapp to bypass 30x models GV initialization block
