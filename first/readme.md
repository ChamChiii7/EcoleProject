**초기 설정**
Ubuntu 설치
언어 선택
IP 설정
저장공간 설정
프로필 생성
패키지 최신화
*중요 이벤트(Install, Update, Upgrade 등등) 직전에 반드시 스냅샷 촬영*
*IP를 수동으로 할당할때*
sudo netplan generate
sudo vi /etc/netplan/50-cloud-init.yaml
적용 후 sudo netplan apply 명령어로 적용 후 ip addr 명령어로 수정사항 반영

sudo apt-get update && sudo apt-get upgrade -y
sudo reboot

터미널을 열기 위해 cockpit 설치 (cockpit의 기본 포트는 9090)
sudo apt-get install cockpit
sudo systemctl enable cockpit
sudo systemctl start cockpit
sudo ufw allow 9090/tcp

cloudpanel - installantion - other에서 DB 정하고 코드 복사

