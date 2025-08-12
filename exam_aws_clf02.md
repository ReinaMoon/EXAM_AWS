1. 다음 중 AWS 계정 루트 사용자의 특징은 무엇입니까?

A. 루트 사용자는 다중 인증(MFA)를 구성할 수 있는 유일한 사용자입니다.

B. 루트 사용자는 AWS 관리 콘솔에 액세스할 수 있는 유일한 사용자입니다.

C. 루트 사용자는 AWS 계정이 생성될 때 사용할 수 있는 첫 번째 로그인 아이디입니다.

D. 루트 사용자의 비밀번호는 변경할 수 없습니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> AWS 계정을 처음 만들 때 사용하는 이메일 주소와 암호가 바로 '루트 사용자' 자격 증명입니다. 계정의 모든 권한을 가진 최초의 사용자입니다.

<b>A (오답):</b> MFA(다중 인증)는 루트 사용자뿐만 아니라 모든 IAM 사용자에게도 설정할 수 있으며, 보안을 위해 강력히 권장됩니다.

<b>B (오답):</b> 적절한 권한을 가진 IAM 사용자 역시 AWS 관리 콘솔에 로그인하여 할당된 작업을 수행할 수 있습니다.

<b>D (오답):</b> 루트 사용자의 비밀번호는 변경할 수 있으며, 보안을 위해 정기적으로 변경해야 합니다.

</details>


---

2. 어떤 AWS 기능 또는 리소스가 소프트웨어 및 보안 요구 사항이 미리 패키지된 배포 가능한 Amazon EC2 인스턴스 템플릿입니까?

A. Amazon Elastic Block Store(Amazon EBS) 볼륨

B. AWS CloudFormation 템플릿

C. Amazon Elastic Block Store(Amazon EBS) 스냅샷

D. Amazon 머신 이미지(AMI)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:

<b>D (정답):</b> AMI(Amazon Machine Image)는 EC2 인스턴스를 시작하는 데 필요한 정보를 제공하는 템플릿입니다. 여기에는 운영 체제(OS), 애플리케이션 서버, 애플리케이션 등이 포함됩니다.

<b>B (오답):</b> AWS CloudFormation 템플릿은 EC2 인스턴스뿐만 아니라 VPC, 데이터베이스, 로드 밸런서 등 전체 AWS 인프라를 코드로 정의하고 배포하는 데 사용됩니다. 범위가 훨씬 더 넓습니다.

</details>


---

3. 다음 중 AWS Well-Architected Framework의 핵심 요소는 무엇입니까? (두 가지 선택)

A. 가용성

B. 신뢰성

C. 확장성

D. 반응형 디자인

E. 운영 우수성

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>, <b>E</b>


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


---

4. 보안 엔지니어가 데이터 보안 관련 규정 준수 요건을 충족하기 위해 자체 암호화 키를 생성, 제어 및 관리할 수 있는 단일 테넌트 AWS 솔루션을 원합니다. 이 엔지니어는 어떤 AWS 서비스를 사용해야 합니까?

A. AWS 키 관리 서비스(AWS KMS)

B. AWS 인증서 관리자(ACM)

C. AWS 클라우드HSM

D. AWS 시스템 관리자

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> AWS CloudHSM은 클라우드에서 전용 하드웨어 보안 모듈(HSM)을 제공하는 단일 테넌트 서비스입니다. 사용자가 직접 암호화 키를 완전하게 생성, 제어, 관리할 수 있으며, FIPS 140-2 Level 3과 같은 높은 수준의 규정 준수 요건을 충족합니다.

<b>A (오답):</b> AWS KMS는 암호화 키를 쉽게 생성하고 제어할 수 있는 관리형 서비스이지만, 다중 테넌트 환경이며 AWS가 하드웨어를 관리합니다. 키에 대한 제어 수준이 CloudHSM보다 낮습니다.

</details>


---

5. 일반적인 네트워크 보안 제어 요구사항에 대해, 어떤 AWS 기능이 이러한 요구 사항을 충족합니까? (2개 선택) 

A. 보안 그룹

B. 네트워크 ACL

C. S3 버킷 정책

D. IAM 사용자 정책

E. S3 버킷 버전 관리

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>, <b>B</b>



<b>A. 보안 그룹 (Security Group):</b> EC2 인스턴스 수준에서 인바운드/아웃바운드 트래픽을 제어하는 가상 방화벽입니다.

<b>B. 네트워크 ACL (Network Access Control List):</b> 서브넷 수준에서 트래픽을 제어하는 방화벽입니다.
B(네트워크 ACL)와 D(IAM 정책)는 서로 다른 계층의 보안을 담당합니다. B는 네트워크 트래픽을, D는 사용자/역할의 AWS 서비스 API 호출 권한을 제어합니다.

</details>


---

6. 중단을 견딜 수 있는 상태 비저장 워크로드에 비해 가장 비용 효율적인 Amazon EC2 인스턴스 구매 옵션은 무엇입니까?

A. 스팟 인스턴스

B. 변환 가능한 예약 인스턴스

C. 표준 예약 인스턴스

D. 전용 호스트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>


설명:

<b>A (정답):</b> 스팟 인스턴스는 AWS의 미사용 EC2 용량을 활용하여 온디맨드 요금보다 훨씬 저렴하게 제공됩니다. 하지만 AWS가 해당 용량을 필요로 할 경우 2분 전 알림과 함께 인스턴스가 중단될 수 있습니다. 따라서 "중단을 견딜 수 있는" 워크로드에 가장 비용 효율적입니다.

<b>B, C (오답):</b> 예약 인스턴스는 1년 또는 3년 약정을 통해 상당한 할인을 받으며, 중단되지 않는 안정적인 워크로드에 적합합니다. 스팟 인스턴스보다는 비쌉니다.

</details>


---

7. 대규모로 밀리초 미만의 지연 시간을 제공하는 키-값 데이터베이스인 AWS 서비스는 무엇입니까?

A. Amazon DynamoDB

B. 아마존 오로라

C. Amazon DocumentDB(MongoDB와 호환)

D. 아마존 넵튠

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>


설명:

<b>A (정답):</b> Amazon DynamoDB는 어떤 규모에서든 한 자릿수 밀리초의 성능을 제공하도록 설계된 키-값 및 문서 데이터베이스입니다.

<b>B (오답):</b> Amazon Aurora는 고성능 관계형 데이터베이스(MySQL, PostgreSQL 호환)입니다.

<b>C (오답):</b> Amazon DocumentDB는 MongoDB와 호환되는 문서 데이터베이스이지만, 키-값 데이터베이스는 아닙니다.

</details>


---

8. Amazon S3에 저장된 객체를 보호하는 데 사용할 수 있는 암호화 유형은 무엇입니까? (2개 선택)

A. AmazonS3 관리 암호화 키(SSE-S3)를 사용한 서버 측 암호화

B. AWS KMS 관리 키를 사용한 서버 측 암호화(SSE-KMS)

C. TLS

D. SSL

E. 투명한 데이터 암호화(TDE)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>, <b>B</b>


설명:

<b>A, B (정답):</b> S3에 저장된 데이터(Encryption at rest, 미사용 데이터 암호화)를 보호하기 위해 서버 측 암호화(SSE)를 사용합니다. SSE-S3는 S3가 키를 관리하고, SSE-KMS는 AWS KMS를 통해 키를 관리하여 더 세분화된 제어와 감사 기능을 제공합니다.

<b>C, D (오답):</b> TLS/SSL은 클라이언트와 서버 간에 **전송 중인 데이터(Encryption in transit)**를 암호화하는 프로토콜입니다. S3에 이미 저장된 객체를 보호하는 것과는 목적이 다릅니다.

</details>


---

9. 한 회사는 통합 청구를 위해 AWS Organizations의 조직에 두 개의 AWS 계정을 가지고 있습니다. 계정 A는 Amazon EC2 Standard Reserved Instances(RI) 5개를 구매했습니다. 계정 A는 EC2 인스턴스 4개를 실행 중입니다. 계정 B는 RI를 구매하지 않았고 EC2 인스턴스 4개를 실행 중입니다. 이 8가지 인스턴스에 대한 설명으로 옳은 것은 무엇입니까?

A. 8개의 인스턴스는 일반 인스턴스로 요금이 청구됩니다.

B. 인스턴스 4개는 RI로 청구되고, 인스턴스 4개는 일반 인스턴스로 청구됩니다.

C. 인스턴스 5개는 RI로 청구되고, 인스턴스 3개는 일반 인스턴스로 청구됩니다.

D. 8개의 인스턴스는 RI로 청구됩니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:
AWS Organizations의 통합 청구에서는 기본적으로 RI 할인이 조직 내 모든 계정 간에 공유됩니다.

계정 A가 구매한 RI 5개는 먼저 구매한 계정 A의 인스턴스 4개에 적용됩니다.

이제 남은 RI 1개가 있습니다. 이 남은 RI 할인은 조직 내 다른 계정인 계정 B의 인스턴스 1개에 적용됩니다.

따라서, 총 5개(계정 A의 4개 + 계정 B의 1개)의 인스턴스가 RI로 청구되고, 계정 B의 나머지 인스턴스 3개는 온디맨드(일반) 요금으로 청구됩니다.

</details>


---

10. 어떤 AWS 서비스가 사용자가 여러 Lambda 함수 세트에 대한 워크플로를 조율하고 프로세스를 조율하는 데 도움을 주도록 설계되었습니까?

A. Amazon DynamoDB

B. AWS 코드 파이프라인

C. AWS 배치

D. AWS Step Functions

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:

<b>D (정답):</b> AWS Step Functions는 Lambda 함수와 같은 여러 AWS 서비스를 시각적인 워크플로로 **조율(Orchestration)**하는 서버리스 서비스입니다. "A 함수 실행 후 성공하면 B 함수, 실패하면 C 함수 실행"과 같은 복잡한 흐름을 관리합니다.

<b>B (오답):</b> AWS CodePipeline은 소스 코드 변경 시 자동으로 빌드, 테스트, 배포하는 CI/CD 파이프라인을 자동화하는 서비스입니다.

<b>C (오답):</b> AWS Batch는 대규모 배치 컴퓨팅 작업을 효율적으로 실행하는 서비스입니다.

</details>


---

11. 한 회사가 타사 소프트웨어 서비스(SaaS) 애플리케이션에 대한 액세스 및 권한을 관리하려고 합니다. 이 회사는 최종 사용자가 할당된 계정 및 AWS 클라우드 애플리케이션에 액세스할 수 있는 포털을 원합니다. 이러한 요구 사항을 충족하기 위해 회사는 어떤 AWS 서비스를 사용해야 합니까?

A. Amazon Cognito

B. AWS IAM Identity Center(AWS Single Sign-On)

C. AWS ID 및 액세스 관리(IAM)

D. Microsoft Active Directory용 AWS 디렉터리 서비스

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>


설명:

<b>B (정답):</b> AWS IAM Identity Center (이전 명칭: AWS SSO)는 여러 AWS 계정 및 Salesforce, Office 365와 같은 **클라우드 애플리케이션(SaaS)**에 대한 Single Sign-On (SSO) 액세스를 중앙에서 관리하는 서비스입니다. 사용자는 포털을 통해 할당된 모든 애플리케이션에 접근할 수 있습니다.

<b>A (오답):</b> Amazon Cognito는 개발하는 웹/모바일 앱의 **고객(외부 사용자)**들이 회원가입, 로그인하는 기능을 제공하는 서비스입니다. 회사 내부 직원의 SSO와는 용도가 다릅니다.

</details>


---

12. 회사에서는 AWS 지출 목표를 설정하고 목표에 따른 비용을 추적하려고 합니다. 이러한 요구 사항을 충족하기 위해 회사는 어떤 AWS 도구나 기능을 사용해야 합니까?

A. AWS 비용 탐색기

B. AWS 예산

C. AWS 비용 및 사용 보고서

D. 저축 계획

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>


설명:

<b>B (정답):</b> AWS Budgets는 사용자 지정 비용 및 사용량 예산을 설정하고, 실제 또는 예측 비용이 예산을 초과할 때 알림을 받도록 하는 기능입니다. "목표 설정 및 추적"이라는 요구사항에 가장 부합합니다.

<b>A (오답):</b> AWS Cost Explorer는 과거의 비용을 시각화하고 분석하는 도구입니다. 예산을 설정하고 알림을 보내는 기능은 없습니다.

</details>


---

13. 가용성 영역의 특징은 무엇입니까? (2개 선택)

A. AWS 지역의 모든 가용성 영역은 대역폭이 높고 지연 시간이 짧은 네트워킹으로 상호 연결됩니다.

B. 가용성 영역은 물리적으로 최소 150km(100마일)의 거리로 분리되어 있습니다.

C. 가용성 영역 간의 모든 트래픽은 암호화됩니다.

D. AWS 지역 내의 가용성 영역은 중복된 전원, 네트워킹 및 연결을 공유합니다.

E. 모든 가용성 영역에는 단일 데이터 센터가 포함됩니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>, <b>C</b>


설명:

<b>A (정답):</b> 가용성 영역(AZ)들은 낮은 지연 시간과 높은 대역폭을 가진 전용 광섬유 네트워크로 연결되어 있어, AZ 간에 데이터를 빠르게 복제할 수 있습니다.

<b>C (정답):</b> AWS 글로벌 네트워크 백본을 통과하는 AZ 간 트래픽은 물리 계층에서 자동으로 암호화됩니다.

<b>D (오답):</b> 가용성 영역은 독립적인 전원, 냉각, 물리적 보안을 갖도록 설계되어 서로의 장애에 영향을 받지 않습니다.

<b>E (오답):</b> 가용성 영역은 하나 이상의 개별 데이터 센터로 구성될 수 있습니다.

</details>


---

14. 한 회사가 타사 ID 공급자(IdP)를 사용합니다. 이 회사는 다른 로그인 자격 증명을 요구하지 않고 직원들에게 AWS 계정 및 서비스에 대한 액세스 권한을 제공하고자 합니다. 어떤 AWS 서비스가 이 요구 사항을 충족할까요?

A. Amazon Cognito

B. AWS 리소스 액세스 관리자(AWS RAM)

C. AWS 디렉터리 서비스

D. AWS IAM ID 센터

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:
이 문제는 11번 문제와 거의 동일합니다.

<b>D (정답):</b> AWS IAM Identity Center는 Okta, Azure AD와 같은 타사 IdP와 연동하여 직원들이 기존 회사 자격 증명으로 AWS 계정에 **SSO(Single Sign-On)**할 수 있도록 지원합니다.

<b>A (오답):</b> Amazon Cognito는 개발하는 앱의 고객 인증용입니다.

</details>


---

15. 회사에서는 모든 프로세스가 효과적이고 직원이 프로세스에 익숙한지 검토하기 위해 작업 흐름을 시뮬레이션합니다. 이 관행에서 회사는 AWS Well-Architected Framework의 어떤 설계 원칙을 따릅니까?

A. 코드로 작업을 수행합니다.

B. 작업 절차를 자주 수정하세요.

C. 작고 되돌릴 수 있는 변경을 자주 만드세요.

D. 비즈니스 성과를 지원하도록 회사를 구성합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:
이 활동은 운영 우수성(Operational Excellence) 기둥과 관련이 있습니다. 작업 흐름을 시뮬레이션(Game days)하는 것은 운영 절차를 검증하고 개선하여 비즈니스 목표를 달성하기 위함입니다.

<b>D (정답):</b> "비즈니스 성과를 지원하도록 회사를 구성합니다"는 운영 우수성의 상위 목표를 가장 잘 나타냅니다. 효과적인 프로세스를 통해 비즈니스 가치를 창출하는 것이 핵심입니다.

<b>A, C (오답):</b> 이들은 운영 우수성의 다른 중요한 원칙들이지만, '프로세스 검토 및 시뮬레이션'이라는 활동보다는 '배포 자동화 및 변경 관리'와 더 직접적으로 관련됩니다.

</details>


---

16. 회사에서는 사업부에서 더 이상 액세스할 필요가 없는 Amazon S3 데이터를 보관해야 합니다. 어떤 S3 스토리지 클래스가 이 요구 사항을 가장 비용 효율적으로 충족할까요?

A. S3 Glacier 즉시 검색

B. S3 Glacier 유연한 검색

C. S3 빙하 심층 아카이브

D. S3 One Zone-Infrequent Access(S3 One Zone-IA)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> S3 Glacier Deep Archive는 가장 저렴한 스토리지 비용을 제공하며, 수년에 한두 번 액세스하는 데이터의 **장기 보관(아카이빙)**을 위해 설계되었습니다.

<b>A, B (오답):</b> Glacier Instant/Flexible Retrieval은 Deep Archive보다 스토리지 비용이 비싸지만 데이터 검색 속도가 더 빠릅니다.

</details>


---

17. 회사에서는 특정 Amazon EC2 인스턴스에 보안 규칙을 적용해야 합니다. 어떤 AWS 서비스나 기능이 이 기능을 제공합니까?

A. AWS 쉴드

B. 네트워크 ACL

C. 보안 그룹

D. AWS 방화벽 관리자

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> 보안 그룹(Security Group)은 개별 EC2 인스턴스에 연결되어 인바운드 및 아웃바운드 트래픽을 제어하는 상태 저장(stateful) 가상 방화벽 역할을 합니다.

<b>B (오답):</b> 네트워크 ACL은 서브넷 수준에서 작동하며, 해당 서브넷 내의 모든 인스턴스에 영향을 미치는 상태 비저장(stateless) 방화벽입니다.

</details>


---

18. 한 회사가 고성능 컴퓨팅(HPC) 워크로드를 위해 설계된 데이터 레이어가 있습니다. 이 회사는 이러한 요구 사항을 충족하기 위해 어떤 Amazon EC2 인스턴스 유형을 사용해야 합니까?

A. 저장소 최적화

B. 일반 목적

C. 메모리 최적화

D. 최적화된 인스턴스 계산

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:

<b>D (정답):</b> 컴퓨팅 최적화 (Compute Optimized) 인스턴스 (예: C 계열)는 고성능 프로세서를 갖추고 있어 HPC, 배치 처리, 미디어 트랜스코딩과 같이 CPU 집약적인 워크로드에 이상적입니다.

</details>


---

19. Amazon Aurora는 어떤 데이터베이스 엔진을 지원합니까? (2개 선택)

A. 오라클

B. 마이크로소프트 SQL 서버

C. MySQL

D. PostgreSQL

E. MariaDB

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>, <b>D</b>


설명:

<b>C, D (정답):</b> Amazon Aurora는 클라우드에 맞게 구축된 관계형 데이터베이스로, MySQL 및 PostgreSQL과 완벽하게 호환됩니다. 기존 애플리케이션을 거의 변경 없이 마이그레이션할 수 있습니다.

</details>


---

20. VPC에 인터넷 게이트웨이를 두는 목적은 무엇입니까?

A. VPC에 VPN 연결을 생성하려면

B. VPC와 인터넷 간 통신을 허용합니다.

C. 인터넷 트래픽에 대역폭 제한을 부과합니다.

D. Amazon EC2 인스턴스 전반에서 인터넷 트래픽의 부하를 분산하려면

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>


설명:

<b>B (정답):</b> 인터넷 게이트웨이(IGW)는 VPC와 인터넷 간의 통신을 가능하게 하는 VPC의 구성 요소입니다. IGW가 연결된 VPC 내의 리소스(예: 퍼블릭 서브넷의 EC2 인스턴스)는 인터넷에 접근할 수 있습니다.

</details>


---

21. AWS Trusted Advisor는 어떤 범주에서 권장 조치를 제공합니까? (2개 선택)

A. 운영 체제 패치

B. 비용 최적화

C. 반복적인 작업

D. 서비스 할당량

E. 계정 활동 기록

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>, <b>D</b>


설명:
AWS Trusted Advisor는 5가지 범주에서 모범 사례 권장 사항을 제공합니다.

비용 최적화 (Cost Optimization)

성능 (Performance)

보안 (Security)

내결함성 (Fault Tolerance)

서비스 한도 (Service Quotas)

</details>


---

22. 알려지지 않은 액세스 패턴에 대해 가장 비용 효율적인 Amazon S3 스토리지 클래스는 무엇입니까?

A. S3 표준

B. S3 Standard-Infrequent Access(S3 Standard-IA)

C. S3 One Zone-Infrequent Access(S3 One Zone-IA)

D. S3 지능형 계층화

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:

<b>D (정답):</b> S3 Intelligent-Tiering은 객체의 액세스 패턴을 모니터링하고, 액세스 빈도에 따라 데이터를 가장 비용 효율적인 스토리지 계층으로 자동으로 이동시키는 서비스입니다. 따라서 "알려지지 않았거나 변경되는" 액세스 패턴에 가장 적합합니다.

</details>


---

23. 어떤 회사는 AWS 클라우드를 자사 온프레미스 인프라의 오프사이트 백업 위치로 사용하려고 합니다. 어떤 AWS 서비스가 이 요구 사항을 가장 비용 효율적으로 충족할 수 있을까요?

A. 아마존 S3

B. Amazon Elastic File System(Amazon EFS)

C. 아마존 FSx

D. Amazon Elastic Block Store(Amazon EBS)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>


설명:

<b>A (정답):</b> Amazon S3는 내구성이 매우 높고 확장 가능하며 비용 효율적인 객체 스토리지 서비스로, 백업 및 아카이빙에 가장 이상적이고 널리 사용됩니다. 다양한 스토리지 클래스와 수명 주기 정책을 통해 비용을 더욱 최적화할 수 있습니다.

</details>


---

24. 사용자는 Amazon EC2 인스턴스에서 실행되는 애플리케이션이 다른 AWS 서비스를 호출할 수 있도록 허용하려고 합니다. 허용된 액세스는 안전해야 합니다. 어떤 AWS 서비스 또는 기능을 사용해야 합니까?

A. 보안 그룹

B. AWS 방화벽 관리자

C. IAM 역할

D. IAM 사용자 SSH 키

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> **IAM 역할(Role)**은 EC2 인스턴스와 같은 AWS 리소스에 권한을 부여하는 가장 안전하고 권장되는 방법입니다. 역할은 임시 보안 자격 증명을 사용하여 다른 서비스에 액세스하므로, 액세스 키와 같은 장기 자격 증명을 코드에 하드코딩할 필요가 없습니다.

</details>


---

25. 한 회사는 지속 가능성 영역에 대한 목표를 달성하는 방법을 파악하기 위해 사용자 행동 패턴을 수집하고 있습니다. 이러한 목표를 달성하기 위해 회사가 구현해야 할 모범 사례는 무엇입니까? (2개 선택)

A. 사용자 부하에 따라 인프라를 확장합니다.

B. 작업 부하와 사용자 위치 간의 지리적 거리를 최대화합니다.

C. 사용되지 않는 자산의 생성 및 유지 관리를 제거합니다.

D. 여유 용량이 있는 리소스를 확장하고 자동 크기 조정을 제거합니다.

E. 사용자 수에 따라 인프라를 확장합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>, <b>C</b> (또는 <b>A</b>, <b>E</b>)


설명:
AWS Well-Architected Framework의 지속 가능성 기둥은 낭비를 줄이고 활용률을 극대화하는 것을 목표로 합니다.

<b>A, E (정답):</b> "사용자 부하/수"에 따라 인프라를 확장하는 것은 수요에 맞게 공급을 조정하는 것으로, 불필요한 리소스 사용을 막는 핵심 원칙입니다.

<b>C (정답):</b> 사용하지 않는 리소스를 제거하는 것은 직접적인 낭비 제거에 해당합니다.

<b>D (오답):</b> 여유 용량을 과도하게 두고 자동 크기 조정을 제거하는 것은 과잉 프로비저닝으로 이어져 지속 가능성에 반하는 행위입니다.

</details>


---

26. AWS는 수십만 명의 사용자의 사용량을 집계하여 더 낮은 종량제 가격을 책정할 수 있는 역량을 갖추고 있습니다. 이는 AWS 클라우드의 어떤 장점을 설명합니까?

A. 몇 분 안에 전 세계적으로 출시

B. 속도와 민첩성 증가

C. 규모의 경제성이 높음

D. 컴퓨팅 용량에 대한 추측 없음

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> **규모의 경제(Economies of scale)**는 AWS가 대규모로 운영함으로써 얻는 비용 절감 효과를 고객에게 더 낮은 가격으로 제공할 수 있음을 의미합니다. 수많은 사용자의 사용량을 집계하는 것이 바로 그 예입니다.

</details>


---

27. 어떤 AWS 클라우드 배포 모델이 애플리케이션 배포 인프라의 일부로 AWS Outposts를 사용합니까?

A. 온프레미스

B. 서버리스

C. 클라우드 네이티브

D. 하이브리드

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:

<b>D (정답):</b> AWS Outposts는 AWS 인프라와 서비스를 고객의 온프레미스 데이터 센터로 확장하는 서비스입니다. 이는 온프레미스 환경과 AWS 클라우드를 원활하게 연결하는 하이브리드 클라우드 모델의 핵심 요소입니다.

</details>


---

28. 회사에서는 SQL 주입 공격을 차단해야 합니다. 어떤 AWS 서비스나 기능이 이 요구 사항을 충족할 수 있을까요?

A. AWS WAF

B. AWS 쉴드

C. 네트워크 ACL

D. 보안 그룹

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>


설명:

<b>A (정답):</b> **AWS WAF (Web Application Firewall)**는 웹 애플리케이션을 보호하는 L7 방화벽으로, SQL 주입, 크로스 사이트 스크립팅(XSS)과 같은 일반적인 웹 공격을 탐지하고 차단하는 규칙을 생성할 수 있습니다.

<b>B, C, D (오답):</b> Shield(DDoS 방어), NACL/보안 그룹(네트워크 트래픽 제어)은 SQL 주입과 같은 애플리케이션 계층의 공격 콘텐츠를 분석하지 않습니다.

</details>


---

29. 어떤 AWS 데이터베이스 서비스가 메모리 내 데이터 스토리를 제공합니까?

A. Amazon DynamoDB

B. 아마존 엘라스티캐시

C. 아마존 RDS

D. 아마존 타임스트림

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>


설명:

<b>B (정답):</b> Amazon ElastiCache는 Redis 및 Memcached와 호환되는 완전 관리형 인메모리(in-memory) 데이터 스토어 또는 캐시 서비스입니다. 빠른 응답 시간이 필요한 애플리케이션의 성능을 향상시키는 데 사용됩니다.

</details>


---

30. 한 회사가 고성능 컴퓨팅(HPC) 애플리케이션을 Amazon EC2 인스턴스로 마이그레이션하려고 합니다. 애플리케이션에는 여러 구성 요소가 있습니다. 애플리케이션에는 내결함성이 있어야 하며 자동 장애 조치가 가능한 기능이 있어야 합니다. 구성 요소 간 지연 시간을 최소화하면서 이러한 요구 사항을 충족하는 AWS 인프라 솔루션은 무엇입니까?

A. 여러 AWS 지역

B. 다중 예지 위성

C. 다중 가용성 영역

D. 지역 에지 캐시

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> **다중 가용성 영역(Multi-AZ)**에 애플리케이션 구성 요소를 배포하는 것은 내결함성을 확보하는 표준 방법입니다. 하나의 AZ에 장애가 발생해도 다른 AZ의 구성 요소가 계속 작동합니다. 또한, 같은 리전 내의 AZ들은 낮은 지연 시간으로 연결되어 있어 구성 요소 간 통신 성능 저하를 최소화할 수 있습니다.

<b>A (오답):</b> 여러 AWS 지역은 재해 복구에는 좋지만, 지역 간 거리가 멀어 지연 시간이 높기 때문에 구성 요소 간 통신에는 적합하지 않습니다.

</details>


---

31. 한 회사가 온프레미스 데이터 웨어하우스를 AWS로 마이그레이션하려고 합니다. 데이터 웨어하우스의 정보는 분석 대시보드를 채우는 데 사용됩니다. 이 회사는 데이터 웨어하우스에 어떤 AWS 서비스를 사용해야 합니까?

A. Amazon ElastiCache

B. 아마존 오로라

C. 아마존 RDS

D. 아마존 레드쉬프트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:

<b>D (정답):</b> Amazon Redshift는 페타바이트 규모의 완전 관리형 데이터 웨어하우스(Data Warehouse) 서비스입니다. 대규모 데이터 세트에 대한 복잡한 쿼리를 빠르게 실행할 수 있어 분석 및 비즈니스 인텔리전스(BI) 대시보드에 이상적입니다.

</details>


---

32. 어떤 회사는 VPC에서 Amazon EC2 인스턴스를 실행하고 있습니다. 전자상거래 회사는 Amazon EC2에서 실행되는 웹 서버를 관리하기 위해 Amazon EC2 Auto Scaling 그룹을 사용하고 있습니다. 이 아키텍처는 어떤 AWS Well-Architected Framework 모범 사례를 따르나요?

A. 작업 부하를 확보하세요

B. 인프라 구성요소 분리

C. 실패를 위한 디자인

D. 병렬적으로 생각해보세요

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> Auto Scaling 그룹은 상태 확인에 실패한 인스턴스를 자동으로 종료하고 새 인스턴스로 교체합니다. 이는 구성 요소의 장애가 전체 시스템의 장애로 이어지지 않도록 하는 **실패를 위한 설계(Design for Failure)**의 대표적인 예시이며, 신뢰성(Reliability) 기둥의 핵심 원칙입니다.

</details>


---

33. 어떤 AWS 서비스가 사용자가 AWS 인프라, AWS 서비스, API 및 도구를 데이터 센터, 콜로케이션 환경 또는 온프레미스 시설로 확장할 수 있는 하이브리드 아키텍처를 지원하는 AWS 서비스는 무엇입니까?

A. AWS 스노모빌

B. AWS 로컬 영역

C. AWS 아웃포스트

D. AWS Fargate

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> AWS Outposts는 AWS 인프라, 서비스, API 및 도구를 고객의 데이터 센터, 코로케이션 환경 또는 온프레미스 시설로 확장하여 진정한 하이브리드 경험을 제공하는 서비스입니다.

</details>


---

34. 회사에서 서버리스 애플리케이션을 시각적으로 디자인하고 구축하는 데 사용할 수 있는 AWS 서비스는 무엇입니까?

A. AWS 람다

B. AWS 배치

C. AWS 애플리케이션 컴포저

D. AWS App Runner

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> AWS Application Composer는 AWS 서비스를 드래그 앤 드롭 방식으로 연결하여 서버리스 애플리케이션 아키텍처를 시각적으로 설계하고, 이를 CloudFormation 또는 SAM 템플릿으로 생성해주는 도구입니다.

</details>


---

35. 가용성 영역은 다음으로 구성됩니다.

A. 단일 위치에 있는 하나 이상의 데이터 센터.

B. 여러 지역에 위치한 두 개 이상의 데이터 센터.

C. 단일 데이터 센터에 있는 하나 이상의 물리적 호스트.

D. 여러 데이터 센터에 있는 두 개 이상의 물리적 호스트.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>


설명:

<b>A (정답):</b> 가용성 영역(AZ)은 하나 이상의 개별 데이터 센터로 구성되며, 각 데이터 센터는 중복 전원, 네트워킹 및 연결 기능을 갖추고 있습니다. 이들은 하나의 AWS 리전 내에 물리적으로 격리된 위치에 있습니다.

</details>


---

36. 어떤 회사에서는 AWS 계정의 모든 사용자 목록, 모든 사용자의 액세스 키 상태, 그리고 다중 요소 인증(MFA)이 구성되었는지 여부를 알고 싶어합니다. 어떤 AWS 서비스나 기능이 이러한 요구 사항을 충족할까요?

A. AWS 키 관리 서비스(AWS KMS)

B. IAM 액세스 분석기

C. IAM 자격 증명 보고서

D. Amazon CloudWatch

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:

<b>C (정답):</b> **IAM 자격 증명 보고서(Credential Report)**는 계정의 모든 사용자와 암호, 액세스 키, MFA 장치 상태 등 다양한 자격 증명 상태에 대한 정보를 나열하는 CSV 보고서를 제공합니다.

<b>B (오답):</b> IAM Access Analyzer는 계정 외부의 엔터티와 공유되어 의도하지 않은 접근을 허용할 수 있는 리소스를 식별하는 데 도움이 됩니다.

</details>


---

37. 강사가 진행하는 환경에서 어떤 클라우드 보안에 대해 배우고자 택하세요? (2가지를 선택하세요.)

A. AWS 신뢰할 수 있는 고문

B. AWS 온라인 기술 토크

C. AWS 블로그

D. AWS 포럼

E. AWS 강의실 교육

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>, <b>E</b>


설명:
"강사가 진행하는 환경"은 실시간으로 전문가의 설명을 들을 수 있는 교육을 의미합니다.

<b>E (정답):</b> AWS 강의실 교육은 공인 강사가 직접 진행하는 공식 교육 과정입니다.

<b>B (정답):</b> AWS 온라인 기술 토크는 AWS 전문가가 특정 주제에 대해 온라인으로 진행하는 웨비나 형식의 세션입니다.

<b>A (오답):</b> Trusted Advisor는 AWS 계정의 상태를 점검해주는 서비스이지 학습 리소스가 아닙니다.

</details>


---

38. 어떤 회사는 고객 경험에 대한 통찰력을 얻기 위해 서버 로그를 쿼리하려고 합니다. 어떤 서비스가 이 데이터를 가장 비용 효율적으로 저장할 수 있을까요?

A. 아마존 오로라

B. Amazon Elastic File System(Amazon EFS)

C. Amazon Elastic Block Store(Amazon EBS)

D. Amazon S3

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:

<b>D (정답):</b> 서버 로그와 같은 대량의 비정형 데이터를 가장 저렴하게 저장하고 나중에 쿼리(예: Athena 사용)하는 데는 Amazon S3가 가장 적합합니다. 저렴한 스토리지 클래스(예: S3 Standard-IA)와 라이프사이클 정책을 통해 비용을 더욱 최적화할 수 있습니다.

<b>A, B, C (오답):</b> 관계형 데이터베이스(Aurora)나 파일/블록 스토리지(EFS/EBS)는 대량의 로그를 저장하는 데 S3보다 훨씬 비쌉니다.

</details>


---

39. 회사에서는 고객에게 Amazon S3 버킷에 호스팅된 특정 데이터를 볼 수 있는 기능을 제공하려고 합니다. 회사는 고객과 공유하는 전체 데이터 세트를 계속 제어하려고 합니다. 이러한 요구 사항을 충족하는 S3 기능은 무엇입니까?

A. S3 스토리지 렌즈

B. S3 크로스 리전 복제(CRR)

C. S3 버전 관리

D. S3 액세스 포인트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:

<b>D (정답):</b> **S3 액세스 포인트(Access Point)**는 대규모 데이터 세트에 대한 액세스 관리를 간소화하는 기능입니다. 각 액세스 포인트에 고유한 정책과 네트워크 제어를 적용하여, 특정 사용자나 애플리케이션 그룹에 세분화된 데이터 액세스 권한을 쉽게 부여할 수 있습니다.

</details>


---

40. 한 회사가 보안 네트워크 연결을 통해 원격 직원에게 관리되는 Windows 가상 데스크톱과 애플리케이션을 제공하고자 합니다. 이 회사는 이러한 요구 사항을 충족하기 위해 어떤 AWS 서비스를 사용할 수 있습니까? (두 가지를 선택하세요.)

A. 아마존 커넥트

B. Amazon AppStream 2.0

C. Amazon 작업 공간

D. AWS 사이트 간 VPN

E. Amazon Elastic Container Service(Amazon ECS)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>, <b>C</b>


설명:

<b>C (정답):</b> Amazon WorkSpaces는 완전 관리형의 안전한 클라우드 기반 가상 데스크톱(DaaS) 서비스입니다. 사용자에게 Windows 또는 Linux 데스크톱을 제공합니다.

<b>B (정답):</b> Amazon AppStream 2.0은 데스크톱 애플리케이션을 중앙에서 관리하고 모든 컴퓨터의 사용자에게 안전하게 스트리밍하는 서비스입니다. 가상 데스크톱 기능도 제공합니다.

</details>


---

41. 한 회사가 애플리케이션에 대한 인터넷 트래픽이 단기적으로 급증할 것으로 예상하고 있습니다. 트래픽이 증가하는 동안 애플리케이션은 중단될 수 없습니다. 또한 회사는 비용을 최소화하고 유연성을 극대화해야 합니다. 회사는 Amazon S3의 데이터를 분석하기 위해 서버리스 대화형 쿼리 서비스를 사용해야 합니다. 쿼리 서비스는 표준 SQL을 지원해야 합니다. 어떤 AWS 서비스가 이러한 요구 사항을 충족할까요?

A. 아마존 레드쉬프트

B. AWS Glue

C. Amazon Athena

D. Amazon Kinesis 데이터 스트림

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>C</b>


설명:
"S3 데이터 분석", "서버리스 대화형 쿼리", "표준 SQL"은 Amazon Athena를 가리키는 핵심 키워드입니다.

<b>C (정답):</b> Amazon Athena는 S3에 저장된 데이터를 표준 SQL을 사용하여 직접 쿼리할 수 있는 서버리스 대화형 쿼리 서비스입니다. 인프라를 관리할 필요가 없고 쿼리한 데이터 양에 대해서만 비용을 지불하므로 비용 효율적입니다.

</details>


---

42. 전자상거래 회사가 Amazon EC2 인스턴스에 새로운 웹 애플리케이션을 배포했습니다. 이 회사는 들어오는 HTTP 트래픽을 모든 실행 중인 인스턴스에 고르게 분산하려고 합니다. 어떤 AWS 서비스나 리소스가 이 요구 사항을 충족할까요?

A. 게이트웨이 로드 밸런서

B. 애플리케이션 로드 밸런서

C. 네트워크 로드 밸런서

D. Amazon EC2 자동 확장

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>


설명:

<b>B (정답):</b> **Application Load Balancer (ALB)**는 OSI 모델의 7계층(애플리케이션 계층)에서 작동하며, HTTP 및 HTTPS 트래픽의 라우팅에 최적화되어 있습니다.

<b>C (오답):</b> Network Load Balancer (NLB)는 4계층(전송 계층)에서 작동하며, TCP/UDP 트래픽에 대한 초고성능 로드 밸런싱에 적합합니다.

<b>D (오답):</b> Auto Scaling은 트래픽에 따라 인스턴스 수를 자동으로 조절하는 기능이며, 트래픽을 분산하는 기능은 아닙니다.

</details>


---

43. 회사의 컴퓨팅 작업 부하가 안정적이고 예측 가능하며 중단되지 않습니다. 이러한 요구 사항을 가장 비용 효율적으로 충족하는 Amazon EC2 인스턴스 구매 옵션은 무엇입니까? (2개 선택)

A. 주문형 인스턴스

B. 예약된 인스턴스

C. 스팟 인스턴스

D. 저축 계획

E. 전용 호스트

<details markdown=1><summary markdown='span'>정답</summary>
정답: <b>B</b>, <b>D</b>


설명:
"안정적이고 예측 가능한" 워크로드에 대한 비용 절감은 약정 기반 옵션을 통해 이루어집니다.

<b>B (정답):</b> **예약 인스턴스(Reserved Instances, RI)**는 특정 인스턴스 유형 및 리전에 대해 1년 또는 3년 약정을 통해 온디맨드 요금보다 상당한 할인을 제공합니다.

<b>D (정답):</b> Savings Plans는 특정 인스턴스 제품군 및 리전 내에서 시간당 컴퓨팅 사용량(USD/시간)에 대해 약정하여 유연하게 할인을 받을 수 있는 모델입니다. RI보다 유연성이 높습니다.

</details>


---

44. 장기 보관에 가장 비용 효율적인 Amazon S3 스토리지 클래스는 무엇입니까?

A. S3 빙하 심층 아카이브

B. S3 표준

C. S3 Standard-Infrequent Access(S3 Standard-IA)

D. S3 One Zone-Infrequent Access(S3 One Zone-IA)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>


설명:
이 문제는 16번 문제와 동일합니다.

<b>A (정답):</b> S3 Glacier Deep Archive는 가장 저렴한 스토리지 비용을 제공하며, 수년에 한두 번 액세스하는 데이터의 **장기 보관(아카이빙)**을 위해 설계되었습니다.

</details>


---

45. 한 회사가 AWS에서 재설계된 웹사이트를 출시할 준비를 하고 있습니다. 전 세계 사용자가 웹사이트에서 디지털 핸드북을 다운로드할 것입니다. 회사에서는 정적 파일을 안전하게 제공하기 위해 어떤 AWS 솔루션을 사용해야 할까요?

A. Amazon Kinesis 데이터 스트림

B. Amazon S3를 갖춘 Amazon CloudFront

C. 애플리케이션 로드 밸런서가 있는 Amazon EC2 인스턴스

D. Amazon Elastic File System(Amazon EFS)

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>B</b>


설명:

<b>B (정답):</b> 이 조합은 정적 콘텐츠 배포의 표준 아키텍처입니다. S3에 원본 정적 파일(핸드북)을 저장하고, Amazon CloudFront(CDN 서비스)를 사용하여 전 세계 엣지 로케이션에 파일을 캐싱합니다. 이를 통해 사용자들은 가장 가까운 위치에서 파일을 다운로드하여 낮은 지연 시간과 높은 전송 속도를 경험할 수 있습니다.

</details>


---

46. 어떤 회사에서는 CI/CD(지속적인 통합/지속적인 배포) 파이프라인을 신속하게 구현하려고 합니다. 어떤 AWS 서비스가 이 요구 사항을 충족할까요?

A. AWS 구성

B. Amazon Cognito

C. AWS 데이터 동기화

D. AWS 코드스타

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>D</b>


설명:

<b>D (정답):</b> AWS CodeStar는 AWS에서 애플리케이션을 신속하게 개발, 빌드 및 배포하기 위한 통합 UI를 제공합니다. 프로젝트 템플릿을 사용하여 전체 CI/CD 파이프라인을 몇 분 만에 설정할 수 있습니다.

<b>A (오답):</b> AWS Config는 AWS 리소스의 구성을 평가, 감사 및 검사하는 서비스입니다.

</details>


---

47. 회사에서는 Amazon S3에 저장된 문서에서 텍스트를 검색해야 합니다. 어떤 AWS 서비스가 이러한 요구 사항을 충족할까요?

A. 아마존 켄드라

B. 아마존 레코그니션

C. 아마존 폴리

D. 아마존 렉스

<details markdown=1><summary markdown='span'>정답 및 설명</summary>
정답: <b>A</b>


설명:

<b>A (정답):</b> Amazon Kendra는 기계 학습 기반의 지능형 검색 서비스입니다. S3와 같은 데이터 소스에 연결하여 사용자가 자연어 질문을 사용하여 문서를 쉽게 찾을 수 있도록 합니다.

<b>B (오답):</b> Amazon Rekognition은 이미지 및 비디오 분석 서비스입니다.

<b>C (오답):</b> Amazon Polly는 텍스트를 음성으로 변환하는 서비스입니다.

<b>D (오답):</b> Amazon Lex는 챗봇을 만드는 서비스입니다.

</details>


---

48. 아래 옵션 중 AWS의 안정성과 관련된 것은 무엇입니까? (2개 선택)

A. 모든 AWS 리소스에 최소 권한의 원칙을 적용합니다.

B. 수요를 충족하기 위해 자동으로 새로운 리소스를 프로비저닝합니다.

C. 모든 AWS 서비스는 글로벌 서비스로 간주되며, 이러한 설계는 고객이 국제 사용자에게 서비스를 제공하는 데 도움이 됩니다.

D. 문제 발생 시 고객에게 보상을 제공합니다.

E. 실패로부터 빠르게 복구할 수 있는 능력.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B, E</b>

<b>설명:</b> '안정성(Reliability)'의 핵심은 시스템이 장애가 발생해도 의도한 대로 계속 작동하고, 장애가 발생하면 자동으로 복구하는 능력입니다.

<b>B (정답):</b> 수요에 따라 리소스를 자동 프로비저닝(Auto Scaling)하는 것은, 특정 인스턴스에 장애가 발생했을 때 자동으로 새로운 인스턴스로 교체하여 서비스 중단을 막는 핵심적인 안정성 원칙입니다.

<b>E (정답):</b> '실패로부터의 복구 능력'은 안정성 원칙 그 자체를 정의하는 가장 직접적인 설명입니다.

<b>A (오답):</b> '최소 권한의 원칙'은 안정성이 아닌 **보안(Security)** 원칙의 핵심입니다.

<b>C (오답):</b> 모든 AWS 서비스가 글로벌 서비스는 아닙니다(대부분 리전 서비스). 또한 글로벌 서비스 제공은 주로 **성능 효율성(Performance Efficiency)**과 관련이 깊습니다.

<b>D (오답):</b> 보상은 기술적인 안정성 원칙이 아닌 서비스 수준 계약(SLA)과 관련된 비즈니스 정책입니다.

</details>

---

49. AWS Snowball은 무엇을 제공합니까? (두 가지 선택)

A. 고객이 로컬로 데이터를 처리할 수 있는 내장 컴퓨팅 기능

B. 고객이 솔루션을 구축하고 사업을 운영하는 데 필요한 타사 소프트웨어 솔루션 카탈로그

C. 온프레미스 환경과 AWS 클라우드 간의 하이브리드 클라우드 스토리지

D. 엄청나게 많은 양의 데이터를 AWS로 옮길 수 있는 엑사바이트 규모의 데이터 전송 서비스입니다.

E. AWS에서 대량의 데이터를 안전하게 전송하거나 수신합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>A, E</b>

<b>설명:</b> AWS Snowball은 대용량 데이터를 물리적으로 AWS에 옮기는 서비스입니다.

<b>A (정답):</b> AWS Snowball Edge 모델은 스토리지 기능 외에 내장 컴퓨팅 기능(EC2, Lambda)을 제공하여 데이터 전송 전 로컬 환경에서 데이터를 처리하거나 분석할 수 있습니다.

<b>E (정답):</b> Snowball의 가장 근본적인 목적은 대량의 데이터를 암호화하여 물리적으로 안전하게 AWS 데이터센터로 옮기는 것입니다.

<b>B (오답):</b> 타사 소프트웨어 카탈로그는 **AWS Marketplace**에 대한 설명입니다.

<b>C (오답):</b> 온프레미스와 클라우드 간의 하이브리드 스토리지는 **AWS Storage Gateway**에 더 가까운 설명입니다.

<b>D (오답):</b> 엑사바이트(Exabyte) 규모의 데이터 전송은 Snowball보다 훨씬 큰 트럭 크기의 **AWS Snowmobile** 서비스에 대한 설명입니다.

</details>

---

50. 한 회사가 AWS Enterprise Support 플랜을 사용하고 있습니다. 이 회사는 청구 및 계정 문의에 대해 빠르고 효율적인 지원을 원합니다. 다음 중 어떤 방법을 사용해야 할까요?

A. AWS 상태 대시보드

B. AWS 지원 컨시어지

C. AWS 고객 서비스

D. AWS 운영 지원

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<b>설명:</b> Enterprise Support 플랜의 핵심적인 혜택 중 하나를 묻는 문제입니다.

<b>B (정답):</b> AWS 컨시어지(Concierge) 팀은 **Enterprise Support 플랜 고객 전용**으로, 청구 및 계정 관련 문의를 전문적으로 처리해주는 전문가 팀입니다.

<b>A (오답):</b> AWS 상태 대시보드는 AWS 서비스의 전반적인 상태를 보여주는 곳이지, 개인의 계정 문의를 처리하는 곳이 아닙니다.

<b>C, D (오답):</b> '고객 서비스'나 '운영 지원'은 일반적인 용어이며, Enterprise 플랜에서 제공하는 이 특정 역할을 지칭하는 정확한 명칭은 '컨시어지'입니다.

</details>

---

51. 한 조직에 AWS 클라우드 인프라를 운영하는 많은 기술 직원이 있습니다. AWS는 이들을 팀으로 구성하고 각 팀에 적절한 권한을 할당하는 데 도움이 되는 어떤 서비스를 제공합니까?

A. IAM 역할

B. IAM 사용자

C. IAM 사용자 그룹

D. AWS 조직

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<b>설명:</b> 여러 사용자에게 동일한 권한을 효율적으로 부여하는 방법을 묻는 문제입니다.

<b>C (정답):</b> IAM 사용자 그룹(User Group)은 여러 IAM 사용자를 하나의 그룹으로 묶고, 그 그룹에 권한 정책을 적용하여 여러 사용자에게 한 번에 동일한 권한을 부여하는 기능입니다. '개발팀', '운영팀' 등으로 구성하는 것이 대표적인 예입니다.

<b>A (오답):</b> IAM 역할(Role)은 사용자나 서비스(예: EC2)가 특정 권한을 위임받아 사용하도록 하는 메커니즘이지, 사용자를 묶는 기능이 아닙니다.

<b>B (오답):</b> IAM 사용자(User)는 개별적인 자격 증명을 의미합니다.

<b>D (오답):</b> AWS 조직(Organizations)은 여러 AWS **계정(Account)**을 중앙에서 관리하는 서비스이지, 한 계정 내의 **사용자(User)**를 관리하는 주된 서비스가 아닙니다.

</details>

---

52. AWS에서 가장 중요한 모범 사례 중 하나는 클라우드 아키텍처의 탄력성 원칙입니다. 이 원칙은 아키텍처 설계를 어떻게 개선할 수 있을까요?

A. 수요 변화에 따라 온프레미스 리소스를 자동으로 확장합니다.

B. Elastic Load Balancer를 사용하여 AWS 리소스를 자동으로 확장합니다.

C. 가능한 한 애플리케이션 구성 요소 간의 상호 종속성을 줄입니다.

D. 수요 변화에 따라 필요한 AWS 리소스를 자동으로 프로비저닝합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<b>설명:</b> 탄력성(Elasticity)의 정확한 정의를 묻는 문제입니다.

<b>D (정답):</b> 탄력성이란, 트래픽이 몰리면 자동으로 서버(리소스)를 늘리고, 트래픽이 줄면 다시 자동으로 서버를 줄여서, 항상 필요한 만큼의 리소스만 사용하도록 하는 능력입니다.

<b>A (오답):</b> 탄력성은 AWS 클라우드 내의 리소스를 대상으로 하며, 온프레미스 리소스에는 적용되지 않습니다.

<b>B (오답):</b> 리소스를 자동으로 확장하는 서비스는 로드 밸런서가 아니라 **Auto Scaling**입니다. 로드 밸런서는 트래픽을 분산하는 역할을 합니다.

<b>C (오답):</b> 구성 요소 간의 종속성을 줄이는 것은 **'느슨한 결합(Loose Coupling)'**이라는 다른 중요한 아키텍처 설계 원칙입니다.

</details>

---

53. 설문조사 애플리케이션을 단 하룻 동안(중단 없이) 실행하려고 경우, 어떤 Amazon EC2 구매 옵션을 사용해야 할까요?

A. 예약된 인스턴스

B. 스팟 인스턴스

C. 전용 인스턴스

D. 주문형 인스턴스

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<b>설명:</b> 워크로드의 특성(기간, 중단 가능성)에 맞는 가장 적절한 구매 옵션을 선택하는 문제입니다.

<b>D (정답):</b> 주문형(On-Demand) 인스턴스는 약정 없이, 사용한 만큼만 비용을 지불하며, 언제든지 중단되지 않고 사용할 수 있어 예측 불가능한 단기 워크로드에 가장 적합합니다.

<b>A (오답):</b> 예약 인스턴스(Reserved Instance)는 1년 또는 3년의 장기 약정을 통해 할인을 받는 모델이므로, 단 하루 사용에는 부적합합니다.

<b>B (오답):</b> 스팟 인스턴스(Spot Instance)는 가장 저렴하지만, AWS가 필요할 때 언제든지 회수(중단)할 수 있으므로 '중단 없이' 실행해야 하는 요구사항을 충족하지 못합니다.

<b>C (오답):</b> 전용 인스턴스(Dedicated Instance)는 규정 준수 등 특별한 요구사항이 있을 때 단일 고객 전용 하드웨어에서 인스턴스를 실행하는 옵션으로, 비용 효율성과는 거리가 멉니다.

</details>

---

54. 다음 중 글로벌 콘텐츠 전송 네트워크(CDN) 서비스로 설명할 수 있는 것은 무엇입니까?

A. AWS VPN

B. 나, AWS 직접 연결

C. AWS 지역

D. 아마존 클라우드프론트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<b>설명:</b> 서비스의 정의를 직접적으로 묻는 문제입니다.

<b>D (정답):</b> 아마존 클라우드프론트(Amazon CloudFront)는 AWS의 CDN(Content Delivery Network) 서비스입니다. 전 세계에 퍼져있는 엣지 로케이션에 콘텐츠를 캐싱하여 최종 사용자에게 낮은 지연 시간으로 빠르게 전달합니다.

<b>A (오답):</b> AWS VPN은 온프레미스 네트워크와 AWS VPC를 안전하게 연결하는 서비스입니다.

<b>B (오답):</b> AWS 직접 연결(Direct Connect)은 인터넷 대신 전용 사설 회선을 통해 온프레미스와 AWS를 연결하는 서비스입니다.

<b>C (오답):</b> AWS 지역(Region)은 AWS 서비스가 호스팅되는 지리적 위치를 의미합니다.

</details>

---

55. 다음 중 AWS가 서비스 운영 및 유지 관리 부담을 책임지는 AWS 관리형 서비스의 예는 무엇입니까? (2개 선택)

A. 아마존 VPC

B. 아마존 다이나모DB

C. 아마존 엘라스틱캐시 멀티큐스

D. AWS IAM

E. 아마존 Elastic Compute Cloud

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B, C</b>

<b>설명:</b> '관리형 서비스'의 의미를 이해하고 있는지 묻는 문제입니다. 관리형 서비스란 인프라, OS 패치, 소프트웨어 설치 및 관리 등을 AWS가 대신해주는 서비스를 의미합니다.

<b>B (정답):</b> 아마존 다이나모DB(DynamoDB)는 서버 프로비저닝이나 관리가 전혀 필요 없는 완전 관리형(서버리스) NoSQL 데이터베이스입니다.

<b>C (정답):</b> 아마존 엘라스틱캐시(ElastiCache)는 AWS가 기본 서버와 캐싱 소프트웨어(Redis, Memcached)를 관리해주는 완전 관리형 인메모리 캐시 서비스입니다.

<b>A, D (오답):</b> VPC와 IAM은 고객이 직접 구성하고 관리해야 하는 네트워킹 및 자격 증명 서비스입니다.

<b>E (오답):</b> 아마존 EC2는 IaaS(Infrastructure as a Service)로, AWS는 하드웨어만 관리해주고 그 위의 운영체제(OS), 패치, 소프트웨어 관리는 **고객의 책임**입니다. 따라서 관리형 서비스가 아닙니다.

</details>

---

56. AWS Basic 지원을 이용 중인데, 일부 AWS 리소스가 악의적으로 사용되고 있으며 해당 리소스가 데이터를 손상시킬 수 있다는 사실을 발견했습니다. 어떻게 해야 할까요?

A. AWS 고객 서비스 팀에 문의하세요.

B. AWS 학대 신고팀에 문의하세요.

C. AWS 컨시어지 팀에 문의하세요.

D. AWS 보안팀에 문의하세요.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B</b>

<b>설명:</b> 특정 상황에 어떤 팀에 연락해야 하는지를 묻는 문제입니다.

<b>B (정답):</b> 스팸 발송, 악성코드 호스팅, 불법적인 활동 등 AWS 리소스의 악의적인 사용(Abuse) 사례를 발견했을 때는 **AWS 학대 신고팀(Abuse Team)**에 신고하는 것이 정해진 절차입니다. 이는 지원 플랜 등급과 관계없이 누구나 할 수 있습니다.

<b>A (오답):</b> 고객 서비스 팀은 주로 일반적인 질문이나 계정 관련 문의를 처리합니다.

<b>C (오답):</b> 컨시어지 팀은 Enterprise Support 고객 전용으로, 청구 및 계정 문의를 담당합니다.

<b>D (오답):</b> '보안팀'은 너무 광범위하며, 이런 유형의 문제를 처리하는 공식적인 창구는 '학대 신고팀'입니다.

</details>

---

57. AWS 공유 컨트롤의 두 가지 예를 선택하세요.

A. 패치 관리

B. IAM 관리

C. VPC 관리

D. 구성 관리

E. 데이터 센터 운영

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>A, D</b>

<b>설명:</b> '공유 컨트롤(Shared Controls)'은 공동 책임 모델에서 AWS와 고객 양쪽 모두에게 책임이 있는 영역을 의미합니다.

<b>A (정답): 패치 관리**는 대표적인 공유 컨트롤입니다. AWS는 인프라와 하이퍼바이저를 패치할 책임이 있고, 고객은 EC2 인스턴스 위의 게스트 OS와 애플리케이션을 패치할 책임이 있습니다.

<b>D (정답): 구성 관리** 역시 공유 컨트롤입니다. AWS는 자사 인프라의 구성을 책임지고, 고객은 자신의 리소스(VPC, 보안 그룹, 데이터베이스 등)를 올바르게 구성하고 관리할 책임이 있습니다.

<b>B, C (오답):</b> IAM과 VPC 관리는 거의 전적으로 고객의 책임 영역입니다.

<b>E (오답):</b> 데이터 센터의 물리적인 운영과 보안은 전적으로 AWS의 책임 영역입니다.

</details>

---

58. '단일 장애점'을 처리할 때 모범 사례를 구현하려면 감지 및 대응 모두에서 최대한 많은 자동화를 구축해야 합니다. 다음 AWS 서비스 중 어떤 것이 도움이 될까요? (두 가지 선택)

A. 앰비

B. 자동 크기 조정

C. 아마존 아테나

D. ECR

E. 아마존 EC2

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B, E</b>

<b>설명:</b> 단일 장애점(Single Point of Failure)을 없애기 위한 자동화된 아키텍처 구성을 묻고 있습니다.

<b>B (정답): 자동 크기 조정(Auto Scaling)**은 EC2 인스턴스의 상태를 모니터링하다가 특정 인스턴스에 장애가 발생하면 자동으로 종료하고 새로운 인스턴스를 시작하여 서비스를 복구합니다. 이는 단일 장애점을 제거하는 핵심적인 자동화 기능입니다.

<b>E (정답): 자동 크기 조정(Auto Scaling)**은 결국 아마존 EC2 인스턴스들을 대상으로 작동합니다. 따라서 단일 장애점을 없애는 고가용성 아키텍처는 여러 가용 영역에 분산된 EC2 인스턴스 그룹과 이를 관리하는 Auto Scaling의 조합으로 이루어집니다.

<b>A, C, D (오답):</b> Amplify(웹/모바일 개발), Athena(쿼리 서비스), ECR(컨테이너 레지스트리)은 인프라 장애 복구 자동화와 직접적인 관련이 없습니다.

</details>

---

59. 한 회사가 AWS에서 교육 웹 사이트를 호스팅하려고 합니다. 비디오 강좌는 전 세계에 스트리밍될 예정입니다. 다음 중 빠른 전송 속도를 달성하는 데 가장 도움이 되는 AWS 서비스는 무엇입니까?

A. 아마존 SNS

B. Amazon Kinesis 비디오 스트림

C. AWS 클라우드포메이션

D. 아마존 클라우드프론트

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<b>설명:</b> 전 세계 사용자에게 콘텐츠를 빠르게 전달하는 방법을 묻고 있습니다.

<b>D (정답): 아마존 클라우드프론트(Amazon CloudFront)**는 AWS의 CDN 서비스입니다. 원본 서버(예: S3)의 콘텐츠를 전 세계 사용자와 가까운 엣지 로케이션에 캐시해 두었다가 전달하므로, 비디오 같은 대용량 콘텐츠를 글로벌 사용자에게 낮은 지연 시간으로 빠르게 전송하는 데 가장 적합합니다.

<b>A (오답):</b> SNS는 푸시 알림 서비스입니다.

<b>B (오답):</b> Kinesis Video Streams는 비디오를 실시간으로 AWS에 **수집(Ingest)**하고 처리하는 서비스이지, 최종 사용자에게 **전달(Deliver)**하는 서비스가 아닙니다.

<b>C (오답):</b> CloudFormation은 인프라를 코드로 배포하는 자동화 도구입니다.

</details>

---

60. AWS Health Dashboard는 무엇을 제공합니까? (두 가지 선택)

A. 리소스에 영향을 미치는 AWS 이벤트에 대한 해결 지침

B. 자동 확장 인스턴스에 대한 상태 점검

C. 비용 최적화를 위한 권장 사항

D. 애플리케이션의 취약점을 자세히 설명하는 대시보드

E. AWS 서비스 상태에 대한 개인화된 보기

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>A, E</b>

<b>설명:</b> AWS Health Dashboard의 정확한 역할을 묻는 문제입니다.

<b>A (정답):</b> 특정 AWS 이벤트(예: 예정된 유지보수)가 내 리소스에 영향을 줄 경우, 해당 이벤트에 대한 설명과 **해결을 위한 지침**을 제공합니다.

<b>E (정답):</b> 모든 AWS 서비스의 일반적인 상태를 보여주는 '서비스 상태 대시보드'와 달리, AWS Health Dashboard는 **내 계정의 리소스에 영향을 미치는 이벤트**만 보여주는 **'개인화된 보기'**를 제공합니다.

<b>B (오답):</b> 인스턴스 상태 점검은 **Amazon CloudWatch**의 주요 기능입니다.

<b>C (오답):</b> 비용 최적화 권장 사항은 **AWS Trusted Advisor**의 주요 기능입니다.

<b>D (오답):</b> 애플리케이션 취약점 분석은 **Amazon Inspector**의 주요 기능입니다.

</details>

---

61. 여러 Amazon EC2 인스턴스에 애플리케이션을 배포했습니다. 고객들이 애플리케이션에 접속할 수 없다고 불평합니다. 이러한 문제를 해결을 위해 EC2 인스턴스 성능을 모니터링할 수 있는 AWS 서비스는 무엇인가요?

A. AWS 람다

B. AWS 구성

C. 아마존 클라우드워치

D. AWS 클라우드트레일

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>C</b>

<b>설명:</b> 리소스의 '성능'을 '모니터링'하는 서비스를 묻고 있습니다.

<b>C (정답): 아마존 클라우드워치(Amazon CloudWatch)**는 CPU 사용률, 네트워크 입출력, 디스크 I/O 등 AWS 리소스의 성능 지표(Metric)를 수집, 모니터링하고 로그를 분석하며 경보를 설정하는 AWS의 핵심 모니터링 서비스입니다.

<b>A (오답):</b> Lambda는 서버리스 컴퓨팅 서비스입니다.

<b>B (오답):</b> AWS Config는 리소스의 **구성 변경 이력**을 추적하는 서비스입니다.

<b>D (오답):</b> AWS CloudTrail은 계정 내의 **API 호출 이력(누가 무엇을 했는지)**을 기록하는 서비스입니다.

</details>

---

62. 귀사는 AWS에서 중요한 웹 애플리케이션을 개발하고 있으며, 애플리케이션 보안이 최우선 과제입니다. 다음 AWS 서비스 중 인프라 보안 최적화와 권장 사항을 제공하는 서비스는 무엇입니까?

A. AWS 쉴드

B. 관리 콘솔

C. AWS Secrets Manager

D. AWS 신뢰할 수 있는 자문가

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>D</b>

<b>설명:</b> AWS 모범 사례에 기반한 '최적화'와 '권장 사항'을 제공하는 서비스를 묻고 있습니다.

<b>D (정답): AWS 신뢰할 수 있는 자문가(Trusted Advisor)**는 고객의 AWS 환경을 자동으로 검사하여 비용 최적화, **보안**, 성능, 내결함성, 서비스 한도 등 5개 영역에 대한 모범 사례 권장 사항을 제공하는 서비스입니다.

<b>A (오답):</b> AWS Shield는 DDoS 공격을 방어하는 서비스입니다.

<b>B (오답):</b> 관리 콘솔은 AWS 리소스를 관리하는 웹 인터페이스입니다.

<b>C (오답):</b> Secrets Manager는 암호, API 키 등 보안 정보를 안전하게 저장하고 관리하는 서비스입니다.

</details>

---

63. 다음 중 Amazon S3의 이점이 아닌 것은 무엇입니까? (두 개 선택)

A. Amazon S3는 모든 유형의 데이터에 대해 무제한 저장 공간을 제공합니다.

B. Amazon S3는 모든 유형의 애플리케이션이나 백 엔드 시스템을 실행할 수 있습니다.

C. Amazon S3는 아무리 많은 객체라도 저장할 수 있지만, 객체 크기에는 제한이 있습니다.

D. Amazon S3는 수동으로 확장하여 어디서든 원하는 양의 데이터를 저장하고 검색할 수 있습니다.

E. Amazon S3는 99.999999999%(11 9s)의 데이터 내구성을 제공합니다.

<details markdown=1><summary markdown='span'>정답 및 설명</summary>

정답: <b>B, D</b>

<b>설명:</b> S3에 대한 설명 중 사실이 '아닌' 것을 고르는 문제입니다.

<b>B (정답 - 이점이 아님):</b> S3는 **스토리지** 서비스이지, **컴퓨팅** 서비스가 아닙니다. 애플리케이션이나 백엔드 시스템(코드)을 실행할 수는 없습니다. 코드는 EC2나 Lambda에서 실행해야 합니다.

<b>D (정답 - 이점이 아님):</b> S3는 사용자가 신경 쓸 필요 없이 **자동으로 확장**됩니다. 용량을 늘리기 위해 사용자가 '수동으로 확장'할 필요가 전혀 없습니다. 따라서 이 설명은 틀렸습니다.

<b>A, C, E (사실인 내용):</b> S3는 사실상 무제한의 저장 공간과 객체 수를 제공하며(단, 단일 객체 크기는 5TB로 제한), 11-nines의 내구성을 제공하는 것이 모두 맞는 설명이자 핵심 이점입니다.

</details>
