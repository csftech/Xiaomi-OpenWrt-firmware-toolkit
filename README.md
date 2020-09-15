# Xiaomi-OpenWrt-firmware-toolkit

**Description**

This tool enables you to do further research on Xiaomi IoT device.

The toolkit currently have two features, (1) show info (2) extraction.

**Usage**

```bash
# show firmware info
python ./toolkit.py -s ./mico_all_0f70e_1.34.36.bin
# extract firmware (-d or --dest for setting destination directory)
python ./toolkit.py -d /home/user/mico -e ./mico_all_0f70e_1.34.36.bin
# print usage
python ./toolkit.py -h
```

As far as I know, Xiaomi router and speaker devices are based on OpenWrt system.

The firmware name always starts with its `product id`, followed by `model id`, `string: "all"||"firmware"`, `MD5 hash last 5 characters`, and the last `version number`.

For Example:
1. `miwifi_r4ac_firmware_cc751_2.18.53.bin`
   
    `product id`: miwifi, `model id`: r4ac

2. `mico_all_0f70e_1.34.36.bin`
       
    `product id`: mico
3. `miwifi_r3a_all_da132_2.18.40.bin`

    `product id`: miwifi, `model id`: r3a
