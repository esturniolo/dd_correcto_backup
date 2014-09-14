dd_correcto_backup
==================

Backup:
sudo dd bs=4M if=/dev/sdb | gzip > /home/your_username/image`date +%d%m%y`.gz

-----------------------------------------------------------------------------------

Restore:
sudo gzip -dc /home/your_username/image.gz | dd bs=4M of=/dev/sdb

-----------------------------------------------------------------------------------

Poniendo en el medio |pv| vemos el tiempo transcurrido.
