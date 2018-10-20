# meck
Match MAC address against list, download&amp;create&amp;use official MAC vendor list.

This program will help:
                        - identify a MAC address against a list of adresses (default or passed)
                        - download and create a list of MAC addresses of vendors
                          and match a MAC address to a vendor in this list

positional arguments:
mac         search for MAC address in your list file (my_mac_addresses.txt) - NOt cASe Sensitive
              	Example: meck 1C:74:0D:11:22:33
              	==> Zyxel Communications Corporation
              	or
              	Example: meck 1C740D112233
              	==> Zyxel Communications Corporation
              
              List example: {MAC address}	{Adapter}	{Name}
              1C:74:0D:11:22:33		wlan	home_router

optional arguments:
  -h, --help  show this help message and exit
  -f F        set an other MAC address list and print it
              	Example: meck -f other_list_of_mac_addresses.txt 1C:74:0D:11:22:33
              	==> Zyxel Communications Corporation
  -u          update MAC vendor list from http://standards.ieee.org/develop/regauth/oui/oui.txt
  -v V        get MAC vendor name
              	Example: meck -v 1C:74:0D:11:22:33
              	==> Zyxel Communications Corporation

Free for use, but it's {up to|on} you. Enjoy:-)
