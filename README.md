# netbox


; sudo a2enmod ssl proxy proxy_http headers
; sudo a2ensite netbox
; sudo systemctl reload netbox netbox-rqworker.service apache2.service
; source /opt/netbox/venv/bin/activate


; pip3.10 install netbox-topology-views==1.1.0
; pip3.10 install netbox-plugin-device-map

; sudo /opt/netbox/upgrade.sh
; sudo NETBOX_DELETE_LEGACY_DATA=1 /opt/netbox/upgrade.sh
; sudo systemctl restart netbox netbox-rqworker.service apache2.service


; sudo -i -u postgres psql


; GRANT ALL PRIVILEGES ON DATABASE netbox TO netbox;

; nano /etc/postgresql/14/main/pg_hba.conf


; PLUGINS_CONFIG = {
;     'netbox_topology_views': {
;         'allow_coordinates_saving': True,
;         'draw_default_layout': True,
;         'draw_interface_name': True,
;     }
; }