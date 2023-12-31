
# 1과목 데이터 모델링의 이해
## 1장 데이터 모델링의 이해
### 1. 데이터 모델의 이해
#### (1) 모델링: 현실세계를 단순화하여 표현하는 것
* 특징
  +	추상화: 일정한 형식에 맞춰 표현함
  +	단순화: 제한된 표기법이나 언어로 표현함
  +	명확성: 이해가 쉽게 표현함
* 관점
  +	데이터 관점: 업무와 데이터 및 데이터 사이의 관계
  +	프로세스 관점: 진행되고 있거나 진행되어야 하는 업무
  + 상관 관점: 데이터에 대한 업무 처리 방식의 영향
#### (2) 데이터 모델링: 정보 시스템 구축을 위한 데이터 관점의 업무 분석 기법
* 목적: (가) 정보에 대한 표기법을 통일하여 업무 내용 분석 정확도 증대 (나) 데이터 모델을 기초로 DB 생성
* 기능: (가) 가시화 (나) 명세화 (다) 구조화된 틀 제공 (라) 문서화 (마) 다양한 관점 제공 (바) 구체화
* 중요성
  + 파급효과(Leverage): 데이터 구조 변경으로 인한 일련의 변경작업 위험요소 해결
  +	간결한 표현(Conciseness): 요구사항, 한계 명확하고 간결하게
  +	데이터 품질(Data Quality): 오래된 데이터의 정확성, 신뢰성 해결
* 유의점
  + 중복 (Duplication) : 데이터베이스가 여러 장소에 같은 정보 저장하는 것 주의
  + 비유연성 (Inflexibility) : 사소한 업무변화에 데이터모델 수시로 변경되면 유지보수 어려움
    - 데이터의 정의를 데이터의 사용 프로세스와 분리하여 해결
  + 비일관성 (Inconsistency) : 데이터의 중복이 없어도 비일관성 발생 가능
    - 모델링 할 때 데이터간 상호 연관관계 명확히 정의하여 해결
*	이해관계자: (가) 개발자 (나) DBA (다) 모델러 (라) 현업업무전문가 들 모두가 완성된 모델을 정확히 해석할 수 있어야 함
#### (3) 데이터 모델링 3단계
1. 개념적 모델링: 엔터티와 속성을 도출하고 ERD를 작성함, 업무 중심적이고 포괄적인 수준의 모델링
2. 논리적 모델링: 식별자를 도출하고 속성과 관계 등을 정의함, 정규화를 수행하여 데이터 모델의 독립성과 재사용성 확보, 논리 데이터 모델은 데이터 모델링 완료 상태
3. 물리적 모델링: DB를 구축함, 성능 및 보안 등 물리적인 성격 고려

※ 프로젝트 생명주기(Life Cycle): 계획 > 분석 > 설계 > 개발 > 테스트 > 전환/이행 단계로 구성됨. (가) 계획과 분석 단계는 개념적 모델링 (나) 분석 단계는 논리적 모델링 (다) 설계 단계는 물리적 모델링에 해당
