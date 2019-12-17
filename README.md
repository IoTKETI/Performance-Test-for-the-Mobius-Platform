# Performance-Test-for-the-Mobius-Platform.

## Introduction
Mobius 플랫폼을 활용하는 중.소 기업들을 위해 Mobius 플랫폼이 성능이 어느 정도인지 파악할수 있도록 하며, 가용성 측면의 성능을 향상시키기 위한 방법과 확장성 측면의 성능을 향상시키기 위한 시스템의 구성 방안을 실제 성능 테스트 수행 결과를 기반으로 그 결과를 공유하고자 한다.

개방형 IoT 오픈 플랫폼(Mobius)에 대한 성능 테스트 환경 구축, 수행은 타겟 시스템에 대한 성능 테스트 및 진단을 통하여 시스템의 성능 저하 요인 등을 파악하고 이에 대한 개선을 통한 서버 처리능력의 향상을 목적으로 한다.
개방형 IoT 오픈 플랫폼(Mobius)이 적용된 시스템에 대한 성능 테스트의 방법 및 절차에 대한 기준을 제시한다. 이를 통하여 IoT 오픈 플랫폼 활용 기업의 시스템 성능을 위한 가이드로 활용될 수 있도록 한다.

## Performance Test Case

### Performance test in terms of availability.

#### - Single Server Configuration environment ( Mobius, MQTT Broker, Maria Database )
<img width="890" alt="스크린샷 2019-12-17 오후 4 27 09" src="https://user-images.githubusercontent.com/29790334/70976526-71fe8680-20ef-11ea-9f2f-5dc1427f8440.png">

#### - Mulity Server Configuration environment ( (Mobius, MQTT Broker, Maria Database) X 3 Set, L4 Switch )
<img width="883" alt="스크린샷 2019-12-17 오후 4 27 21" src="https://user-images.githubusercontent.com/29790334/70976556-7f1b7580-20ef-11ea-81b7-09188bd2d54f.png">

### Performance test in terms of scalability.

#### - Single Service Server + Single Database ( (Mobius, MQTT Broker) , Maria Database )
<img width="891" alt="스크린샷 2019-12-17 오후 4 27 31" src="https://user-images.githubusercontent.com/29790334/70976557-7f1b7580-20ef-11ea-9938-60e37df6fa00.png">

#### - Multiy Service Server + Single Database ( (Mobius, MQTT Broker) X 2 Set , Maria Database, L4 Switch )
<img width="883" alt="스크린샷 2019-12-17 오후 4 27 41" src="https://user-images.githubusercontent.com/29790334/70976558-7fb40c00-20ef-11ea-9b4b-a37bbaf43ad3.png">

## Performace Testing Tools & Agent PC
Apache Jmeter v5.1.1 : one of the leading tools used for load testing of web and application servers. ( Open Source )

Jmeter Agent running PC ( 7 Set )

## Author
Dong Ha Park (araha@keti.re.kr)
