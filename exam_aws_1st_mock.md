### **AWS 클라우드 전문가(CLF-C02) 최종 실전 모의고사 1st**

---

1. 회사가 초기 하드웨어 구매 비용을 없애고 사용한 만큼만 비용을 지불하는 클라우드 컴퓨팅 모델로 전환하려고 합니다. 이는 AWS 클라우드의 어떤 이점에 해당합니까?

A. 규모의 경제

B. 자본 비용(CAPEX)을 가변 비용(OPEX)으로 전환

C. 비즈니스 민첩성 향상

D. 보안 및 규정 준수

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

설명:

<b>B (정답):</b> 서버 같은 물리적 자산을 미리 구매하는 막대한 초기 투자(자본 비용)를, 사용한 만큼만 지불하는 월별 운영 비용(가변 비용)으로 전환하는 것은 AWS 클라우드의 가장 핵심적인 경제적 이점입니다.

<b>A (오답):</b> 규모의 경제는 AWS가 대규모로 운영하기 때문에 사용자에게 더 저렴한 요금을 제공할 수 있다는 이점입니다.

</details>


---

2. 한 개발자가 자주 변경되지 않는 웹사이트의 HTML, CSS, JavaScript 파일과 이미지를 저장하고 사용자에게 직접 제공하려고 합니다. 가장 비용 효율적인 스토리지 서비스는 무엇입니까?

A. Amazon EBS (Elastic Block Store)

B. Amazon EFS (Elastic File System)

C. Amazon S3 (Simple Storage Service)

D. Amazon RDS (Relational Database Service)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

설명:

<b>C (정답):</b> **Amazon S3**는 정적 웹사이트 호스팅, 이미지, 동영상 등 모든 유형의 파일을 저렴한 비용으로 저장하고 제공하는 데 최적화된 객체 스토리지 서비스입니다.

<b>A (오답):</b> Amazon EBS는 EC2 인스턴스에 연결하여 사용하는 가상 하드 디스크입니다.

<b>B (오답):</b> Amazon EFS는 여러 EC2 인스턴스에서 공유하는 파일 시스템으로, 단순 파일 저장에는 S3보다 비용이 비쌉니다.

</details>


---

3. 한 조직에 여러 명의 개발자가 있으며, 이들 모두에게 S3 버킷에 대한 읽기 전용 액세스 권한을 부여하려고 합니다. 가장 효율적인 관리 방법은 무엇입니까?

A. 각 개발자에게 개별적으로 인라인 정책을 할당합니다.

B. 모든 개발자를 위한 단일 IAM 역할을 생성합니다.

C. '개발자' IAM 그룹을 생성하고, 그룹에 정책을 연결한 후 사용자를 추가합니다.

D. AWS Organizations를 사용하여 정책을 적용합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

설명:

<b>C (정답):</b> 여러 사용자에게 동일한 권한을 부여할 때는 **IAM 그룹**을 사용하는 것이 가장 효율적이고 권장되는 모범 사례입니다. 그룹에 정책을 한 번만 연결하면, 해당 그룹에 속한 모든 사용자가 동일한 권한을 상속받습니다.

<b>A (오답):</b> 개별적으로 정책을 할당하는 것은 사용자가 많아질수록 관리가 복잡해지고 실수가 발생하기 쉽습니다.

<b>D (오답):</b> AWS Organizations는 여러 AWS '계정'을 관리하는 서비스이지, 한 계정 내의 '사용자'를 관리하는 주된 도구가 아닙니다.

</details>


---

4. 새로운 프로젝트를 시작하기 전에, 특정 구성의 EC2 인스턴스 10대와 RDS 데이터베이스를 1년간 사용할 경우의 예상 월별 비용을 산출하고 싶습니다. 어떤 AWS 도구를 사용해야 할까요?

A. AWS Cost Explorer

B. AWS Budgets

C. AWS Trusted Advisor

D. AWS Pricing Calculator

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

설명:

<b>D (정답):</b> **AWS Pricing Calculator(요금 계산기)**는 AWS 서비스를 사용하기 '전'에, 원하는 구성에 대한 예상 비용을 '견적' 내는 데 사용되는 웹 기반 도구입니다.

<b>A (오답):</b> AWS Cost Explorer는 이미 발생한 과거의 비용을 시각화하고 '분석'하는 도구입니다.

<b>B (오답):</b> AWS Budgets는 설정한 예산을 초과할 것 같을 때 '알림'을 보내는 서비스입니다.

</details>


---

5. 다음 중 AWS 공동 책임 모델에 따라 AWS의 책임에 해당하는 것은 무엇입니까? (2개 선택)

A. 고객 데이터 암호화

B. AWS 글로벌 인프라의 물리적 보안

C. EC2 인스턴스의 게스트 운영체제(OS) 관리

D. IAM 사용자의 암호 정책 설정

E. 하드웨어 및 하이퍼바이저 유지 관리

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B, E</b>

설명:

<b>B (정답):</b> 데이터 센터, 서버, 네트워킹 장비 등 AWS 글로벌 인프라의 **물리적 보안**은 전적으로 AWS의 책임입니다.

<b>E (정답):</b> 서버 **하드웨어**와 그 위에서 가상화를 실행하는 **하이퍼바이저**의 보안 및 유지 관리는 AWS가 책임지는 '클라우드 자체'의 보안 영역입니다.

<b>A, C, D (오답):</b> 데이터 암호화, 게스트 OS 관리, IAM 정책 설정은 모두 '클라우드 안'의 보안 영역으로, 전적으로 고객의 책임입니다.

</details>


---

6. 소셜 미디어 애플리케이션의 사용자 프로필, 친구 목록과 같은 데이터를 저장하려고 합니다. 데이터 모델이 유연하고, 어떤 규모에서든 한 자릿수 밀리초의 매우 빠른 읽기/쓰기 성능이 요구됩니다. 어떤 데이터베이스 서비스가 가장 적합합니까?

A. Amazon Redshift

B. Amazon RDS

C. Amazon DynamoDB

D. Amazon ElastiCache

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

설명:

<b>C (정답):</b> **"유연한 데이터 모델", "초고속 성능", "어떤 규모에서든"** 이라는 키워드는 NoSQL 데이터베이스인 **Amazon DynamoDB**의 핵심적인 특징입니다. DynamoDB는 이러한 요구사항을 가진 대규모 애플리케이션을 위해 설계되었습니다.

<b>B (오답):</b> Amazon RDS는 관계형 데이터베이스로, 스키마가 엄격하고 수평적 확장에 한계가 있습니다.

<b>A (오답):</b> Amazon Redshift는 데이터 분석 및 웨어하우징을 위한 서비스입니다.

</details>


---

7. 한 회사가 전 세계 사용자들에게 정적 및 동적 콘텐츠를 낮은 지연 시간으로 제공하여 웹사이트 로딩 속도를 개선하려고 합니다. 어떤 서비스를 사용해야 할까요?

A. AWS Global Accelerator

B. Amazon CloudFront

C. Amazon S3 전송 가속화

D. Amazon Route 53

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

설명:

<b>B (정답):</b> **"콘텐츠"**를 전 세계 사용자에게 **"낮은 지연 시간"**으로 제공하는 가장 대표적인 서비스는 **CDN(콘텐츠 전송 네트워크)인 Amazon CloudFront**입니다. 엣지 로케이션에 콘텐츠를 캐싱하여 사용자에게 가장 가까운 곳에서 전달합니다.

<b>A (오답):</b> AWS Global Accelerator는 네트워크 경로 자체를 최적화하는 서비스로, 콘텐츠 캐싱 기능은 없습니다.

<b>C (오답):</b> S3 전송 가속화는 S3 버킷으로의 업로드/다운로드 속도를 개선하는 기능입니다.

</details>


---

8. AWS Well-Architected Framework의 신뢰성(Reliability) 원칙을 가장 잘 설명하는 것은 무엇입니까?

A. 불필요한 비용을 제거하고 가장 적절한 리소스를 사용하는 능력

B. 시스템 및 고객 데이터를 보호하는 능력

C. 수요 변화에 맞춰 컴퓨팅 리소스를 효율적으로 사용하는 능력

D. 장애 발생 시 자동으로 복구하고, 수요를 충족하도록 리소스를 동적으로 확보하는 능력

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

설명:

<b>D (정답):</b> **신뢰성** 원칙의 핵심은 장애 상황에 대한 대응입니다. 장애가 발생했을 때 **자동으로 복구**하고, 리소스 수요를 동적으로 처리(예: Auto Scaling)하여 서비스 중단을 방지하는 능력을 의미합니다.

<b>A (오답):</b> 이것은 비용 최적화 원칙입니다.

<b>B (오답):</b> 이것은 보안 원칙입니다.

<b>C (오답):</b> 이것은 성능 효율성 원칙입니다.

</details>


---

9. 다음 중 온프레미스 데이터 센터와 AWS VPC를 공용 인터넷을 통해 안전하게 연결하는 데 사용되는 서비스는 무엇입니까?

A. VPC Peering

B. AWS Direct Connect

C. AWS Site-to-Site VPN

D. 인터넷 게이트웨이

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

설명:

<b>C (정답):</b> **AWS Site-to-Site VPN**은 **'공용 인터넷'**을 통해 암호화된 터널을 만들어 온프레미스 네트워크와 AWS VPC를 안전하게 연결하는 서비스입니다.

<b>B (오답):</b> AWS Direct Connect는 공용 인터넷이 아닌, 전용 사설 회선을 통해 연결합니다.

<b>D (오답):</b> 인터넷 게이트웨이는 VPC가 인터넷과 통신하게 해주는 '출입문' 역할입니다.

</details>


---

10. "최소 권한의 원칙(Principle of Least Privilege)"은 무엇을 의미합니까?

A. 모든 사용자에게 관리자 권한을 부여하는 것

B. 사용자가 작업을 수행하는 데 필요한 최소한의 권한만 부여하는 것

C. 모든 AWS 서비스에 대한 접근을 기본적으로 허용하는 것

D. 루트 사용자만 모든 작업을 수행하도록 하는 것

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

설명:

<b>B (정답):</b> **최소 권한의 원칙**은 IAM의 가장 기본이 되는 보안 모범 사례로, 사용자가 자신의 업무를 수행하는 데 **반드시 필요한 최소한의 권한**만 부여하여 보안 사고의 위험을 줄이는 것을 목표로 합니다.

</details>


---

11. 한 회사가 다음 분기 재무 보고서 작성을 위해 3시간 동안 대규모 데이터 분석 작업을 실행해야 합니다. 이 작업은 중단 없이 완료되어야 합니다. 가장 적합한 EC2 구매 옵션은 무엇입니까?

A. 스팟 인스턴스

B. 예약 인스턴스

C. 온디맨드 인스턴스

D. Savings Plans

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> "단기적"이고 "중단 없이" 실행해야 하는 예측 불가능한 워크로드에는 **온디맨드 인스턴스**가 가장 적합합니다. 약정 없이 사용한 만큼만 비용을 지불하며, AWS가 임의로 중단시키지 않습니다.

<br>

<b>A (오답):</b> 스팟 인스턴스는 저렴하지만 언제든지 중단될 수 있어 요구사항에 맞지 않습니다.

<br>

<b>B, D (오답):</b> 예약 인스턴스와 Savings Plans는 1~3년의 장기 약정을 통해 할인을 받는 모델로, 3시간 사용에는 부적합합니다.

</details>


---

12. 개발자가 소스 코드만 업로드하면, AWS가 용량 프로비저닝, 로드 밸런싱, 오토 스케일링, 애플리케이션 상태 모니터링을 포함한 환경을 자동으로 처리해주는 서비스는 무엇입니까?

A. AWS Lambda

B. AWS CloudFormation

C. AWS Elastic Beanstalk

D. Amazon EC2

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> 개발자가 인프라 걱정 없이 **"코드만 업로드하면"** 웹 애플리케이션 환경 전체를 **자동으로 구축하고 배포**해주는 PaaS(Platform as a Service)는 **AWS Elastic Beanstalk**입니다.

<br>

<b>B (오답):</b> AWS CloudFormation은 개발자가 템플릿 코드를 직접 작성하여 인프라를 정의해야 하는 IaC(Infrastructure as Code) 서비스입니다.

</details>


---

13. AWS 환경의 보안을 강화하기 위해, SQL 인젝션이나 크로스 사이트 스크립팅과 같은 일반적인 웹 공격으로부터 웹 애플리케이션을 보호하고 싶습니다. 어떤 서비스를 사용해야 할까요?

A. AWS Shield

B. 네트워크 ACL (NACL)

C. 보안 그룹

D. AWS WAF

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> SQL 인젝션, 크로스 사이트 스크립팅과 같은 **웹 애플리케이션 계층(Layer 7)의 공격**을 탐지하고 차단하는 웹 방화벽 서비스는 **AWS WAF(Web Application Firewall)**입니다.

<br>

<b>A (오답):</b> AWS Shield는 대규모 트래픽을 이용한 DDoS 공격(Layer 3/4)을 방어하는 서비스입니다.

</details>


---

14. 한 관리자가 특정 S3 버킷이 어젯밤 삭제된 것을 발견했습니다. 어떤 사용자가 이 작업을 수행했는지 확인하기 위해 가장 먼저 확인해야 할 서비스는 무엇입니까?

A. Amazon CloudWatch

B. AWS Trusted Advisor

C. AWS CloudTrail

D. VPC 흐름 로그

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **AWS CloudTrail**은 계정 내에서 발생한 모든 API 호출(예: S3 버킷 생성/삭제, EC2 인스턴스 시작/종료 등)에 대한 기록을 남깁니다. **"누가, 언제, 무엇을 했는지"** 추적하는 데 사용되는 핵심 감사 서비스입니다.

<br>

<b>A (오답):</b> Amazon CloudWatch는 리소스의 성능 지표와 로그를 모니터링합니다.

</details>


---

15. 여러 EC2 인스턴스가 동시에 접근하여 데이터를 읽고 쓸 수 있는 공유 파일 시스템이 필요합니다. 리눅스 기반 인스턴스에서 사용할 NFS(Network File System) 프로토콜을 지원하는 완전 관리형 서비스는 무엇입니까?

A. Amazon S3

B. Amazon EBS

C. 인스턴스 스토어

D. Amazon EFS

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> **"여러 EC2 인스턴스가 동시에 접근"**하는 **"공유 파일 시스템"**은 **Amazon EFS(Elastic File System)**의 핵심적인 사용 사례입니다. NFS 프로토콜을 지원하며, 여러 인스턴스가 동시에 마운트하여 사용할 수 있습니다.

<br>

<b>B (오답):</b> Amazon EBS는 하나의 EC2 인스턴스에만 연결하여 사용할 수 있습니다.

</details>


---

16. 다음 중 AWS Support 플랜에 대한 설명으로 올바른 것은 무엇입니까?

A. 모든 플랜은 24x7 전화, 이메일, 채팅 지원을 제공합니다.

B. Basic 플랜은 기술 지원 케이스를 열 수 있습니다.

C. Enterprise 플랜은 전담 기술 계정 관리자(TAM)를 제공합니다.

D. Developer 플랜은 15분 이내의 응답 시간을 보장합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **Enterprise Support 플랜**의 가장 큰 혜택 중 하나는 고객의 AWS 환경에 대해 사전 예방적인 기술 자문을 제공하는 **전담 기술 계정 관리자(TAM)**가 배정된다는 것입니다.

<br>

<b>A (오답):</b> 24x7 기술 지원은 Business 플랜 이상부터 제공됩니다.

<br>

<b>B (오답):</b> Basic 플랜은 기술 지원 케이스를 열 수 없으며, 계정 및 결제 관련 문의만 가능합니다.

<br>

<b>D (오답):</b> Developer 플랜의 응답 시간은 업무 시간 기준 12시간 또는 24시간입니다.

</details>


---

17. 사용자가 업로드하는 비디오를 트랜스코딩하는 것과 같이 시간이 오래 걸리는 백그라운드 작업을 처리하려고 합니다. 작업 요청을 순서대로 안정적으로 처리하고, 처리 시스템과 요청 시스템을 분리(디커플링)하고 싶습니다. 어떤 서비스가 가장 적합합니까?

A. Amazon SNS

B. Amazon SQS

C. Amazon Kinesis

D. AWS Lambda

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **Amazon SQS(Simple Queue Service)**는 메시지(작업 요청)를 큐에 저장해두고, 처리 시스템이 가져가서 처리하도록 하여 두 시스템을 **분리(디커플링)**하는 데 사용됩니다. 이를 통해 한쪽 시스템에 장애가 발생해도 다른 쪽에 영향을 주지 않으며, 작업을 안정적으로 처리할 수 있습니다.

<br>

<b>A (오답):</b> Amazon SNS는 하나의 메시지를 여러 구독자에게 동시에 전달(Fan-out)하는 데 사용됩니다.

</details>


---

18. 도메인 이름(예: www.example.com)을 EC2 인스턴스의 IP 주소나 로드 밸런서로 라우팅하는 데 사용되는 서비스는 무엇입니까?

A. Amazon VPC

B. Amazon Route 53

C. Amazon CloudFront

D. AWS Direct Connect

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **Amazon Route 53**은 AWS의 **DNS(도메인 이름 시스템)** 서비스입니다. 사용자가 웹 브라우저에 도메인 이름을 입력했을 때, 해당 도메인과 연결된 서버의 IP 주소로 안내(라우팅)하는 역할을 합니다.

<br>

<b>C (오답):</b> Amazon CloudFront는 콘텐츠를 캐싱하여 빠르게 전송하는 CDN 서비스입니다.

</details>


---

19. 다음 중 단일 장애점(Single Point of Failure)을 방지하여 고가용성을 확보하기 위한 가장 기본적인 전략은 무엇입니까?

A. 단일 가용 영역에 더 큰 EC2 인스턴스를 배포

B. 여러 리전에 걸쳐 리소스를 배포

C. 여러 가용 영역에 걸쳐 리소스를 배포

D. EBS 스냅샷을 정기적으로 생성

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **고가용성(High Availability)**의 핵심은 **다중 AZ(Multi-AZ)** 배포입니다. 하나의 가용 영역(데이터 센터)에 장애가 발생하더라도 다른 가용 영역에 있는 리소스가 서비스를 계속 이어갈 수 있도록 하여 단일 장애점을 제거합니다.

<br>

<b>B (오답):</b> 여러 리전에 배포하는 것은 주로 재해 복구(Disaster Recovery) 전략에 해당합니다.

</details>


---

20. 월별 AWS 청구서의 예상 요금이 설정한 임계값(예: 100달러)을 초과할 때 이메일 알림을 받고 싶습니다. 어떤 기능을 사용해야 할까요?

A. AWS Cost Explorer

B. AWS Trusted Advisor

C. Amazon CloudWatch 결제 경보

D. AWS Organizations

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **Amazon CloudWatch**는 리소스 성능 지표뿐만 아니라 **예상 청구 요금(EstimatedCharges)** 지표도 모니터링할 수 있습니다. 이 지표에 대해 경보를 설정하면, 예상 요금이 특정 금액을 초과했을 때 알림을 받을 수 있습니다. **AWS Budgets**도 비슷한 기능을 제공하며 더 정교한 설정이 가능하지만, CloudWatch 결제 경보는 가장 기본적인 알림 기능입니다.

</details>


---

21. 다음 중 AWS 공동 책임 모델에 따라 고객의 책임에 해당하는 것은 무엇입니까? (2개 선택)

A. Amazon S3에 저장된 데이터의 암호화 설정

B. AWS 데이터 센터의 전원 및 냉각 시스템 관리

C. 보안 그룹 및 네트워크 ACL 규칙 구성

D. AWS 리전 및 가용 영역의 물리적 위치 선정

E. 하이퍼바이저 수준의 보안

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>A, C</b>

<br>

설명:

<br>

<b>A (정답):</b> S3에 저장하는 **데이터를 암호화**할지 여부와 방법을 결정하고 설정하는 것은 "클라우드 안의 보안" 영역으로, 전적으로 **고객의 책임**입니다.

<br>

<b>C (정답):</b> VPC 내의 네트워크 트래픽을 제어하는 **보안 그룹과 NACL의 규칙을 구성**하고 관리하는 것 역시 **고객의 책임**입니다.

<br>

<b>B, D, E (오답):</b> 물리적 인프라(전원, 냉각, 위치)와 가상화를 위한 하이퍼바이저 보안은 모두 "클라우드 자체"의 보안 영역으로, AWS의 책임입니다.

</details>


---

22. 한 회사가 EC2 인스턴스의 CPU 사용률이 80%를 5분간 초과하면 자동으로 새로운 인스턴스를 추가하여 부하를 분산시키려고 합니다. 어떤 서비스를 사용해야 할까요?

A. Elastic Load Balancing

B. Amazon CloudWatch

C. AWS Auto Scaling

D. AWS Lambda

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> 특정 조건(예: CPU 사용률)에 따라 **EC2 인스턴스 수를 자동으로 늘리거나 줄이는 것**은 **AWS Auto Scaling**의 핵심 기능입니다. 이를 통해 탄력성과 가용성을 확보할 수 있습니다.

<br>

<b>A (오답):</b> Elastic Load Balancing은 인스턴스 수를 조절하는 것이 아니라, 들어오는 트래픽을 여러 인스턴스로 분산시키는 역할을 합니다.

<br>

<b>B (오답):</b> Amazon CloudWatch는 CPU 사용률을 모니터링하고 경보를 발생시켜 Auto Scaling을 트리거하는 역할을 하지만, 직접 인스턴스를 추가하지는 않습니다.

</details>


---

23. 자주 액세스하지는 않지만, 필요할 때 즉시(밀리초 단위) 검색해야 하는 중요한 데이터를 장기간 보관하려고 합니다. S3 Standard보다 저렴한 스토리지 비용을 원할 때 가장 적합한 S3 스토리지 클래스는 무엇입니까?

A. S3 Standard-IA

B. S3 One Zone-IA

C. S3 Glacier Instant Retrieval

D. S3 Glacier Flexible Retrieval

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>A</b>

<br>

설명:

<br>

<b>A (정답):</b> **S3 Standard-IA(Infrequent Access)**는 이름 그대로 **자주 액세스하지 않는 데이터**를 S3 Standard보다 저렴한 비용으로 저장하면서도, 필요할 때는 **빠른 속도로 접근**할 수 있도록 설계된 스토리지 클래스입니다. 데이터는 최소 3개의 가용 영역에 저장되어 높은 내구성과 가용성을 보장합니다.

<br>

<b>B (오답):</b> S3 One Zone-IA는 단일 가용 영역에만 데이터를 저장하므로, AZ 장애 시 데이터가 손실될 수 있어 중요 데이터 보관에는 적합하지 않습니다.

<br>

<b>C, D (오답):</b> Glacier 계열은 '아카이빙'을 위한 스토리지로, IA 클래스보다 검색 비용이 더 비싸거나 검색 시간이 더 오래 걸립니다.

</details>


---

24. VPC 내의 특정 서브넷으로 들어오고 나가는 트래픽을 제어하는 상태 비저장(Stateless) 방화벽 역할을 하는 것은 무엇입니까?

A. 보안 그룹

B. 인터넷 게이트웨이

C. 라우팅 테이블

D. 네트워크 ACL (NACL)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> **네트워크 ACL(NACL)**은 **서브넷 수준**에서 작동하며, 인바운드와 아웃바운드 규칙을 각각 설정해야 하는 **상태 비저장(Stateless)** 방화벽입니다.

<br>

<b>A (오답):</b> 보안 그룹은 인스턴스 수준에서 작동하며, 들어온 요청에 대한 응답은 자동으로 허용되는 상태 저장(Stateful) 방화벽입니다.

</details>


---

25. AWS Marketplace는 무엇을 제공합니까?

A. AWS 리소스 관리를 위한 무료 스크립트 모음

B. 중고 EC2 인스턴스를 저렴하게 구매할 수 있는 시장

C. AWS에서 실행할 수 있는 타사 소프트웨어 및 서비스를 찾고 구매하는 디지털 카탈로그

D. AWS 전문가와 프로젝트를 위해 연결해주는 프리랜서 플랫폼

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **AWS Marketplace**는 보안, 네트워킹, 스토리지 등 다양한 카테고리의 **타사(3rd-party) 소프트웨어**를 쉽게 찾고, 구매하며, AWS 환경에 배포할 수 있도록 지원하는 온라인 스토어입니다.

</details>


---

26. 다음 중 객체 스토리지(Object Storage)의 특징으로 올바른 것은 무엇입니까?

A. EC2 인스턴스의 부팅 볼륨으로 사용된다.

B. 파일을 폴더와 하위 폴더 계층 구조로 저장한다.

C. 데이터를 고유한 ID를 가진 객체로 저장하며, 파일과 메타데이터를 포함한다.

D. 여러 EC2 인스턴스에서 동시에 마운트하여 사용할 수 있다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **객체 스토리지(예: Amazon S3)**는 데이터를 파일 시스템의 계층 구조가 아닌, 고유한 ID(Key)를 가진 평평한 구조의 **객체(Object)**로 저장합니다. 각 객체는 데이터 자체와 함께 데이터에 대한 설명(메타데이터)을 포함합니다.

<br>

<b>A (오답):</b> EC2 부팅 볼륨으로는 블록 스토리지인 EBS를 사용합니다.

<br>

<b>B (오답):</b> 폴더 계층 구조는 파일 스토리지(예: EFS)의 특징입니다.

<br>

<b>D (오답):</b> 여러 EC2에서 동시에 마운트하는 것은 파일 스토리지(EFS)의 특징입니다.

</details>


---

27. EC2 인스턴스가 S3 버킷에 안전하게 접근할 수 있도록 자격 증명을 부여하려고 합니다. 액세스 키를 코드에 하드코딩하는 대신 사용할 수 있는 가장 안전하고 권장되는 방법은 무엇입니까?

A. 루트 사용자 자격 증명을 사용합니다.

B. EC2 인스턴스에 IAM 역할을 연결합니다.

C. 모든 권한을 가진 새로운 IAM 사용자를 생성합니다.

D. 보안 그룹을 사용하여 접근을 허용합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> AWS 리소스(예: EC2 인스턴스)가 다른 AWS 서비스(예: S3)에 접근해야 할 때, **IAM 역할(Role)**을 사용하는 것이 가장 안전하고 권장되는 모범 사례입니다. IAM 역할을 통해 임시 보안 자격 증명이 자동으로 발급되고 관리되므로, 액세스 키와 같은 장기 자격 증명을 코드에 노출할 필요가 없습니다.

<br>

<b>A, C (오답):</b> 루트 사용자나 과도한 권한을 가진 사용자의 자격 증명을 사용하는 것은 보안상 매우 위험합니다.

<br>

<b>D (오답):</b> 보안 그룹은 네트워크 트래픽을 제어하는 방화벽이며, IAM 권한을 부여하는 기능이 없습니다.

</details>


---

28. AWS 클라우드 채택 프레임워크(AWS CAF)의 6가지 관점(Perspective)에 포함되지 않는 것은 무엇입니까?

A. 비즈니스 (Business)

B. 인력 (People)

C. 거버넌스 (Governance)

D. 마케팅 (Marketing)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> **AWS CAF**의 6가지 관점은 **비즈니스, 인력, 거버넌스, 플랫폼, 보안, 운영**입니다. 마케팅은 이에 포함되지 않습니다.

</details>


---

29. 재해 복구(Disaster Recovery) 전략의 일환으로, 한 AWS 리전 전체에 장애가 발생하더라도 다른 리전에서 서비스를 신속하게 복구할 수 있도록 준비하려고 합니다. 이를 위해 가장 중요한 것은 무엇입니까?

A. 여러 가용 영역에 리소스를 분산하는 것

B. 다른 리전에 데이터를 백업하거나 복제하는 것

C. 더 큰 EC2 인스턴스 타입을 사용하는 것

D. AWS Shield Advanced를 구독하는 것

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **재해 복구(DR)**는 지진이나 홍수와 같이 **리전 전체에 영향을 미치는 대규모 재해**에 대비하는 것입니다. 따라서 서비스와 데이터를 **다른 리전**에 백업하거나 복제해 두는 것이 가장 핵심적인 전략입니다.

<br>

<b>A (오답):</b> 여러 가용 영역에 분산하는 것은 한 리전 내에서의 **고가용성(HA)** 전략입니다. 리전 전체에 장애가 발생하면 효과가 없습니다.

</details>


---

30. AWS 환경의 보안을 지속적으로 모니터링하여 악의적인 활동이나 무단 동작을 탐지하는 지능형 위협 탐지 서비스는 무엇입니까?

A. Amazon Inspector

B. Amazon GuardDuty

C. AWS WAF

D. AWS Secrets Manager

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **Amazon GuardDuty**는 VPC 흐름 로그, CloudTrail 로그, DNS 로그와 같은 데이터 소스를 머신러닝을 통해 분석하여, 계정 내의 **비정상적인 활동이나 잠재적인 위협**을 자동으로 탐지하고 경고를 생성하는 **지능형 위협 탐지** 서비스입니다.

<br>

<b>A (오답):</b> Amazon Inspector는 EC2 인스턴스 내의 알려진 소프트웨어 취약점을 스캔합니다.

</details>


---

31. 다음 중 데이터 웨어하우징 및 비즈니스 인텔리전스(BI) 워크로드를 위해 설계된 페타바이트 규모의 분석 데이터베이스 서비스는 무엇입니까?

A. Amazon RDS

B. Amazon DynamoDB

C. Amazon Redshift

D. Amazon DocumentDB

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **Amazon Redshift**는 대규모 데이터 세트에 대해 복잡한 분석 쿼리를 빠르게 실행하도록 최적화된 **데이터 웨어하우스(DW)** 서비스입니다. BI 도구와 연동하여 보고서나 대시보드를 만드는 데 주로 사용됩니다.

<br>

<b>A, B, D (오답):</b> 이들은 운영 워크로드를 위한 데이터베이스(OLTP)이며, 대규모 분석(OLAP)에는 적합하지 않습니다.

</details>


---

32. AWS의 모든 서비스는 API를 통해 제어할 수 있습니다. 다음 중 AWS 서비스와 프로그래밍 방식으로 상호 작용하는 방법이 아닌 것은 무엇입니까?

A. AWS 관리 콘솔

B. AWS CLI (명령줄 인터페이스)

C. AWS SDK (소프트웨어 개발 키트)

D. AWS CloudFormation

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>A</b>

<br>

설명:

<br>

<b>A (정답):</b> **AWS 관리 콘솔**은 사용자가 웹 브라우저를 통해 클릭, 드래그 등 그래픽 인터페이스(GUI)를 사용하여 AWS와 상호 작용하는 방식입니다. 이는 '프로그래밍 방식'이 아닙니다.

<br>

<b>B, C, D (오답):</b> CLI, SDK, CloudFormation(IaC)은 모두 코드를 통해 AWS 리소스를 생성하고 관리하는 '프로그래밍 방식'의 상호 작용 방법입니다.

</details>


---

33. 한 회사에서 여러 AWS 계정을 중앙에서 관리하고, 모든 계정의 비용을 하나의 청구서로 통합하며, 서비스 제어 정책(SCP)을 사용하여 특정 서비스 사용을 제한하고 싶어합니다. 어떤 서비스를 사용해야 할까요?

A. AWS Control Tower

B. AWS IAM

C. AWS Organizations

D. AWS License Manager

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **AWS Organizations**는 **여러 AWS 계정**을 조직적으로 관리하기 위한 서비스입니다. **통합 결제(Consolidated Billing)**를 통해 비용을 관리하고, **서비스 제어 정책(SCP)**을 사용하여 모든 하위 계정에 대한 권한 가드레일을 설정하는 핵심 기능을 제공합니다.

<br>

<b>B (오답):</b> AWS IAM은 단일 계정 내의 사용자 및 권한을 관리합니다.

</details>


---

34. 다음 중 서버리스(Serverless) 컴퓨팅 서비스의 주요 이점은 무엇입니까? (2개 선택)

A. 사용자가 운영체제에 대한 완전한 제어권을 가짐

B. 서버 프로비저닝이나 관리가 필요 없음

C. 코드가 실행되지 않을 때는 비용이 거의 발생하지 않음

D. 모든 유형의 워크로드에 가장 적합함

E. 고정된 월별 요금으로 비용 예측이 쉬움

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B, C</b>

<br>

설명:

<br>

<b>B (정답):</b> 서버리스의 가장 큰 특징은 이름 그대로 **서버를 프로비저닝하거나 패치, 관리할 필요가 없다**는 것입니다.

<br>

<b>C (정답):</b> 코드가 요청이나 이벤트에 의해 실행될 때만 비용이 발생하므로, **유휴 시간에는 비용이 거의 들지 않아** 비용 효율적입니다.

<br>

<b>A (오답):</b> 서버리스는 서버 관리를 추상화하므로 사용자는 OS에 접근할 수 없습니다. OS 제어가 필요하면 EC2를 사용해야 합니다.

</details>


---

35. EC2 인스턴스와 함께 사용하는 스토리지 중, 인스턴스가 중지되거나 종료되면 데이터가 삭제되는 임시(휘발성) 스토리지 유형은 무엇입니까?

A. Amazon EBS

B. Amazon EFS

C. Amazon S3

D. 인스턴스 스토어

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> **인스턴스 스토어**는 EC2 호스트 컴퓨터에 물리적으로 연결된 스토리지로, 매우 빠른 성능을 제공하지만 **임시적(휘발성)**입니다. EC2 인스턴스가 중지, 종료, 또는 하드웨어 장애 시 저장된 데이터가 모두 사라집니다.

<br>

<b>A, B (오답):</b> EBS와 EFS는 영구적인 스토리지로, 인스턴스가 종료되어도 데이터는 보존됩니다.

</details>


---

36. Enterprise Support 플랜을 사용하는 고객이 청구 및 계정 관련 문의에 대해 전문가의 지원을 받고 싶을 때 이용할 수 있는 전담팀은 무엇입니까?

A. AWS Trusted Advisor

B. 기술 계정 관리자 (TAM)

C. AWS 컨시어지 팀

D. AWS Professional Services

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **AWS 컨시어지 팀**은 **Enterprise Support 플랜 고객 전용**으로, **청구 및 계정 관련 문의**를 전문적으로 신속하게 처리해주는 전문가 팀입니다.

<br>

<b>B (오답):</b> 기술 계정 관리자(TAM)는 기술적인 조언과 아키텍처 검토를 담당하는 기술 전문가입니다.

</details>


---

37. 데이터베이스의 읽기 성능을 향상시키기 위해, 자주 요청되는 쿼리 결과를 메모리에 캐싱하는 데 사용되는 서비스는 무엇입니까?

A. Amazon SQS

B. Amazon ElastiCache

C. Amazon Kinesis

D. AWS Storage Gateway

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **Amazon ElastiCache**는 Redis나 Memcached와 같은 인기 있는 오픈 소스 **인메모리 캐싱** 엔진을 완전 관리형으로 제공하는 서비스입니다. 데이터베이스 앞에서 자주 사용되는 데이터를 캐시에 저장하여 데이터베이스 부하를 줄이고 애플리케이션의 읽기 성능을 크게 향상시킵니다.

</details>


---

38. 한 사용자가 자신의 AWS 환경이 AWS 모범 사례를 잘 따르고 있는지 확인하고 싶어합니다. 비용 최적화, 보안, 내결함성 등에 대한 자동화된 점검 및 권장 사항을 제공하는 서비스는 무엇입니까?

A. AWS Well-Architected Tool

B. AWS Trusted Advisor

C. Amazon Inspector

D. AWS Config

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **AWS Trusted Advisor**는 고객의 AWS 환경을 자동으로 점검하여 **비용 최적화, 보안, 성능, 내결함성, 서비스 한도** 등 5가지 영역에 대한 모범 사례 **권장 사항**을 제공하는 개인화된 컨설턴트 서비스입니다.

<br>

<b>A (오답):</b> AWS Well-Architected Tool은 사용자가 직접 질문에 답하며 자신의 아키텍처를 프레임워크에 비추어 검토하는 셀프 서비스 도구입니다.

</details>


---

39. 대규모 데이터를 물리적으로 AWS로 전송하기 위한 페타바이트 규모의 휴대용 스토리지 디바이스는 무엇입니까?

A. AWS Snowmobile

B. AWS Snowball Edge

C. AWS Storage Gateway

D. AWS DataSync

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **AWS Snowball**은 **페타바이트(PB) 규모**의 데이터를 AWS로 전송하기 위해 사용되는 물리적인 휴대용 스토리지 디바이스입니다. Snowball Edge 모델은 스토리지 외에 컴퓨팅 기능도 제공합니다.

<br>

<b>A (오답):</b> AWS Snowmobile은 엑사바이트(EB) 규모의 데이터를 전송하기 위한 컨테이너 트럭 크기의 훨씬 더 큰 서비스입니다.

</details>


---

40. 다음 중 AWS 리소스에 태그(Tag)를 지정하는 주요 목적은 무엇입니까?

A. 리소스의 성능을 향상시키기 위해

B. 리소스를 그룹화하고 비용을 추적 및 할당하기 위해

C. 리소스에 대한 자동 백업을 활성화하기 위해

D. 리소스의 가용성을 높이기 위해

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **태그**는 키-값 쌍으로 이루어진 메타데이터 레이블입니다. 태그를 사용하여 리소스를 프로젝트, 부서, 환경 등으로 **그룹화**하고, AWS 비용 및 사용 보고서에서 태그를 활성화하여 **비용을 추적하고 할당**하는 것이 주요 목적입니다.

</details>


---

41. 다음 중 AWS에서 제공하는 완전 관리형 관계형 데이터베이스(RDS) 엔진이 아닌 것은 무엇입니까?

A. MySQL

B. PostgreSQL

C. Amazon Aurora

D. MongoDB

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> **MongoDB**는 문서 기반의 **NoSQL** 데이터베이스이며, Amazon RDS에서 제공하는 관계형 데이터베이스 엔진이 아닙니다. (AWS에서는 DocumentDB라는 서비스가 MongoDB와 호환됩니다.)

<br>

<b>A, B, C (오답):</b> MySQL, PostgreSQL, Amazon Aurora는 모두 Amazon RDS에서 지원하는 대표적인 관계형 데이터베이스 엔진입니다.

</details>


---

42. 하나의 VPC에 있는 EC2 인스턴스가 다른 VPC에 있는 EC2 인스턴스와 비공개적으로 통신할 수 있도록 두 VPC를 연결하는 네트워킹 기능은 무엇입니까?

A. 인터넷 게이트웨이

B. VPC 엔드포인트

C. VPC 피어링

D. NAT 게이트웨이

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **VPC 피어링**은 두 개의 VPC를 1:1로 연결하여, 마치 같은 네트워크에 있는 것처럼 **비공개적으로 통신**할 수 있게 해주는 네트워킹 기능입니다. 트래픽은 AWS의 백본 네트워크를 통해 전달되며 인터넷을 거치지 않습니다.

</details>


---

43. S3 버킷에 객체가 업로드될 때마다, 여러 구독자(Lambda 함수, SQS 큐, 이메일 등)에게 동시에 알림을 보내는 '팬아웃(Fan-out)' 아키텍처를 구현하는 데 가장 적합한 서비스는 무엇입니까?

A. Amazon SQS

B. Amazon Kinesis Data Streams

C. AWS Step Functions

D. Amazon SNS

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> **Amazon SNS(Simple Notification Service)**는 게시/구독(Pub/Sub) 모델을 기반으로 합니다. 하나의 주제(Topic)에 메시지를 게시하면, 해당 주제를 구독하는 **여러 엔드포인트(구독자)에게 동시에 메시지를 전달**하는 **팬아웃(Fan-out)** 패턴에 가장 적합합니다.

<br>

<b>A (오답):</b> Amazon SQS는 1:1 메시지 전달을 위한 큐 서비스입니다.

</details>


---

44. 암호, 데이터베이스 연결 문자열, API 키와 같은 보안 정보를 안전하게 저장하고, 수명 주기를 관리하며, 접근을 제어하는 데 사용되는 서비스는 무엇입니까?

A. AWS KMS (Key Management Service)

B. AWS Secrets Manager

C. AWS Certificate Manager

D. AWS IAM

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **AWS Secrets Manager**는 **데이터베이스 자격 증명, API 키와 같은 비밀 정보 자체**를 안전하게 저장하고, IAM 정책을 통해 접근을 제어하며, 데이터베이스 암호의 **자동 교체(Rotation)** 기능까지 제공하는 전문 서비스입니다.

<br>

<b>A (오답):</b> AWS KMS는 데이터를 암호화하는 데 사용되는 '암호화 키'를 관리하는 서비스이지, 비밀 정보 자체를 저장하는 서비스가 아닙니다.

</details>


---

45. 다음 중 '고가용성(High Availability)'을 가장 잘 설명하는 것은 무엇입니까?

A. 재해 발생 시 다른 리전에서 복구하는 능력

B. 구성 요소에 장애가 발생하더라도 최소한의 중단으로 계속 작동하는 시스템의 능력

C. 수요에 따라 리소스를 자동으로 확장하거나 축소하는 능력

D. 전 세계 사용자에게 낮은 지연 시간을 제공하는 능력

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **고가용성(HA)**은 시스템의 일부(예: 서버 한 대, 데이터 센터 하나)에 장애가 발생하더라도, 전체 서비스는 **중단 없이 계속해서 작동**할 수 있는 능력을 의미합니다. 다중 AZ 배포가 이를 달성하기 위한 핵심 전략입니다.

<br>

<b>A (오답):</b> 이것은 재해 복구(Disaster Recovery)입니다.

<br>

<b>C (오답):</b> 이것은 탄력성(Elasticity)입니다.

</details>


---

46. 클라우드로 마이그레이션할 때, 기존 애플리케이션을 거의 또는 전혀 변경하지 않고 그대로 AWS EC2 인스턴스로 옮기는 마이그레이션 전략은 무엇입니까?

A. 리팩토링 (Refactoring)

B. 리플랫포밍 (Replatforming)

C. 리호스팅 (Rehosting)

D. 재구매 (Repurchasing)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **리호스팅(Rehosting)**은 **'리프트 앤 시프트(Lift-and-Shift)'**라고도 불리며, 애플리케이션을 변경 없이 그대로 들어서 AWS 환경(주로 EC2)으로 옮기는 가장 빠르고 간단한 마이그레이션 전략입니다.

<br>

<b>B (오답):</b> 리플랫포밍은 데이터베이스를 RDS로 전환하는 것처럼, 클라우드 환경에 맞게 약간의 최적화를 수행하는 전략입니다.

</details>


---

47. AWS 리소스의 구성이 조직의 보안 및 규정 준수 정책을 따르는지 지속적으로 평가, 감사 및 검사하는 서비스는 무엇입니까?

A. AWS Config

B. AWS Artifact

C. AWS Security Hub

D. Amazon Macie

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>A</b>

<br>

설명:

<br>

<b>A (정답):</b> **AWS Config**는 AWS 리소스의 **구성을 지속적으로 모니터링하고 기록**하며, 정의된 규칙(예: 'S3 버킷은 공개되면 안 된다')에 따라 **구성의 규정 준수 여부를 평가**하는 서비스입니다.

<br>

<b>B (오답):</b> AWS Artifact는 AWS의 규정 준수 보고서를 다운로드하는 포털입니다.

<br>

<b>C (오답):</b> AWS Security Hub는 여러 보안 서비스의 결과를 통합하여 보여주는 대시보드입니다.

</details>


---

48. 한 회사가 3년 동안 안정적으로 사용할 것으로 예상되는 워크로드에 대해 EC2 비용을 크게 절감하고 싶어합니다. 이 회사는 특정 인스턴스 유형을 약정하는 대신, 시간당 특정 컴퓨팅 사용량(예: $10/시간)을 약정하여 유연하게 할인을 받고 싶어합니다. 가장 적합한 구매 옵션은 무엇입니까?

A. 스팟 인스턴스

B. 예약 인스턴스

C. Savings Plans

D. 전용 호스트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **Savings Plans**는 특정 인스턴스 유형에 묶이지 않고, **시간당 특정 컴퓨팅 사용량(USD/시간)**을 1년 또는 3년간 약정하여 할인을 받는 **유연한** 요금 모델입니다. 인스턴스 패밀리, 크기, 리전을 자유롭게 변경할 수 있는 장점이 있습니다.

<br>

<b>B (오답):</b> 예약 인스턴스는 특정 인스턴스 패밀리 및 리전에 약정이 묶이므로 유연성이 떨어집니다.

</details>


---

49. 여러 단계로 구성된 복잡한 워크플로우를 시각적으로 디자인하고, 각 단계를 안정적으로 조정하며, 오류 처리 및 재시도를 자동화하는 데 사용되는 서버리스 오케스트레이션 서비스는 무엇입니까?

A. Amazon SQS

B. AWS Step Functions

C. Amazon EventBridge

D. AWS Batch

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **AWS Step Functions**는 Lambda 함수, SQS, SNS 등 여러 AWS 서비스를 연결하여 **복잡한 워크플로우(상태 머신)를 시각적으로 구성하고 조정(오케스트레이션)**하는 서버리스 서비스입니다.

<br>

<b>C (오답):</b> Amazon EventBridge는 다양한 소스로부터 이벤트를 받아 정의된 규칙에 따라 대상을 호출하는 이벤트 버스 서비스입니다.

</details>


---

50. 다음 중 AWS 클라우드의 경제적 이점이 아닌 것은 무엇입니까?

A. 총 소유 비용(TCO) 감소

B. 고정된 초기 자본 지출 증가

C. 비즈니스 민첩성으로 인한 기회비용 감소

D. 규모의 경제를 통한 저렴한 요금

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답 - 이점이 아님):</b> AWS 클라우드의 핵심 경제적 이점은 서버 구매와 같은 막대한 초기 **자본 지출(고정 비용)을 없애고**, 사용한 만큼만 지불하는 **운영 비용(가변 비용)으로 전환**하는 것입니다. 따라서 고정 지출이 '증가'한다는 것은 틀린 설명입니다.

</details>


---

51. VPC 내 프라이빗 서브넷에 있는 EC2 인스턴스가 인터넷에서 직접 접근할 수는 없지만, 소프트웨어 업데이트 등을 위해 인터넷으로 나가는(아웃바운드) 연결은 가능하게 하려면 어떤 구성 요소가 필요합니까?

A. 인터넷 게이트웨이

B. NAT 게이트웨이

C. 가상 프라이빗 게이트웨이

D. VPC 엔드포인트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **NAT 게이트웨이**는 **프라이빗 서브넷**에 있는 리소스가 외부 인터넷으로 **아웃바운드 요청(예: 소프트웨어 패치 다운로드)**을 보낼 수 있게 해주면서, 외부 인터넷에서는 해당 리소스로 직접 접근(인바운드)할 수 없도록 막아주는 역할을 합니다.

<br>

<b>A (오답):</b> 인터넷 게이트웨이는 퍼블릭 서브넷이 인터넷과 양방향으로 통신할 수 있게 해줍니다.

</details>


---

52. 여러 리전에 걸쳐 있는 애플리케이션의 상태를 모니터링하고, DNS 수준에서 상태가 비정상적인 리전으로는 트래픽이 라우팅되지 않도록 자동으로 장애 조치(Failover)를 수행할 수 있는 서비스는 무엇입니까?

A. Elastic Load Balancing

B. AWS Auto Scaling

C. Amazon Route 53

D. Amazon CloudWatch

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **Amazon Route 53**은 단순한 DNS 서비스를 넘어, 엔드포인트에 대한 **상태 확인(Health Check)**을 수행하고, 특정 엔드포인트가 비정상이라고 판단되면 자동으로 트래픽을 다른 정상적인 엔드포인트로 전환하는 **DNS 장애 조치(Failover)** 기능을 제공합니다.

<br>

<b>A (오답):</b> ELB는 한 리전 내에서 여러 인스턴스로 트래픽을 분산합니다.

</details>


---

53. S3에 저장된 데이터에서 개인 식별 정보(PII)나 금융 정보와 같은 민감한 데이터를 자동으로 발견하고 분류하며 보호하는 데 도움이 되는 데이터 보안 서비스는 무엇입니까?

A. Amazon GuardDuty

B. Amazon Macie

C. Amazon Inspector

D. AWS Secrets Manager

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **Amazon Macie**는 머신러닝을 사용하여 Amazon S3에 저장된 데이터에서 **개인 식별 정보(PII)와 같은 민감한 데이터를 자동으로 발견, 분류**하고, 데이터에 대한 보안 및 접근 제어 상태를 평가하여 알려주는 서비스입니다.

<br>

<b>A (오답):</b> GuardDuty는 계정 활동을 분석하여 위협을 탐지합니다.

<br>

<b>C (오답):</b> Inspector는 EC2의 소프트웨어 취약점을 점검합니다.

</details>


---

54. 사용하지 않는 IAM 자격 증명을 식별하거나, S3 버킷 권한을 공개로 설정하는 등의 보안 위험을 감지하여 권장 사항을 제공하는 AWS 서비스는 무엇입니까?

A. Amazon CloudWatch

B. AWS IAM Access Analyzer

C. AWS Trusted Advisor

D. AWS Security Hub

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **AWS Trusted Advisor**의 **보안** 점검 항목에는 공개적으로 접근 가능한 S3 버킷, IAM 액세스 키 순환, MFA 활성화 등 다양한 보안 모범 사례에 대한 검사가 포함되어 있으며, 이에 대한 **권장 사항**을 제공합니다.

<br>

<b>B (오답):</b> IAM Access Analyzer는 주로 외부 엔터티와 공유된 리소스를 식별하는 데 중점을 둡니다.

</details>


---

55. EC2 인스턴스에 대한 SSH(리눅스) 또는 RDP(윈도우) 접근을 제어하는 가상 방화벽 역할을 하는 것은 무엇입니까?

A. 네트워크 ACL

B. 보안 그룹

C. AWS WAF

D. AWS Firewall Manager

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **보안 그룹**은 **EC2 인스턴스** 수준에서 작동하는 상태 저장(Stateful) 방화벽입니다. 특정 포트(예: SSH용 22번, RDP용 3389번)에 대해 특정 IP 주소 범위의 접근을 허용하거나 거부하는 규칙을 설정하여 인스턴스를 보호합니다.

<br>

<b>A (오답):</b> 네트워크 ACL은 서브넷 수준에서 작동합니다.

</details>


---

56. AWS 클라우드에서 애플리케이션을 성공적으로 구축하고 운영하기 위한 아키텍처 모범 사례와 설계 원칙을 제공하는 것은 무엇입니까?

A. AWS 공동 책임 모델

B. AWS 클라우드 채택 프레임워크 (CAF)

C. AWS Well-Architected Framework

D. AWS Support 플랜

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **AWS Well-Architected Framework**는 AWS가 수년간의 경험을 바탕으로 정리한 **아키텍처 설계의 모범 사례 가이드**입니다. 6가지 원칙(운영 우수성, 보안, 신뢰성, 성능 효율성, 비용 최적화, 지속 가능성)을 통해 고객이 성공적인 클라우드 애플리케이션을 구축하도록 돕습니다.

</details>


---

57. 다음 중 AWS에서 데이터를 백업하고 복원하는 데 사용할 수 있는 서비스가 아닌 것은 무엇입니까?

A. Amazon S3

B. EBS 스냅샷

C. AWS Backup

D. AWS Cost Explorer

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> **AWS Cost Explorer**는 AWS 사용 **비용을 분석**하고 시각화하는 도구이며, 데이터 백업이나 복원 기능과는 전혀 관련이 없습니다.

<br>

<b>A, B, C (오답):</b> S3, EBS 스냅샷, AWS Backup은 모두 데이터를 백업하고 보존하는 데 사용되는 핵심 서비스입니다.

</details>


---

58. 어떤 사용자가 AWS 서비스 및 리소스와 상호 작용하기 위해 사용하는 이름과 암호 또는 액세스 키를 무엇이라고 합니까?

A. 정책 (Policy)

B. 역할 (Role)

C. 자격 증명 (Credentials)

D. 리소스 (Resource)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> 사용자를 인증하고 식별하는 데 사용되는 정보, 즉 **사용자 이름과 암호, 액세스 키 ID와 비밀 액세스 키** 등을 통칭하여 **자격 증명(Credentials)**이라고 부릅니다.

</details>


---

59. EC2 인스턴스에서 실행되는 애플리케이션의 성능 문제를 해결하기 위해, 코드의 어느 부분에서 병목 현상이 발생하는지 분석하고 성능 데이터를 수집하는 데 도움이 되는 서비스는 무엇입니까?

A. AWS X-Ray

B. AWS CodeDeploy

C. Amazon CloudWatch

D. AWS CloudTrail

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>A</b>

<br>

설명:

<br>

<b>A (정답):</b> **AWS X-Ray**는 개발자가 분산 애플리케이션의 요청 흐름을 추적하고, **코드 내의 성능 병목 구간을 식별**하여 디버깅하고 분석하는 데 도움을 주는 서비스입니다.

<br>

<b>C (오답):</b> CloudWatch는 인프라 수준의 성능(CPU, 메모리 등)을 모니터링하지만, 코드 내부까지 들여다보지는 못합니다.

</details>


---

60. 한 회사가 여러 AWS 계정의 리소스를 통합하여 보고 싶어합니다. 예를 들어, 여러 계정에 흩어져 있는 AWS Config 규칙 위반 사항이나 보안 결과를 하나의 대시보드에서 확인하고 싶을 때 어떤 서비스를 사용해야 할까요?

A. AWS Trusted Advisor

B. AWS Organizations

C. AWS Security Hub

D. Amazon CloudWatch

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<br>

설명:

<br>

<b>C (정답):</b> **AWS Security Hub**는 AWS Organizations와 통합하여, 여러 AWS 계정의 **보안 상태를 포괄적으로 확인**할 수 있는 단일 장소를 제공합니다. GuardDuty, Inspector, Macie 등 다양한 보안 서비스의 결과를 **하나의 대시보드에 통합**하여 보여줍니다.

<br>

<b>B (오답):</b> AWS Organizations는 계정 관리 프레임워크 자체이며, 보안 결과를 직접 통합하여 보여주지는 않습니다.

</details>


---

61. 개발자가 웹 또는 모바일 애플리케이션의 백엔드(인증, 스토리지, API 등)를 쉽게 구축하고 구성할 수 있도록 도와주는 개발 프레임워크 및 도구 세트는 무엇입니까?

A. AWS Amplify

B. Amazon API Gateway

C. AWS Elastic Beanstalk

D. AWS AppSync

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>A</b>

<br>

설명:

<br>

<b>A (정답):</b> **AWS Amplify**는 개발자가 클라우드 전문 지식 없이도 확장 가능한 웹 및 모바일 앱을 구축할 수 있도록 지원하는 **개발 프레임워크**입니다. 인증, 스토리지, 데이터스토어, API 등 백엔드 기능을 쉽게 구성할 수 있는 도구와 라이브러리를 제공합니다.

<br>

<b>C (오답):</b> Elastic Beanstalk은 코드 배포를 자동화하는 PaaS 플랫폼입니다.

</details>


---

62. 다음 중 AWS가 고객에게 제공하는 클라우드 배포 모델이 아닌 것은 무엇입니까?

A. 클라우드 (All-in Cloud)

B. 하이브리드 (Hybrid)

C. 온프레미스 (On-Premises)

D. 폐쇄형 네트워크 (Closed-Network)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> AWS는 모든 것을 클라우드에서 실행하는 모델, 클라우드와 온프레미스를 함께 사용하는 하이브리드 모델, 그리고 **AWS Outposts**와 같은 서비스를 통해 고객의 데이터 센터에서 AWS 인프라를 실행하는 온프레미스 모델을 지원합니다. '폐쇄형 네트워크'는 표준 배포 모델이 아닙니다.

</details>


---

63. AWS 리소스에 대한 모든 API 호출은 암호화된 채널(TLS)을 통해 이루어집니다. 이는 어떤 유형의 데이터 보호 조치에 해당합니까?

A. 저장 데이터 암호화 (Encryption at Rest)

B. 전송 데이터 암호화 (Encryption in Transit)

C. 클라이언트 측 암호화 (Client-Side Encryption)

D. 서버 측 암호화 (Server-Side Encryption)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> 데이터가 네트워크를 통해 **이동하는 중**에 가로채더라도 내용을 알 수 없도록 암호화하는 것을 **전송 데이터 암호화(Encryption in Transit)**라고 합니다. TLS(Transport Layer Security)는 이를 위한 표준 프로토콜입니다.

<br>

<b>A (오답):</b> 저장 데이터 암호화는 디스크나 스토리지에 저장된 데이터를 보호하는 것입니다.

</details>


---

64. 한 조직의 모든 구성원이 기존 회사 자격 증명(예: Active Directory)을 사용하여 한 번의 로그인으로 여러 AWS 계정 및 비즈니스 애플리케이션에 접근할 수 있도록 하려고 합니다. 어떤 서비스가 가장 적합합니까?

A. AWS IAM

B. Amazon Cognito

C. AWS Directory Service

D. AWS IAM Identity Center (구 AWS Single Sign-On)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<br>

설명:

<br>

<b>D (정답):</b> **AWS IAM Identity Center**는 **한 번의 로그인(Single Sign-On, SSO)**으로 여러 AWS 계정과 클라우드 애플리케이션에 대한 접근을 중앙에서 관리하는 서비스입니다. 기존의 자격 증명 공급자(IdP)와 연동하여 사용할 수 있습니다.

<br>

<b>B (오답):</b> Amazon Cognito는 주로 고객 대면 애플리케이션(모바일/웹 앱)의 사용자 가입 및 로그인을 위한 서비스입니다.

</details>


---

65. AWS Well-Architected Framework의 비용 최적화 원칙을 실천하는 가장 좋은 예는 무엇입니까?

A. 모든 워크로드에 가장 큰 EC2 인스턴스를 사용하여 성능을 보장합니다.

B. 워크로드의 특성에 맞는 적절한 구매 옵션(예: Savings Plans)을 선택합니다.

C. 모든 데이터를 가장 빠른 스토리지(예: 프로비저닝된 IOPS EBS)에 저장합니다.

D. 보안 모니터링 서비스를 비활성화하여 비용을 절감합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<br>

설명:

<br>

<b>B (정답):</b> **비용 최적화**의 핵심은 불필요한 지출을 없애고, 워크로드에 가장 적합한 리소스와 요금 모델을 선택하는 것입니다. 안정적인 워크로드에 Savings Plans나 예약 인스턴스와 같은 할인된 **구매 옵션을 선택**하는 것이 대표적인 실천 방안입니다.

<br>

<b>A, C (오답):</b> 필요 이상으로 과도한 사양의 리소스를 사용하는 것은 비용 낭비이며, 비용 최적화에 위배됩니다.

<br>

<b>D (오답):</b> 비용을 절감하기 위해 보안을 희생하는 것은 절대 권장되지 않는 방법입니다.

</details>