# MLOPS-Project

## ML DevOps=MLOps

### MLOps 구성 요소

1. 데이터
   
데이터 수집 파이프라인: Sqoop, Flume, Kafka, Flink, Spark Streaming, Airflow

데이터 저장:MySQL, Hadoop, S3, MinlO

데이터 관리: TFDV, DVC, Feast, Amundsen

   
2. 모델

모델 개발: Jupyter Hub, Docker, Kubeflow, Optuna, Ray, Katib

모델 버전 관리: Git. MLflow, Github Action, jenkins

모델 학습 스케줄링 관리: Grafana, Kubernetes
  
3. 서빙

  모델 패키징: Docker, Flask, FastAPI, BentoML, Kubeflow, TFServing, seldon-core

  서빙 모니터링: Prometheus, Frafana, Thanos

  파이프라인 매니징: Kubeflow, argo workflows, Airflow

# Docker & Kubernetes

1. Containerization: 컨테이너화 하는 기술

2. Container: 격리된 공간에서 프로세스를 실행시킬 수 있는 기술

Build Once=> Run Anywhere

# 환경 구축

1. Oracle VM Virtual Box 설치

링크: https://www.virtualbox.org/wiki/Download_Old_Builds_6_1

version: virtualBox 6.1.26

2. Unbuntu 설치

링크: http://lt.releases.ubuntu.com/20.04.3/

version: ubuntu 20.04.3

3. 가상환경 구축

![image](https://github.com/TaewonEum/MLOPS-Project/assets/104436260/5148d53a-fe79-47cb-a324-1ca0f8fdefe8)

Oracle VM VirtualBox 접속-> 새로 만들기-> Linux, Ubuntu 설정

# Docker 설치

가상환경내에 Docker설치 후 설치 확인 까지

- apt 패키지 업데이터

![image](https://github.com/TaewonEum/MLOPS-Project/assets/104436260/8477ddbe-dc22-4897-948d-9daa0bf7af8c)

- Docker prerequisite package 설치

![image](https://github.com/TaewonEum/MLOPS-Project/assets/104436260/3d1a9ea6-a134-4be8-9258-4a4b5fc27ae5)

1) apt-transport-https:  HTTPS를 통해 APT 저장소를 사용할 수 있도록 해주는 도구
2) ca-certificates:  인증서를 관리하기 위한 필수 패키지
3) curl: URL을 통해 데이터를 전송하고 받을 수 있는 명령줄 도구
4) gnupg: 암호화 및 디지털 서명 기능을 제공하는 GNU Privacy Guard
5) lsb-release: Linux Standard Base 버전 및 정보를 제공하는 패키지

- 도커 공식 GPG key를 생성합니다

![image](https://github.com/TaewonEum/MLOPS-Project/assets/104436260/0860c592-8e17-450f-8605-6c298be4454d)

- 이후 코드

echo \
"deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] http
s://download.docker.com/linux/ubuntu \
$(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /de
v/null

sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io 

sudo docker run hello-world

![image](https://github.com/TaewonEum/MLOPS-Project/assets/104436260/8b5732a2-a61b-4801-b482-8d13339376f4)

다음과 같은 실행문이 나온다면 정상적으로 설치 된 것

sudo usermod -a -G docker $USER
sudo service docker restart


- 실행 중인 컨테이너의 목록을 표시

![image](https://github.com/TaewonEum/MLOPS-Project/assets/104436260/419a7e2f-1aec-44a1-b10f-12ded1dfe679)









