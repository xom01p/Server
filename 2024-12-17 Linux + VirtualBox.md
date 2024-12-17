버츄얼 박스에서 리눅스를 사용한 2가상환경의 통신 구현

Vitualbox version
- vitualbox 7.0.0 vesion
(https://www.virtualbox.org/wiki/Download_Old_Builds_7_0)

---
## 기본 설정

C드라이브에 workspace라는 공간 생성
workspace 하위 폴더 생성
- basic
    - Ubuntu-22.04-64bit-VB
    - Ubuntu-24.04-64bit-VB
    - MobaXterm_Personal_24.4
- VMs
- VirtualBox (VirtualBox 7.0.0 version 다운장소)

---
## VirtualBox 실습과정
Home에서 가져오기를 선택후 Ubuntu 22.04 , 24.04를 설정 
![image](https://github.com/user-attachments/assets/403ebe9f-1643-4691-858f-01cdd526a96f)
머신 기본폴더를 workspace에 만든 VMs 라는곳에 할당
MAC 주소 정책 : 모든 네트워크 어뎁터의 새 MAC 주소 생성으로 변경

도구에서 네트워크 설정
NAT NetWorks 만들기 IPv4Prefix : 192.168.100.0/24 적용

가져온 Ubunt 가상환경의 설정에서 네트워크의 어뎁터1 NatNetwork로 변경

## Ubunt 실습과정
osboxes 기본 암호 osboxes.org

로그인 완료후 

terminal 명령어
>passwd )패스워드 변경 명령
>sudo passwd root )root 패스워드 변경 명령
>ip a )네트워크 상태 확인 
