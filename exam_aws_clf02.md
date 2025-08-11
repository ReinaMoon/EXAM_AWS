
1. 다음 중 AWS 계정 루트 사용자의 특징은 무엇입니까?

A. 루트 사용자는 다중 인증(MFA)를 구성할 수 있는 유일한 사용자입니다.

B. 루트 사용자는 AWS 관리 콘솔에 액세스할 수 있는 유일한 사용자입니다.

C. 루트 사용자는 AWS 계정이 생성될 때 사용할 수 있는 첫 번째 로그인 아이디입니다.

D. 루트 사용자의 비밀번호는 변경할 수 없습니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): AWS 계정을 처음 만들 때 사용하는 이메일 주소와 암호가 바로 '루트 사용자' 자격 증명입니다. 계정의 모든 권한을 가진 최초의 사용자입니다.

A (오답): MFA(다중 인증)는 루트 사용자뿐만 아니라 모든 IAM 사용자에게도 설정할 수 있으며, 보안을 위해 강력히 권장됩니다.

B (오답): 적절한 권한을 가진 IAM 사용자 역시 AWS 관리 콘솔에 로그인하여 할당된 작업을 수행할 수 있습니다.

D (오답): 루트 사용자의 비밀번호는 변경할 수 있으며, 보안을 위해 정기적으로 변경해야 합니다.

</details>

2. 어떤 AWS 기능 또는 리소스가 소프트웨어 및 보안 요구 사항이 미리 패키지된 배포 가능한 Amazon EC2 인스턴스 템플릿입니까?

A. Amazon Elastic Block Store(Amazon EBS) 볼륨

B. AWS CloudFormation 템플릿

C. Amazon Elastic Block Store(Amazon EBS) 스냅샷

D. Amazon 머신 이미지(AMI)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:

D (정답): AMI(Amazon Machine Image)는 EC2 인스턴스를 시작하는 데 필요한 정보를 제공하는 템플릿입니다. 여기에는 운영 체제(OS), 애플리케이션 서버, 애플리케이션 등이 포함됩니다.

B (오답): AWS CloudFormation 템플릿은 EC2 인스턴스뿐만 아니라 VPC, 데이터베이스, 로드 밸런서 등 전체 AWS 인프라를 코드로 정의하고 배포하는 데 사용됩니다. 범위가 훨씬 더 넓습니다.

</details>

3. 다음 중 AWS Well-Architected Framework의 핵심 요소는 무엇입니까? (두 가지 선택)

A. 가용성

B. 신뢰성

C. 확장성

D. 반응형 디자인

E. 운영 우수성

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B, E**


설명:
AWS Well-Architected Framework는 6개의 핵심 요소(Pillars)로 구성됩니다.

운영 우수성 (Operational Excellence)

보안 (Security)

신뢰성 (Reliability)

성능 효율성 (Performance Efficiency)

비용 최적화 (Cost Optimization)

지속 가능성 (Sustainability)
A(가용성)와 C(확장성)는 신뢰성 및 성능 효율성 기둥에 포함되는 하위 개념입니다.

</details>

4. 보안 엔지니어가 데이터 보안 관련 규정 준수 요건을 충족하기 위해 자체 암호화 키를 생성, 제어 및 관리할 수 있는 단일 테넌트 AWS 솔루션을 원합니다. 이 엔지니어는 어떤 AWS 서비스를 사용해야 합니까?

A. AWS 키 관리 서비스(AWS KMS)

B. AWS 인증서 관리자(ACM)

C. AWS 클라우드HSM

D. AWS 시스템 관리자

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): AWS CloudHSM은 클라우드에서 전용 하드웨어 보안 모듈(HSM)을 제공하는 단일 테넌트 서비스입니다. 사용자가 직접 암호화 키를 완전하게 생성, 제어, 관리할 수 있으며, FIPS 140-2 Level 3과 같은 높은 수준의 규정 준수 요건을 충족합니다.

A (오답): AWS KMS는 암호화 키를 쉽게 생성하고 제어할 수 있는 관리형 서비스이지만, 다중 테넌트 환경이며 AWS가 하드웨어를 관리합니다. 키에 대한 제어 수준이 CloudHSM보다 낮습니다.

</details>

5. 어떤 AWS 기능이 이러한 요구 사항을 충족합니까? (2개 선택) - 질문 컨텍스트 부족

A. 보안 그룹

B. 네트워크 ACL

C. S3 버킷 정책

D. IAM 사용자 정책

E. S3 버킷 버전 관리

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A, B (만약 네트워크 트래픽 제어 요구사항이라면)**


설명:
질문의 컨텍스트가 명확하지 않지만, 일반적인 네트워크 보안 제어 요구사항을 가정할 때의 답입니다.

A. 보안 그룹 (Security Group): EC2 인스턴스 수준에서 인바운드/아웃바운드 트래픽을 제어하는 가상 방화벽입니다.

B. 네트워크 ACL (Network Access Control List): 서브넷 수준에서 트래픽을 제어하는 방화벽입니다.
사용자님께서 선택하신 B(네트워크 ACL)와 D(IAM 정책)는 서로 다른 계층의 보안을 담당합니다. B는 네트워크 트래픽을, D는 사용자/역할의 AWS 서비스 API 호출 권한을 제어합니다.

</details>

6. 중단을 견딜 수 있는 상태 비저장 워크로드에 비해 가장 비용 효율적인 Amazon EC2 인스턴스 구매 옵션은 무엇입니까?

A. 스팟 인스턴스

B. 변환 가능한 예약 인스턴스

C. 표준 예약 인스턴스

D. 전용 호스트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A**


설명:

A (정답): 스팟 인스턴스는 AWS의 미사용 EC2 용량을 활용하여 온디맨드 요금보다 훨씬 저렴하게 제공됩니다. 하지만 AWS가 해당 용량을 필요로 할 경우 2분 전 알림과 함께 인스턴스가 중단될 수 있습니다. 따라서 "중단을 견딜 수 있는" 워크로드에 가장 비용 효율적입니다.

B, C (오답): 예약 인스턴스는 1년 또는 3년 약정을 통해 상당한 할인을 받으며, 중단되지 않는 안정적인 워크로드에 적합합니다. 스팟 인스턴스보다는 비쌉니다.

</details>

7. 대규모로 밀리초 미만의 지연 시간을 제공하는 키-값 데이터베이스인 AWS 서비스는 무엇입니까?

A. Amazon DynamoDB

B. 아마존 오로라

C. Amazon DocumentDB(MongoDB와 호환)

D. 아마존 넵튠

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A**


설명:

A (정답): Amazon DynamoDB는 어떤 규모에서든 한 자릿수 밀리초의 성능을 제공하도록 설계된 키-값 및 문서 데이터베이스입니다.

B (오답): Amazon Aurora는 고성능 관계형 데이터베이스(MySQL, PostgreSQL 호환)입니다.

C (오답): Amazon DocumentDB는 MongoDB와 호환되는 문서 데이터베이스이지만, 키-값 데이터베이스는 아닙니다.

</details>

8. Amazon S3에 저장된 객체를 보호하는 데 사용할 수 있는 암호화 유형은 무엇입니까? (2개 선택)

A. AmazonS3 관리 암호화 키(SSE-S3)를 사용한 서버 측 암호화

B. AWS KMS 관리 키를 사용한 서버 측 암호화(SSE-KMS)

C. TLS

D. SSL

E. 투명한 데이터 암호화(TDE)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A, B**


설명:

A, B (정답): S3에 저장된 데이터(Encryption at rest, 미사용 데이터 암호화)를 보호하기 위해 서버 측 암호화(SSE)를 사용합니다. SSE-S3는 S3가 키를 관리하고, SSE-KMS는 AWS KMS를 통해 키를 관리하여 더 세분화된 제어와 감사 기능을 제공합니다.

C, D (오답): TLS/SSL은 클라이언트와 서버 간에 **전송 중인 데이터(Encryption in transit)**를 암호화하는 프로토콜입니다. S3에 이미 저장된 객체를 보호하는 것과는 목적이 다릅니다.

</details>

9. 한 회사는 통합 청구를 위해 AWS Organizations의 조직에 두 개의 AWS 계정을 가지고 있습니다. 계정 A는 Amazon EC2 Standard Reserved Instances(RI) 5개를 구매했습니다. 계정 A는 EC2 인스턴스 4개를 실행 중입니다. 계정 B는 RI를 구매하지 않았고 EC2 인스턴스 4개를 실행 중입니다. 이 8가지 인스턴스에 대한 설명으로 옳은 것은 무엇입니까?

A. 8개의 인스턴스는 일반 인스턴스로 요금이 청구됩니다.

B. 인스턴스 4개는 RI로 청구되고, 인스턴스 4개는 일반 인스턴스로 청구됩니다.

C. 인스턴스 5개는 RI로 청구되고, 인스턴스 3개는 일반 인스턴스로 청구됩니다.

D. 8개의 인스턴스는 RI로 청구됩니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:
AWS Organizations의 통합 청구에서는 기본적으로 RI 할인이 조직 내 모든 계정 간에 공유됩니다.

계정 A가 구매한 RI 5개는 먼저 구매한 계정 A의 인스턴스 4개에 적용됩니다.

이제 남은 RI 1개가 있습니다. 이 남은 RI 할인은 조직 내 다른 계정인 계정 B의 인스턴스 1개에 적용됩니다.

따라서, 총 5개(계정 A의 4개 + 계정 B의 1개)의 인스턴스가 RI로 청구되고, 계정 B의 나머지 인스턴스 3개는 온디맨드(일반) 요금으로 청구됩니다.

</details>

10. 어떤 AWS 서비스가 사용자가 여러 Lambda 함수 세트에 대한 워크플로를 조율하고 프로세스를 조율하는 데 도움을 주도록 설계되었습니까?

A. Amazon DynamoDB

B. AWS 코드 파이프라인

C. AWS 배치

D. AWS Step Functions

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:

D (정답): AWS Step Functions는 Lambda 함수와 같은 여러 AWS 서비스를 시각적인 워크플로로 **조율(Orchestration)**하는 서버리스 서비스입니다. "A 함수 실행 후 성공하면 B 함수, 실패하면 C 함수 실행"과 같은 복잡한 흐름을 관리합니다.

B (오답): AWS CodePipeline은 소스 코드 변경 시 자동으로 빌드, 테스트, 배포하는 CI/CD 파이프라인을 자동화하는 서비스입니다.

C (오답): AWS Batch는 대규모 배치 컴퓨팅 작업을 효율적으로 실행하는 서비스입니다.

</details>

11. 한 회사가 타사 소프트웨어 서비스(SaaS) 애플리케이션에 대한 액세스 및 권한을 관리하려고 합니다. 이 회사는 최종 사용자가 할당된 계정 및 AWS 클라우드 애플리케이션에 액세스할 수 있는 포털을 원합니다. 이러한 요구 사항을 충족하기 위해 회사는 어떤 AWS 서비스를 사용해야 합니까?

A. Amazon Cognito

B. AWS IAM Identity Center(AWS Single Sign-On)

C. AWS ID 및 액세스 관리(IAM)

D. Microsoft Active Directory용 AWS 디렉터리 서비스

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B**


설명:

B (정답): AWS IAM Identity Center (이전 명칭: AWS SSO)는 여러 AWS 계정 및 Salesforce, Office 365와 같은 **클라우드 애플리케이션(SaaS)**에 대한 Single Sign-On (SSO) 액세스를 중앙에서 관리하는 서비스입니다. 사용자는 포털을 통해 할당된 모든 애플리케이션에 접근할 수 있습니다.

A (오답): Amazon Cognito는 개발하는 웹/모바일 앱의 **고객(외부 사용자)**들이 회원가입, 로그인하는 기능을 제공하는 서비스입니다. 회사 내부 직원의 SSO와는 용도가 다릅니다.

</details>

12. 회사에서는 AWS 지출 목표를 설정하고 목표에 따른 비용을 추적하려고 합니다. 이러한 요구 사항을 충족하기 위해 회사는 어떤 AWS 도구나 기능을 사용해야 합니까?

A. AWS 비용 탐색기

B. AWS 예산

C. AWS 비용 및 사용 보고서

D. 저축 계획

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B**


설명:

B (정답): AWS Budgets는 사용자 지정 비용 및 사용량 예산을 설정하고, 실제 또는 예측 비용이 예산을 초과할 때 알림을 받도록 하는 기능입니다. "목표 설정 및 추적"이라는 요구사항에 가장 부합합니다.

A (오답): AWS Cost Explorer는 과거의 비용을 시각화하고 분석하는 도구입니다. 예산을 설정하고 알림을 보내는 기능은 없습니다.

</details>

13. 가용성 영역의 특징은 무엇입니까? (2개 선택)

A. AWS 지역의 모든 가용성 영역은 대역폭이 높고 지연 시간이 짧은 네트워킹으로 상호 연결됩니다.

B. 가용성 영역은 물리적으로 최소 150km(100마일)의 거리로 분리되어 있습니다.

C. 가용성 영역 간의 모든 트래픽은 암호화됩니다.

D. AWS 지역 내의 가용성 영역은 중복된 전원, 네트워킹 및 연결을 공유합니다.

E. 모든 가용성 영역에는 단일 데이터 센터가 포함됩니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A, C**


설명:

A (정답): 가용성 영역(AZ)들은 낮은 지연 시간과 높은 대역폭을 가진 전용 광섬유 네트워크로 연결되어 있어, AZ 간에 데이터를 빠르게 복제할 수 있습니다.

C (정답): AWS 글로벌 네트워크 백본을 통과하는 AZ 간 트래픽은 물리 계층에서 자동으로 암호화됩니다.

D (오답): 가용성 영역은 독립적인 전원, 냉각, 물리적 보안을 갖도록 설계되어 서로의 장애에 영향을 받지 않습니다.

E (오답): 가용성 영역은 하나 이상의 개별 데이터 센터로 구성될 수 있습니다.

</details>

14. 한 회사가 타사 ID 공급자(IdP)를 사용합니다. 이 회사는 다른 로그인 자격 증명을 요구하지 않고 직원들에게 AWS 계정 및 서비스에 대한 액세스 권한을 제공하고자 합니다. 어떤 AWS 서비스가 이 요구 사항을 충족할까요?

A. Amazon Cognito

B. AWS 리소스 액세스 관리자(AWS RAM)

C. AWS 디렉터리 서비스

D. AWS IAM ID 센터

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:
이 문제는 11번 문제와 거의 동일합니다.

D (정답): AWS IAM Identity Center는 Okta, Azure AD와 같은 타사 IdP와 연동하여 직원들이 기존 회사 자격 증명으로 AWS 계정에 **SSO(Single Sign-On)**할 수 있도록 지원합니다.

A (오답): Amazon Cognito는 개발하는 앱의 고객 인증용입니다.

</details>

15. 회사에서는 모든 프로세스가 효과적이고 직원이 프로세스에 익숙한지 검토하기 위해 작업 흐름을 시뮬레이션합니다. 이 관행에서 회사는 AWS Well-Architected Framework의 어떤 설계 원칙을 따릅니까?

A. 코드로 작업을 수행합니다.

B. 작업 절차를 자주 수정하세요.

C. 작고 되돌릴 수 있는 변경을 자주 만드세요.

D. 비즈니스 성과를 지원하도록 회사를 구성합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:
이 활동은 운영 우수성(Operational Excellence) 기둥과 관련이 있습니다. 작업 흐름을 시뮬레이션(Game days)하는 것은 운영 절차를 검증하고 개선하여 비즈니스 목표를 달성하기 위함입니다.

D (정답): "비즈니스 성과를 지원하도록 회사를 구성합니다"는 운영 우수성의 상위 목표를 가장 잘 나타냅니다. 효과적인 프로세스를 통해 비즈니스 가치를 창출하는 것이 핵심입니다.

A, C (오답): 이들은 운영 우수성의 다른 중요한 원칙들이지만, '프로세스 검토 및 시뮬레이션'이라는 활동보다는 '배포 자동화 및 변경 관리'와 더 직접적으로 관련됩니다.

</details>

16. 회사에서는 사업부에서 더 이상 액세스할 필요가 없는 Amazon S3 데이터를 보관해야 합니다. 어떤 S3 스토리지 클래스가 이 요구 사항을 가장 비용 효율적으로 충족할까요?

A. S3 Glacier 즉시 검색

B. S3 Glacier 유연한 검색

C. S3 빙하 심층 아카이브

D. S3 One Zone-Infrequent Access(S3 One Zone-IA)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): S3 Glacier Deep Archive는 가장 저렴한 스토리지 비용을 제공하며, 수년에 한두 번 액세스하는 데이터의 **장기 보관(아카이빙)**을 위해 설계되었습니다.

A, B (오답): Glacier Instant/Flexible Retrieval은 Deep Archive보다 스토리지 비용이 비싸지만 데이터 검색 속도가 더 빠릅니다.

</details>

17. 회사에서는 특정 Amazon EC2 인스턴스에 보안 규칙을 적용해야 합니다. 어떤 AWS 서비스나 기능이 이 기능을 제공합니까?

A. AWS 쉴드

B. 네트워크 ACL

C. 보안 그룹

D. AWS 방화벽 관리자

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): 보안 그룹(Security Group)은 개별 EC2 인스턴스에 연결되어 인바운드 및 아웃바운드 트래픽을 제어하는 상태 저장(stateful) 가상 방화벽 역할을 합니다.

B (오답): 네트워크 ACL은 서브넷 수준에서 작동하며, 해당 서브넷 내의 모든 인스턴스에 영향을 미치는 상태 비저장(stateless) 방화벽입니다.

</details>

18. 한 회사가 고성능 컴퓨팅(HPC) 워크로드를 위해 설계된 데이터 레이어가 있습니다. 이 회사는 이러한 요구 사항을 충족하기 위해 어떤 Amazon EC2 인스턴스 유형을 사용해야 합니까?

A. 저장소 최적화

B. 일반 목적

C. 메모리 최적화

D. 최적화된 인스턴스 계산

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:

D (정답): 컴퓨팅 최적화 (Compute Optimized) 인스턴스 (예: C 계열)는 고성능 프로세서를 갖추고 있어 HPC, 배치 처리, 미디어 트랜스코딩과 같이 CPU 집약적인 워크로드에 이상적입니다.

</details>

19. Amazon Aurora는 어떤 데이터베이스 엔진을 지원합니까? (2개 선택)

A. 오라클

B. 마이크로소프트 SQL 서버

C. MySQL

D. PostgreSQL

E. MariaDB

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C, D**


설명:

C, D (정답): Amazon Aurora는 클라우드에 맞게 구축된 관계형 데이터베이스로, MySQL 및 PostgreSQL과 완벽하게 호환됩니다. 기존 애플리케이션을 거의 변경 없이 마이그레이션할 수 있습니다.

</details>

20. VPC에 인터넷 게이트웨이를 두는 목적은 무엇입니까?

A. VPC에 VPN 연결을 생성하려면

B. VPC와 인터넷 간 통신을 허용합니다.

C. 인터넷 트래픽에 대역폭 제한을 부과합니다.

D. Amazon EC2 인스턴스 전반에서 인터넷 트래픽의 부하를 분산하려면

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B**


설명:

B (정답): 인터넷 게이트웨이(IGW)는 VPC와 인터넷 간의 통신을 가능하게 하는 VPC의 구성 요소입니다. IGW가 연결된 VPC 내의 리소스(예: 퍼블릭 서브넷의 EC2 인스턴스)는 인터넷에 접근할 수 있습니다.

</details>

21. AWS Trusted Advisor는 어떤 범주에서 권장 조치를 제공합니까? (2개 선택)

A. 운영 체제 패치

B. 비용 최적화

C. 반복적인 작업

D. 서비스 할당량

E. 계정 활동 기록

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B, D**


설명:
AWS Trusted Advisor는 5가지 범주에서 모범 사례 권장 사항을 제공합니다.

비용 최적화 (Cost Optimization)

성능 (Performance)

보안 (Security)

내결함성 (Fault Tolerance)

서비스 한도 (Service Quotas)

</details>

22. 알려지지 않은 액세스 패턴에 대해 가장 비용 효율적인 Amazon S3 스토리지 클래스는 무엇입니까?

A. S3 표준

B. S3 Standard-Infrequent Access(S3 Standard-IA)

C. S3 One Zone-Infrequent Access(S3 One Zone-IA)

D. S3 지능형 계층화

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:

D (정답): S3 Intelligent-Tiering은 객체의 액세스 패턴을 모니터링하고, 액세스 빈도에 따라 데이터를 가장 비용 효율적인 스토리지 계층으로 자동으로 이동시키는 서비스입니다. 따라서 "알려지지 않았거나 변경되는" 액세스 패턴에 가장 적합합니다.

</details>

23. 어떤 회사는 AWS 클라우드를 자사 온프레미스 인프라의 오프사이트 백업 위치로 사용하려고 합니다. 어떤 AWS 서비스가 이 요구 사항을 가장 비용 효율적으로 충족할 수 있을까요?

A. 아마존 S3

B. Amazon Elastic File System(Amazon EFS)

C. 아마존 FSx

D. Amazon Elastic Block Store(Amazon EBS)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A**


설명:

A (정답): Amazon S3는 내구성이 매우 높고 확장 가능하며 비용 효율적인 객체 스토리지 서비스로, 백업 및 아카이빙에 가장 이상적이고 널리 사용됩니다. 다양한 스토리지 클래스와 수명 주기 정책을 통해 비용을 더욱 최적화할 수 있습니다.

</details>

24. 사용자는 Amazon EC2 인스턴스에서 실행되는 애플리케이션이 다른 AWS 서비스를 호출할 수 있도록 허용하려고 합니다. 허용된 액세스는 안전해야 합니다. 어떤 AWS 서비스 또는 기능을 사용해야 합니까?

A. 보안 그룹

B. AWS 방화벽 관리자

C. IAM 역할

D. IAM 사용자 SSH 키

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): **IAM 역할(Role)**은 EC2 인스턴스와 같은 AWS 리소스에 권한을 부여하는 가장 안전하고 권장되는 방법입니다. 역할은 임시 보안 자격 증명을 사용하여 다른 서비스에 액세스하므로, 액세스 키와 같은 장기 자격 증명을 코드에 하드코딩할 필요가 없습니다.

</details>

25. 한 회사는 지속 가능성 영역에 대한 목표를 달성하는 방법을 파악하기 위해 사용자 행동 패턴을 수집하고 있습니다. 이러한 목표를 달성하기 위해 회사가 구현해야 할 모범 사례는 무엇입니까? (2개 선택)

A. 사용자 부하에 따라 인프라를 확장합니다.

B. 작업 부하와 사용자 위치 간의 지리적 거리를 최대화합니다.

C. 사용되지 않는 자산의 생성 및 유지 관리를 제거합니다.

D. 여유 용량이 있는 리소스를 확장하고 자동 크기 조정을 제거합니다.

E. 사용자 수에 따라 인프라를 확장합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A, C (또는 A, E)**


설명:
AWS Well-Architected Framework의 지속 가능성 기둥은 낭비를 줄이고 활용률을 극대화하는 것을 목표로 합니다.

A, E (정답): "사용자 부하/수"에 따라 인프라를 확장하는 것은 수요에 맞게 공급을 조정하는 것으로, 불필요한 리소스 사용을 막는 핵심 원칙입니다.

C (정답): 사용하지 않는 리소스를 제거하는 것은 직접적인 낭비 제거에 해당합니다.

D (오답): 여유 용량을 과도하게 두고 자동 크기 조정을 제거하는 것은 과잉 프로비저닝으로 이어져 지속 가능성에 반하는 행위입니다.

</details>

26. AWS는 수십만 명의 사용자의 사용량을 집계하여 더 낮은 종량제 가격을 책정할 수 있는 역량을 갖추고 있습니다. 이는 AWS 클라우드의 어떤 장점을 설명합니까?

A. 몇 분 안에 전 세계적으로 출시

B. 속도와 민첩성 증가

C. 규모의 경제성이 높음

D. 컴퓨팅 용량에 대한 추측 없음

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): **규모의 경제(Economies of scale)**는 AWS가 대규모로 운영함으로써 얻는 비용 절감 효과를 고객에게 더 낮은 가격으로 제공할 수 있음을 의미합니다. 수많은 사용자의 사용량을 집계하는 것이 바로 그 예입니다.

</details>

27. 어떤 AWS 클라우드 배포 모델이 애플리케이션 배포 인프라의 일부로 AWS Outposts를 사용합니까?

A. 온프레미스

B. 서버리스

C. 클라우드 네이티브

D. 하이브리드

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:

D (정답): AWS Outposts는 AWS 인프라와 서비스를 고객의 온프레미스 데이터 센터로 확장하는 서비스입니다. 이는 온프레미스 환경과 AWS 클라우드를 원활하게 연결하는 하이브리드 클라우드 모델의 핵심 요소입니다.

</details>

28. 회사에서는 SQL 주입 공격을 차단해야 합니다. 어떤 AWS 서비스나 기능이 이 요구 사항을 충족할 수 있을까요?

A. AWS WAF

B. AWS 쉴드

C. 네트워크 ACL

D. 보안 그룹

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A**


설명:

A (정답): **AWS WAF (Web Application Firewall)**는 웹 애플리케이션을 보호하는 L7 방화벽으로, SQL 주입, 크로스 사이트 스크립팅(XSS)과 같은 일반적인 웹 공격을 탐지하고 차단하는 규칙을 생성할 수 있습니다.

B, C, D (오답): Shield(DDoS 방어), NACL/보안 그룹(네트워크 트래픽 제어)은 SQL 주입과 같은 애플리케이션 계층의 공격 콘텐츠를 분석하지 않습니다.

</details>

29. 어떤 AWS 데이터베이스 서비스가 메모리 내 데이터 스토리를 제공합니까?

A. Amazon DynamoDB

B. 아마존 엘라스티캐시

C. 아마존 RDS

D. 아마존 타임스트림

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B**


설명:

B (정답): Amazon ElastiCache는 Redis 및 Memcached와 호환되는 완전 관리형 인메모리(in-memory) 데이터 스토어 또는 캐시 서비스입니다. 빠른 응답 시간이 필요한 애플리케이션의 성능을 향상시키는 데 사용됩니다.

</details>

30. 한 회사가 고성능 컴퓨팅(HPC) 애플리케이션을 Amazon EC2 인스턴스로 마이그레이션하려고 합니다. 애플리케이션에는 여러 구성 요소가 있습니다. 애플리케이션에는 내결함성이 있어야 하며 자동 장애 조치가 가능한 기능이 있어야 합니다. 구성 요소 간 지연 시간을 최소화하면서 이러한 요구 사항을 충족하는 AWS 인프라 솔루션은 무엇입니까?

A. 여러 AWS 지역

B. 다중 예지 위성

C. 다중 가용성 영역

D. 지역 에지 캐시

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): **다중 가용성 영역(Multi-AZ)**에 애플리케이션 구성 요소를 배포하는 것은 내결함성을 확보하는 표준 방법입니다. 하나의 AZ에 장애가 발생해도 다른 AZ의 구성 요소가 계속 작동합니다. 또한, 같은 리전 내의 AZ들은 낮은 지연 시간으로 연결되어 있어 구성 요소 간 통신 성능 저하를 최소화할 수 있습니다.

A (오답): 여러 AWS 지역은 재해 복구에는 좋지만, 지역 간 거리가 멀어 지연 시간이 높기 때문에 구성 요소 간 통신에는 적합하지 않습니다.

</details>

31. 한 회사가 온프레미스 데이터 웨어하우스를 AWS로 마이그레이션하려고 합니다. 데이터 웨어하우스의 정보는 분석 대시보드를 채우는 데 사용됩니다. 이 회사는 데이터 웨어하우스에 어떤 AWS 서비스를 사용해야 합니까?

A. Amazon ElastiCache

B. 아마존 오로라

C. 아마존 RDS

D. 아마존 레드쉬프트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:

D (정답): Amazon Redshift는 페타바이트 규모의 완전 관리형 데이터 웨어하우스(Data Warehouse) 서비스입니다. 대규모 데이터 세트에 대한 복잡한 쿼리를 빠르게 실행할 수 있어 분석 및 비즈니스 인텔리전스(BI) 대시보드에 이상적입니다.

</details>

32. 어떤 회사는 VPC에서 Amazon EC2 인스턴스를 실행하고 있습니다. 전자상거래 회사는 Amazon EC2에서 실행되는 웹 서버를 관리하기 위해 Amazon EC2 Auto Scaling 그룹을 사용하고 있습니다. 이 아키텍처는 어떤 AWS Well-Architected Framework 모범 사례를 따르나요?

A. 작업 부하를 확보하세요

B. 인프라 구성요소 분리

C. 실패를 위한 디자인

D. 병렬적으로 생각해보세요

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): Auto Scaling 그룹은 상태 확인에 실패한 인스턴스를 자동으로 종료하고 새 인스턴스로 교체합니다. 이는 구성 요소의 장애가 전체 시스템의 장애로 이어지지 않도록 하는 **실패를 위한 설계(Design for Failure)**의 대표적인 예시이며, 신뢰성(Reliability) 기둥의 핵심 원칙입니다.

</details>

33. 어떤 AWS 서비스가 사용자가 AWS 인프라, AWS 서비스, API 및 도구를 데이터 센터, 콜로케이션 환경 또는 온프레미스 시설로 확장할 수 있는 하이브리드 아키텍처를 지원하는 AWS 서비스는 무엇입니까?

A. AWS 스노모빌

B. AWS 로컬 영역

C. AWS 아웃포스트

D. AWS Fargate

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): AWS Outposts는 AWS 인프라, 서비스, API 및 도구를 고객의 데이터 센터, 코로케이션 환경 또는 온프레미스 시설로 확장하여 진정한 하이브리드 경험을 제공하는 서비스입니다.

</details>

34. 회사에서 서버리스 애플리케이션을 시각적으로 디자인하고 구축하는 데 사용할 수 있는 AWS 서비스는 무엇입니까?

A. AWS 람다

B. AWS 배치

C. AWS 애플리케이션 컴포저

D. AWS App Runner

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): AWS Application Composer는 AWS 서비스를 드래그 앤 드롭 방식으로 연결하여 서버리스 애플리케이션 아키텍처를 시각적으로 설계하고, 이를 CloudFormation 또는 SAM 템플릿으로 생성해주는 도구입니다.

</details>

35. 가용성 영역은 다음으로 구성됩니다.

A. 단일 위치에 있는 하나 이상의 데이터 센터.

B. 여러 지역에 위치한 두 개 이상의 데이터 센터.

C. 단일 데이터 센터에 있는 하나 이상의 물리적 호스트.

D. 여러 데이터 센터에 있는 두 개 이상의 물리적 호스트.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A**


설명:

A (정답): 가용성 영역(AZ)은 하나 이상의 개별 데이터 센터로 구성되며, 각 데이터 센터는 중복 전원, 네트워킹 및 연결 기능을 갖추고 있습니다. 이들은 하나의 AWS 리전 내에 물리적으로 격리된 위치에 있습니다.

</details>

36. 어떤 회사에서는 AWS 계정의 모든 사용자 목록, 모든 사용자의 액세스 키 상태, 그리고 다중 요소 인증(MFA)이 구성되었는지 여부를 알고 싶어합니다. 어떤 AWS 서비스나 기능이 이러한 요구 사항을 충족할까요?

A. AWS 키 관리 서비스(AWS KMS)

B. IAM 액세스 분석기

C. IAM 자격 증명 보고서

D. Amazon CloudWatch

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:

C (정답): **IAM 자격 증명 보고서(Credential Report)**는 계정의 모든 사용자와 암호, 액세스 키, MFA 장치 상태 등 다양한 자격 증명 상태에 대한 정보를 나열하는 CSV 보고서를 제공합니다.

B (오답): IAM Access Analyzer는 계정 외부의 엔터티와 공유되어 의도하지 않은 접근을 허용할 수 있는 리소스를 식별하는 데 도움이 됩니다.

</details>

37. 강사가 진행하는 환경에서 어떤 클라우드 보안에 대해 배우고자 택하세요? (2가지를 선택하세요.)

A. AWS 신뢰할 수 있는 고문

B. AWS 온라인 기술 토크

C. AWS 블로그

D. AWS 포럼

E. AWS 강의실 교육

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B, E**


설명:
"강사가 진행하는 환경"은 실시간으로 전문가의 설명을 들을 수 있는 교육을 의미합니다.

E (정답): AWS 강의실 교육은 공인 강사가 직접 진행하는 공식 교육 과정입니다.

B (정답): AWS 온라인 기술 토크는 AWS 전문가가 특정 주제에 대해 온라인으로 진행하는 웨비나 형식의 세션입니다.

A (오답): Trusted Advisor는 AWS 계정의 상태를 점검해주는 서비스이지 학습 리소스가 아닙니다.

</details>

38. 어떤 회사는 고객 경험에 대한 통찰력을 얻기 위해 서버 로그를 쿼리하려고 합니다. 어떤 서비스가 이 데이터를 가장 비용 효율적으로 저장할 수 있을까요?

A. 아마존 오로라

B. Amazon Elastic File System(Amazon EFS)

C. Amazon Elastic Block Store(Amazon EBS)

D. Amazon S3

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:

D (정답): 서버 로그와 같은 대량의 비정형 데이터를 가장 저렴하게 저장하고 나중에 쿼리(예: Athena 사용)하는 데는 Amazon S3가 가장 적합합니다. 저렴한 스토리지 클래스(예: S3 Standard-IA)와 라이프사이클 정책을 통해 비용을 더욱 최적화할 수 있습니다.

A, B, C (오답): 관계형 데이터베이스(Aurora)나 파일/블록 스토리지(EFS/EBS)는 대량의 로그를 저장하는 데 S3보다 훨씬 비쌉니다.

</details>

39. 회사에서는 고객에게 Amazon S3 버킷에 호스팅된 특정 데이터를 볼 수 있는 기능을 제공하려고 합니다. 회사는 고객과 공유하는 전체 데이터 세트를 계속 제어하려고 합니다. 이러한 요구 사항을 충족하는 S3 기능은 무엇입니까?

A. S3 스토리지 렌즈

B. S3 크로스 리전 복제(CRR)

C. S3 버전 관리

D. S3 액세스 포인트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:

D (정답): **S3 액세스 포인트(Access Point)**는 대규모 데이터 세트에 대한 액세스 관리를 간소화하는 기능입니다. 각 액세스 포인트에 고유한 정책과 네트워크 제어를 적용하여, 특정 사용자나 애플리케이션 그룹에 세분화된 데이터 액세스 권한을 쉽게 부여할 수 있습니다.

</details>

40. 한 회사가 보안 네트워크 연결을 통해 원격 직원에게 관리되는 Windows 가상 데스크톱과 애플리케이션을 제공하고자 합니다. 이 회사는 이러한 요구 사항을 충족하기 위해 어떤 AWS 서비스를 사용할 수 있습니까? (두 가지를 선택하세요.)

A. 아마존 커넥트

B. Amazon AppStream 2.0

C. Amazon 작업 공간

D. AWS 사이트 간 VPN

E. Amazon Elastic Container Service(Amazon ECS)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B, C**


설명:

C (정답): Amazon WorkSpaces는 완전 관리형의 안전한 클라우드 기반 가상 데스크톱(DaaS) 서비스입니다. 사용자에게 Windows 또는 Linux 데스크톱을 제공합니다.

B (정답): Amazon AppStream 2.0은 데스크톱 애플리케이션을 중앙에서 관리하고 모든 컴퓨터의 사용자에게 안전하게 스트리밍하는 서비스입니다. 가상 데스크톱 기능도 제공합니다.

</details>

41. 한 회사가 애플리케이션에 대한 인터넷 트래픽이 단기적으로 급증할 것으로 예상하고 있습니다. 트래픽이 증가하는 동안 애플리케이션은 중단될 수 없습니다. 또한 회사는 비용을 최소화하고 유연성을 극대화해야 합니다. 회사는 Amazon S3의 데이터를 분석하기 위해 서버리스 대화형 쿼리 서비스를 사용해야 합니다. 쿼리 서비스는 표준 SQL을 지원해야 합니다. 어떤 AWS 서비스가 이러한 요구 사항을 충족할까요?

A. 아마존 레드쉬프트

B. AWS Glue

C. Amazon Athena

D. Amazon Kinesis 데이터 스트림

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: C**


설명:
"S3 데이터 분석", "서버리스 대화형 쿼리", "표준 SQL"은 Amazon Athena를 가리키는 핵심 키워드입니다.

C (정답): Amazon Athena는 S3에 저장된 데이터를 표준 SQL을 사용하여 직접 쿼리할 수 있는 서버리스 대화형 쿼리 서비스입니다. 인프라를 관리할 필요가 없고 쿼리한 데이터 양에 대해서만 비용을 지불하므로 비용 효율적입니다.

</details>

42. 전자상거래 회사가 Amazon EC2 인스턴스에 새로운 웹 애플리케이션을 배포했습니다. 이 회사는 들어오는 HTTP 트래픽을 모든 실행 중인 인스턴스에 고르게 분산하려고 합니다. 어떤 AWS 서비스나 리소스가 이 요구 사항을 충족할까요?

A. 게이트웨이 로드 밸런서

B. 애플리케이션 로드 밸런서

C. 네트워크 로드 밸런서

D. Amazon EC2 자동 확장

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B**


설명:

B (정답): **Application Load Balancer (ALB)**는 OSI 모델의 7계층(애플리케이션 계층)에서 작동하며, HTTP 및 HTTPS 트래픽의 라우팅에 최적화되어 있습니다.

C (오답): Network Load Balancer (NLB)는 4계층(전송 계층)에서 작동하며, TCP/UDP 트래픽에 대한 초고성능 로드 밸런싱에 적합합니다.

D (오답): Auto Scaling은 트래픽에 따라 인스턴스 수를 자동으로 조절하는 기능이며, 트래픽을 분산하는 기능은 아닙니다.

</details>

43. 회사의 컴퓨팅 작업 부하가 안정적이고 예측 가능하며 중단되지 않습니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 Amazon EC2 인스턴스 구매 옵션은 무엇입니까? (2개 선택)

A. 주문형 인스턴스

B. 예약된 인스턴스

C. 스팟 인스턴스

D. 저축 계획

E. 전용 호스트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B, D**


설명:
"안정적이고 예측 가능한" 워크로드에 대한 비용 절감은 약정 기반 옵션을 통해 이루어집니다.

B (정답): **예약 인스턴스(Reserved Instances, RI)**는 특정 인스턴스 유형 및 리전에 대해 1년 또는 3년 약정을 통해 온디맨드 요금보다 상당한 할인을 제공합니다.

D (정답): Savings Plans는 특정 인스턴스 제품군 및 리전 내에서 시간당 컴퓨팅 사용량(USD/시간)에 대해 약정하여 유연하게 할인을 받을 수 있는 모델입니다. RI보다 유연성이 높습니다.

</details>

44. 장기 보관에 가장 비용 효율적인 Amazon S3 스토리지 클래스는 무엇입니까?

A. S3 빙하 심층 아카이브

B. S3 표준

C. S3 Standard-Infrequent Access(S3 Standard-IA)

D. S3 One Zone-Infrequent Access(S3 One Zone-IA)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A**


설명:
이 문제는 16번 문제와 동일합니다.

A (정답): S3 Glacier Deep Archive는 가장 저렴한 스토리지 비용을 제공하며, 수년에 한두 번 액세스하는 데이터의 **장기 보관(아카이빙)**을 위해 설계되었습니다.

</details>

45. 한 회사가 AWS에서 재설계된 웹사이트를 출시할 준비를 하고 있습니다. 전 세계 사용자가 웹사이트에서 디지털 핸드북을 다운로드할 것입니다. 회사에서는 정적 파일을 안전하게 제공하기 위해 어떤 AWS 솔루션을 사용해야 할까요?

A. Amazon Kinesis 데이터 스트림

B. Amazon S3를 갖춘 Amazon CloudFront

C. 애플리케이션 로드 밸런서가 있는 Amazon EC2 인스턴스

D. Amazon Elastic File System(Amazon EFS)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: B**


설명:

B (정답): 이 조합은 정적 콘텐츠 배포의 표준 아키텍처입니다. S3에 원본 정적 파일(핸드북)을 저장하고, Amazon CloudFront(CDN 서비스)를 사용하여 전 세계 엣지 로케이션에 파일을 캐싱합니다. 이를 통해 사용자들은 가장 가까운 위치에서 파일을 다운로드하여 낮은 지연 시간과 높은 전송 속도를 경험할 수 있습니다.

</details>

46. 어떤 회사에서는 CI/CD(지속적인 통합/지속적인 배포) 파이프라인을 신속하게 구현하려고 합니다. 어떤 AWS 서비스가 이 요구 사항을 충족할까요?

A. AWS 구성

B. Amazon Cognito

C. AWS 데이터 동기화

D. AWS 코드스타

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: D**


설명:

D (정답): AWS CodeStar는 AWS에서 애플리케이션을 신속하게 개발, 빌드 및 배포하기 위한 통합 UI를 제공합니다. 프로젝트 템플릿을 사용하여 전체 CI/CD 파이프라인을 몇 분 만에 설정할 수 있습니다.

A (오답): AWS Config는 AWS 리소스의 구성을 평가, 감사 및 검사하는 서비스입니다.

</details>

47. 회사에서는 Amazon S3에 저장된 문서에서 텍스트를 검색해야 합니다. 어떤 AWS 서비스가 이러한 요구 사항을 충족할까요?

A. 아마존 켄드라

B. 아마존 레코그니션

C. 아마존 폴리

D. 아마존 렉스

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
**정답: A**


설명:

A (정답): Amazon Kendra는 기계 학습 기반의 지능형 검색 서비스입니다. S3와 같은 데이터 소스에 연결하여 사용자가 자연어 질문을 사용하여 문서를 쉽게 찾을 수 있도록 합니다.

B (오답): Amazon Rekognition은 이미지 및 비디오 분석 서비스입니다.

C (오답): Amazon Polly는 텍스트를 음성으로 변환하는 서비스입니다.

D (오답): Amazon Lex는 챗봇을 만드는 서비스입니다.

</details>
