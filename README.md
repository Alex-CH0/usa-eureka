# Eureka Server

MSA로 구성된 환경에서 로드밸런싱 및 서비스 디스커버리를 담당하는 서버.
여러 Micro Service의 IP, Port, Instance ID를 가지고 관리해준다. 

## Configuration

Port: 8088

IP: localhost(추후 변경 예정)

여기서 관리될 서비스는
- API Gateway
- User Micro Service(이하 MS)
- Order MS
- Financial MS