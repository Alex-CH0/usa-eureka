# Eureka Server

MSA로 구성된 환경에서 로드밸런싱 및 서비스 디스커버리를 담당하는 서버.
여러 Micro Service의 IP, Port, Instance ID를 가지고 관리한다. 

## Configuration

Port: 8088

IP: localhost(추후 변경 예정)

여기서 관리될 서비스는
- API Gateway
- User Micro Service(이하 MS)
- Order MS
- Financial MS


## Project 개요

본 프로젝트는 가상 투자 대회 서비스로 빗썸 API를 활용하여 선택된 코인정보를 불러와 
투자 수익률 계산 및 수익률 순위 대쉬보드를 제공한다.

프로젝트 구성은 MSA형태로 구성되며 구성요소로는
- Eureka Server
- API Gateway
- Front Server(웹)
- User Micro Service(이하 MS)
- Order MS
- Financial MS

이 있다.

## Repository

모노레포 vs 멀티레포

많은 고민이 있었지만 모놀리틱 서비스 (그리고 당연하게 따라오는 모노레포) 상황에서 
각 개발자가 진행하는 업무 단위별로 코드리뷰, 개발서버 배포, 상용서버 배포에 순탄하지 못한
순간들이 많았다. 

그리고 멀티레포가 가져오는 장점과 단점을 몸소 채험해보고 싶은 생각이 있다.

따라서 본 프로젝트는 멀티레포로 관리되며, URL은 아래와 같다. 

[API Gateway Github Link](https://github.com/Alex-CH0/usa-gateway)

[Front Server(웹) Github Link](https://github.com/Alex-CH0/usa-client)

[User Micro Service Github Link](https://github.com/Alex-CH0/usa-user-service)

[Order Micro Service Github Link](https://github.com/Alex-CH0/usa-order-service)

[Finance(빗썸 API) Micro Service Github Link](https://github.com/Alex-CH0/usa-finance-service)



