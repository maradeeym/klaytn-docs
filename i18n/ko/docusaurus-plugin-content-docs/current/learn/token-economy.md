# 토큰 이코노미

## 개요 <a id="overview"></a>

클레이튼의 토큰 이코노미는 생태계, 성장 이니셔티브, 전략적 투자를 강화하기 위한 지속 가능한 자금 구조를 만들기 위해 설계되었습니다. 많은 퍼블릭 블록체인 프로젝트는 노드 운영자(채굴자 또는 블록 생성자)에게만 인센티브를 제공하는 화폐 시스템을 가지고 있으며, 네트워크 유지보수라는 기술적 측면에만 초점을 맞추고 있습니다. 그러나 이러한 설계는 네트워크 토큰 이코노미의 성장에 기여하거나 장기적인 성장 전망에 투자하는 다른 유형의 참여자들에게 인센티브를 제공하는 것의 중요성을 놓치고 있습니다. 이와는 대조적으로 클레이튼의 토큰 이코노미는 보다 다양한 형태의 참여자들이 기여한 것에 대해 보상하도록 설계되었으며, 블록체인 노드를 유지하는 것 외에도 미래 성장 이니셔티브와 전략적 투자 프로젝트에 필요한 지속적인 자원을 조달할 수 있는 자금 조달 구조가 내장되어 있습니다.

## 펀딩 구조 <a id="funding-structure"></a>

클레이튼의 자금 구조는 클레이튼 네트워크의 블록 생성과 함께 지속적으로 운영됩니다. 새로운 블록이 생성될 때마다 새로 발행된 KLAY와 해당 블록에서 사용된 트랜잭션 수수료의 합계(통칭하여 "블록 보상"이라 함)가 합산되어 미리 정해진 비율에 따라 다음 세 개의 대상 계좌에 분배됩니다:

* 클레이튼 거버넌스 카운슬(GC) 보상:
    * GC 블록 제안자 보상: 10%
    * GC 스테이킹 보상: 40%
* 클레이튼 커뮤니티 펀드 \(KCF\): 30%
* 클레이튼 재단 기금 \(KFF\): 20%

새로운 블록이 생성될 때마다 6.4 KLAY가 발행됩니다. 이는 연간 약 2억 KLAY가 발행된다는 것을 의미하며, 이는 제네시스에서 발행된 100억 KLAY 대비 연간 2%의 인플레이션에 해당합니다(연간 인플레이션율은 Klaytn 거버넌스 프로세스를 통해 변경될 수 있습니다). 트랜잭션 수수료는 OPCODE당 부과되며, 트랜잭션 수수료 표에 따라 계산됩니다. 트랜잭션 수수료 표에 대한 자세한 내용은 [트랜잭션 수수료](./transaction-fees.md)를 참고하시기 바랍니다.

## 클레이튼 거버넌스 카운슬 보상 <a id="klaytn-governance-council-reward"></a>

클레이튼 거버넌스 카운슬은 코어 셀 운영자 \(CCO\)들의 집합체입니다. 카운슬 멤버는 코어 셀 \(CC\)을 유지 관리할 책임이 있으며, 따라서 카운슬은 클레이튼 생태계에서 기본 인프라 제공을 책임지는 필수적인 기구입니다. 카운슬 멤버가 되려면 클레이튼 거버넌스 프로세스에 따라 자격 심사를 거쳐야 하며, 최소 5백만 KLAY를 스테이킹해야 합니다. 클레이튼 거버넌스 카운슬 보상은 카운슬 멤버들이 클레이튼 생태계의 안정적인 기반을 지속적으로 제공할 수 있도록 인센티브를 제공하는 구조입니다.

### 클레이튼 거버넌스 카운슬 보상 메커니즘 <a id="klaytn-governance-council-reward-mechanism"></a>

모든 블록마다 무작위로 선정된 카운슬 멤버로 구성된 위원회가 구성됩니다. 각 위원회에는 제안자 역할을 맡은 한 명의 위원이 있으며, 다른 모든 위원회 위원은 검증자 역할을 맡습니다. 블록이 성공적으로 생성되어 클레이튼 블록체인에 추가되면 해당 블록의 제안자는 블록 보상의 100%를 보상받게 됩니다. 카운슬 멤버가 제안자로 선정될 확률은 해당 멤버가 스테이킹한 KLAY의 양에 비례합니다. 즉, 멤버가 더 많은 KLAY를 스테이킹할수록 제안자로 선정되어 블록 보상을 받을 가능성이 높아집니다.

최소 5백만 KLAY 스테이킹 요건을 충족하는 한, Klaytn 거버넌스 카운슬 멤버는 자신의 KLAY를 자유롭게 스테이킹하거나 스테이킹을 해제할 수 있습니다. 스테이킹 정보는 86,400 블록마다 업데이트되며, 새로 스테이킹된 KLAY는 스테이킹이 완료된 시점으로부터 두 번의 업데이트 주기 후에 정보가 적용됩니다. 악의적인 회원의 즉각적인 탈퇴를 방지하기 위해 스테이킹된 KLAY를 철회하려면 1주일의 지연 시간이 필요합니다.

많이 투자한 소수의 카운슬 멤버들이 클레이튼 거버넌스 카운슬 보상을 독점적으로 청구하는 것을 방지하기 위해, Gini 계수를 사용하여 스테이킹된 KLAY의 유효량을 조정할 수 있습니다. 적용 공식은 다음과 같으며, 여기서 G는 거버넌스 카운슬의 KLAY 스테이킹 분포의 Gini 계수를 나타냅니다:

* _조정된 스테이킹 금액 = \(카운슬 멤버의 스테이킹 금액\)^\(1/1+G\)_


### 잘못된 행동을 한 카운슬 멤버에 대한 페널티 <a id="penalty-for-misbehaving-council-members"></a>

카운슬 멤버는 아래에 정의된 잘못된 행동을 할 경우 페널티를 받을 수 있습니다. 향후 클레이튼 거버넌스 프로세스를 통해 더 많은 페널티 규정이 수립되고 개선될 수 있습니다.

Safety Failure 야기:

* 제안자로 선정된 카운슬 멤버는 동일한 높이의 블록을 두 개 이상 생성할 수 없습니다.
* 제안자로 선정된 카운슬 멤버는 특정 거래를 의도적으로 생략할 수 없습니다.

Liveness Failure 야기:

* 제안자로 선정된 카운슬 멤버는 유효한 블록을 생성해야 합니다.
* 검증자로 선정된 카운슬 멤버는 제안자가 제안한 블록의 유효성을 검사해야 합니다.

## 클레이튼 커뮤니티 펀드 <a id="klaytn-community-fund"></a>
클레이튼 커뮤니티 기금(KCF)은 더 높은 투명성과 검증 가능성을 실현하고자 하는 클레이튼의 미션을 지원하기 위해 설립되었습니다. 기존 클레이튼 성장 기금(KGF)과 클레이튼 개선 준비금(KIR)이 합쳐져 새로운 클레이튼 커뮤니티 기금(KCF)이 되었다는 점을 기억해두시기 바랍니다.

클레이튼 커뮤니티 펀드는 다음과 같이 클레이튼 생태계를 개선하는 활동에 자금을 지원하는 데 사용됩니다:

1. **기여 증명(Proof of Contribution)에 대한 보상**: 이미 개발된 서비스 중 클레이튼 생태계에 기여도가 높은 프로젝트에 대해 가스비 지원 등 후속 지원을 제공합니다.
2. **개발자 커뮤니티 구축**: 재단은 클레이튼 개발자 커뮤니티를 육성하고 성장시키기 위해 해커톤, 개발 교육 프로그램, 업계와의 공동 연구, 다양한 DAO와의 협업 등 다양한 이니셔티브를 지원할 예정입니다.
3. **생태계 서비스 및 인프라 육성**: KCF는 명확한 효용성을 가진 서비스 개발과 마케팅 지원과 함께 필수적인 생태계 인프라를 지원할 것입니다.
4. **클레이튼 에코 펀드 간접 투자**: KCF는 크립토 전문 VC에 위탁하여 중장기 간접 투자를 진행하며, 추후 투자금 회수 시 발생하는 수익의 대부분을 클레이튼 생태계에 환원할 예정입니다.

클레이튼 커뮤니티 기금의 운영은 GC가 [클레이튼 스퀘어](https://square.klaytn.foundation/Home)의 공개 포럼에서 기금 사용을 검토하고 승인하는 절차를 따릅니다. 재단은 각 카테고리에 대한 예산 제안서를 GC에 제출하여 승인을 받습니다. 승인된 예산 범위 내에서 구체적인 사용처에 대한 검토와 GC의 재승인이 이루어집니다. 한편, KCF는 현재 [파일럿 프로그램](https://klaytn.foundation/kcf-grant-pilot/)으로 운영되고 있으며, 관심 있는 분들은 [클레이튼 거버넌스 포럼](https://govforum.klaytn.foundation/t/operational-procedures-of-the-kcf-grant-program-pilot/288)에서 프로그램에 대한 자세한 내용을 확인할 수 있습니다.

## 클레이튼 재단 펀드 <a id="klaytn-foundation-fund"></a>

클레이튼 재단 기금(KFF)은 이 두 가지 카테고리에 집중할 운영 기금입니다:

1. **생태계 지원**: 여기에는 소정의 재정 지원, 신규 GC 멤버 확보, 유동성 공급, 재단 주도의 서비스 개발/펀딩 등이 포함됩니다.
2. **재단 운영**: 개발, 회계, 인프라 운영, 마케팅, 인건비 등의 운영 비용과 재무 관리 및 투자유치 비용이 포함됩니다.

KFF는 KCF와 마찬가지로 온체인 투표를 통해 GC의 승인을 받은 후 자율적이고 투명하게 집행될 예정입니다.

자세한 내용은 이 [기사](https://medium.com/klaytn/klaytn-tokenomics-optimization-governance-proposal-securing-a-sustainable-verifiable-token-1efd2a49b04e)를 참조하세요.
