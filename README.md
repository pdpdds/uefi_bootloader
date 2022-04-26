# uefi_bootloader
limine + stivale2

## 환경
우분투 20.04 LTS

## 빌드
```
https://wikidocs.net/164084 문서를 참고해서 x86_64-elf 크로스 컴파일러를 만든다.  
export PATH="/opt/cross/bin:$PATH" 

git clone https://github.com/pdpdds/uefi_bootloader
cd uefi_bootloader/limine
chmod 744 limine-install
cd ..
make
```

## 실행
```
qemu-system-x86_64 -hda disk.hdd
```
