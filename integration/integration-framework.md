#통합 프레임워크 (EIP 기반의 프레임워크)

##Apache Camel
- 2.15.3
- 문서화가 잘 되어 있음
- 레퍼런스 (JBoss Fuse, ESB 구현)
- 다양한 컴포넌트 및 안정성

##Spring Integration
- 4.1.6
- 스프링 연계 (bean, config 그대로 사용), 훌륭한 성능
- In memory channel 기반 : 시스템 에러시 큐 데이터 유실 가능성, 로드밸런싱 X, 모니터링 도구 X
- 상대적으로 짧은 이력으로 변경이 많음

##비동기처리
Apache ActiveMQ
- 5.9.0
- JMS (only java)
- one to one, pub/sub
- byte, text, stream, map, object
- 안정성
- 관리자 콘솔: http://localhost:8161/admin (admin/admin)

##RabbitMQ
- 3.5.4
- AMQP (다양한 언어)
- direct, fanout, topic, headers
- binary type 만 지원
- 다양한 기능, 문서화, 사용편리성
- 20000 TPS (뛰어난 성능)
- 설치가 필요, 관리포인트가 증가
- High Availability
- 모니터링 도구 제공

##Apache Kafka
- 대용량 분산큐
- 100000 TPS

##통신프로토콜
JMS(Java Message Service) 
참조: http://docs.spring.io/spring-framework/docs/current/spring-framework-reference/html/jms.html

##대외연계
Netty

##모니터링
http://localhost:8161/hawtio
http://localhost:8161/admin/queues.jsp
http://localhost:8080/hawtio/login
