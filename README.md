strategy:
  matrix:
    model: ["A105FN"]
  - name : Kernel configure
    run : |
      ./cruelbuild config \
                   model = $ {{matrix.model]] \
                   name = "Unicornio-v1.0" \
                   + magisk \
                   + nohardeing \
                   + ttl \
                   + wireguard \
                   + cifs \
                   + sdfat \
                   + ntfs \
                   + morosound \
                   + boeffla_wl_blocker
                   + magisk = canary
                   dtb
                   empty_vbmeta
                   alwais_permit
                   25hz
                   noatime
                   simple_lmk
                   io_bfq
                   io_maple
                   io_fiops
                   io_sio
                   io_zen
                   io_anxiety
                   io_noop
                   io_cfq
                   + sdfat
                   + ntfs
                   + cifs
                   tcp_cubic
                   tcp_westwood
                   tcp_htcp
                   tcp_bbr
                   tcp_bic
                   sched _...
                   ttL
                   mass_storage
                   + wireguard
                   + morosound
                   + boeffla_wl_blocker
                   + nohardening
                   nohardening2
                   size
                   performance
                   + nodebug
                   usb_serial
                   fake_config
