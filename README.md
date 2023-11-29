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

sudo apt-get update

- Docker prerequisite package 설치

sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release

- apt-transport-https:  HTTPS를 통해 APT 저장소를 사용할 수 있도록 해주는 도구
- ca-certificates:  인증서를 관리하기 위한 필수 패키지
- curl: URL을 통해 데이터를 전송하고 받을 수 있는 명령줄 도구
- gnupg: 암호화 및 디지털 서명 기능을 제공하는 GNU Privacy Guard
- lsb-release: Linux Standard Base 버전 및 정보를 제공하는 패키지


curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg







