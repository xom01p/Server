## Bastion EC2
Bastion Host를 AWS의 EC2(Elastic Compute Cloud) 인스턴스로 설정한 것
퍼블릭 서브넷에 EC2 인스턴스(Bastion) 생성
보안 그룹에서 SSH(22번 포트)만 특정 IP에서 접근 가능하도록 설정
내부 네트워크에 있는 Private EC2에는 SSH Key를 이용해 Bastion EC2를 통해 접근
 

## NoSQL Database
관계형 데이터베이스에서 볼 수 있는 기존 구조 외부에서 데이터를 저장하고 쿼리할 수 있는 데이터베이스 설계 접근 방식
 
## MongoDB
NoSQL DBMS의 한 종류.
MongoDB는 NoSQL로 분류되는 크로스플랫폼 도큐먼트 지향 데이터베이스 시스템 

## ElastiCache
분산 인메모리(In-memory) 캐싱 서비스
데이터베이스나 다른 백엔드 스토리지에서 가져오는 데이터를 캐싱(Cache)하여 액세스 속도를 향상시키는 데 사용됨
데이터를 더 빨리 가져오기 위한 메모리 기반의 저장소 서비스 

## Redis
오픈소스 인메모리 데이터 저장소로, 빠른 속도의 키-값(key-value) 데이터 구조를 제공한다.
보안이 중요한 경우: 기본 포트(6379) 대신 랜덤한 높은 포트(16379, 26379 등) 사용
 
## Application (2024지방기경)
Golang으로 개발된 바이너리
token 애플리케이션의 REST API 사용이 가능해야 합니다. 부록 2에 명시된 바이너리 사용 방법을 충분히 숙지하고, 애플리케이션을 운용해야 합니다. 또한, 컨테이너 이미지 내에서 curl 사용이 가능해야 합니다. 제공자료에 API 문서가 있습니다.

## Secrets Store
수명 주기 전반에 걸쳐 데이터베이스 자격 증명, 애플리케이션 자격 증명, OAuth 토큰, API 키 및 기타 보안 암호를 관리, 검색 및 교체하는 데 도움
JWT를 발행할 수 있게 user 애플리케이션에서 Secrets Manager에 접근할 수 있어야 합니다.

## Container Image Registry
애플리케이션 이미지 및 아티팩트를 안정적으로 배포할 수 있도록 뛰어난 성능 호스팅을 제공하는 완전관리형 컨테이너 레지스트리

## Container Orchestration
컨테이너 오케스트레이션은 대규모 애플리케이션을 배포할 수 있도록 컨테이너의 네트워킹 및 관리를 자동화하는 프로세스
EKS 기반의 Kubernetes로 Container Orchestration을 구성

## Kubernetes Cluster
Amazon EKS 제어 영역에는 etcd 및 Kubernetes API 서버와 같은 Kubernetes 소프트웨어를 실행하는 제어 영역 노드가 포함
 
## CloudWatch Logs
Amazon Elastic Compute Cloud(Amazon EC2) 인스턴스, Route 53 및 기타 소스에서 로그 파일을 모니터링 AWS CloudTrail, 저장 및 액세스

## Addon Nodegroup
EKS(Elastic Kubernetes Service)에서 제공하는 기능으로, 특정 Kubernetes 애드온을 AWS에서 직접 관리하는 EKS 관리형 노드 그룹(Nodegroup)입니다.

