# SmartSpeakerWidyaWicara

Cara Running Smart Speaker

a. Jalankan setup sesuai prosedur 3.2.1 Host Setup di file PDF MT8516_Yocto_Linux_User_Guide_V2.7.3.pdf
b. Build source code, caranya seperti berikut :
1. Sync all compile
namaPC@namaPC:~/MT8516folder/hcn_overlay$ ./Sync_all_compile.sh

2. Set environment
namaPC@namaPC:~/MT8516folder$ . env.sh 06d_32b
output nya seperti berikut
======================================================================================
platform : bwd06 32b
======================================================================================

3. namaPC@namaPC:~/MT8516folder/build$ ./mybuild.sh

c. Jalankan smart speaker dengan cara :
1. Buka folder namaPC@namaPC:~MT8516/build/tmp/deploy/images/bwd06l-consys-emmc-128-32b
2. Open in terminal
3. Running smart speaker dengan python flashimage_adb.py
