# [WIP]
# 문서화 원칙
문서는 협업의 기본이다.
개발한 내용을 공유할 때는 문서를 작성한다.
중요한 작업인 만큼 문서를 작성할 때는 원칙이 있어야한다.
[좋은 문서를 만드는 8가지 원칙](https://www.hanbit.co.kr/channel/category/category_view.html?cms_code=CMS6877759475)([원문](https://www.oreilly.com/content/the-eight-rules-of-good-documentation/) by [adam scott](https://www.oreilly.com/people/adam-scott/))을 바탕으로, 현재 개발팀에 어떻게 적용할 것인가를 고민했다.

문서를 효율적으로 공유하고 소통하는데 도움을 주는 프로세스를 만들기 위해 "8가지 원칙"을 개발팀에 맞게 5가지 원칙으로 재구성했다.
단, 아래 5가지 원칙은 팀 전체의 역량 증가와 효율성을 위한 것이기 때문에 팀원 전체의 합의가 필요하며, 개선할 여지가 있다.

1. 자유로운 접근
    - 문서는 기획, 개발, 아트 누구나 원할 때 언제든지 접근, 작성, 수정할 수 있어야 한다.
2. 찾기 쉽고 정돈된 문서
    - 최신 버전의 문서는 자신의 내용이 최신임을 스스로 보장해야 한다.
    - 접근한 문서는 항상 최신일 수 있도록 유도하고, 특별한 경우에만 구식 문서를 열람하는 환경을 제공해야 한다.
    - 문서는 찾기 쉬워야만 한다.
3. 문서-구현 일치
    - 구현된 것은 항상 문서와 일치해야 한다. 문서에 없다면 구현되지 말고, 구현되었다면 문서에 있어야한다.
    - 구현 과정이나 의사결정 과정에서 달라진 내용이 있다면 즉시 문서를 최신화해야 한다.
    - 문서가 "쓸모없어진" 상황은 문서가 "없는" 상황과 동일하며, 문서의 최신화가 가장 우선되어야 한다.
    - "쓸모없는 문서"가 공유되면 안된다.
4. 효율적인 문서 작성
    - 문서 작성에 많은 노동력을 투입하는 것은 지양한다.
    - 문서 작업과 구현은 항상 매끄럽게 연결되어야 한다.
5. 공동 책임
    - 공개된 문서는 그 문서를 작성했거나 담당하게 된 사람 뿐만 아니라 그 문서를 읽는 사람도 문서를 관리해야 한다.
    - 원칙에 어긋난 문서는 발견한 사람이 책임지고 수정하거나 인계해야 한다.

## 1. 자유로운 접근
- 문서는 기획, 개발, 아트 누구나 원할 때 언제든지 접근, 작성, 수정할 수 있어야 한다.

### [ 문제 인식 ]
팀원이 변경되거나, 개발 중 의사결정을 할 때 문서가 필요하다.
일반적으로 담당 인원에게 문서를 요청하거나, 문서 공유 플랫폼을 이용해 문서에 접근하게 된다.
하지만 가끔 열람 권한 문제로 문서를 볼 수 없다거나, 문서가 정돈되지 않아 담당자에게 직접 요청을 하는 경우가 많다.
일반적인 상황에서는 괜찮지만, 급한 상황이나 담당자가 오래 자리를 비우는 경우에는 큰 문제다.
심하면 누가 담당자인지 모르는 경우도 있다.
특히 비대면 근무를 하는 팀의 경우 자주 이런 문제가 발생한다.
팀원마다 연락 가능한 시간대가 다르거나 연락을 놓칠 수 있고, 한 공간에 함께 있는 것보다 소통이 어렵기 때문이다.

__문서의 자유로운 접근__ 이란 문서의 권한 문제 뿐만 아니라 문서가 있음에도 어디있는지 찾기 어려운 상황을 최대한 없애자는 원칙이다.
문제의 근본적인 원인은 __"내가 필요한 문서가 존재하는지, 어디에 있는지 모른다"__ 는 것이다.
이 문제를 해결하기 위해서는 팀원이 스스로 원하는 문서를 찾을 수 있도록 유도해야 하며, 동시에 문서의 존재 유무도 알 수 있어야한다.

## 2. 찾기 쉽고 정돈된 문서
- 최신 버전의 문서는 자신의 내용이 최신임을 스스로 보장해야 한다.
- 접근한 문서는 항상 최신일 수 있도록 유도하고, 특별한 경우에만 구식 문서를 열람하는 환경을 제공해야 한다.
- 문서는 찾기 쉬워야만 한다.

### [ 문제 인식 ]
문서를 공유받았는데 구버전인 경우가 있다.
업데이트하지 않았을 수 있고, 업데이트 했지만 관리가 되지않아 이전 버전을 공유받았거나, 버전이 다른 중복된 문서가 동시에 공유된 것일 수 있다.
이것은 매우 큰 문제다.
실제 구현이 의도와는 다르게 될 수 있기 때문이다.
따라서 문서는 버전이 관리되어야 하며, 구글 드라이브에 동일한 문서가 `문서_최종, 문서_최종최종, 문서_진짜최종`처럼 존재하는 상황은 피해야한다.
하나의 문서가 메신저와 이슈 탭에 동시에 공유되는 상황도 피해야한다.
가장 좋은 방법은 문서로 유도하는 과정에서 최신 문서만을 확인할 수 있도록 만드는 것과, 이미 공유된 문서를 다시 공유할 때는 문서의 링크가 아닌 문서가 공유된 장소의 링크를 공유하는 것이다.

## 3. 문서-구현 일치
- 구현된 것은 항상 문서와 일치해야 한다. 문서에 없다면 구현되지 말고, 구현되었다면 문서에 있어야한다.
- 구현 과정이나 의사결정 과정에서 달라진 내용이 있다면 즉시 문서를 최신화해야 한다.
- 문서가 "쓸모없어진" 상황은 문서가 "없는" 상황과 동일하며, 문서의 최신화가 가장 우선되어야 한다.

### [ 문제 인식 ]
마감 시간이 다가오면 귀찮은 문서작업보다는 빠른 구현에 초점을 맞춘다.
변경점이 문서에 적용되는 시간보다 구현이 빠르게 진행되며 문서는 기능을 하지 못한다.
빠른 구현보다 문서 작성에 초점을 맞춰야 한다고 오해할 수 있지만, 핵심은 문서에 실시간으로 변경사항이 적용되지 못하는 환경을 개선해야 한다는 것이다.
해결책으로는 기획 문서는 변경이 적은 큰 틀만 간단히 작성하고, 작은 디테일은 회의록 등 간단하게만 정리하면 문서 작성에 노력도 감소한다.
이것은 `4. 효율적인 문서 작성` 원칙과 연결되는 내용이다.
주의할 점은 변경사항이 발생하면 반드시 `"A"에서 "B"로 변경됨` 처럼 변경사항의 히스토리를 파악할 수 있게 작성해야 한다는 것이다.

## 4. 효율적인 문서 작성
- 문서 작성에 많은 노동력을 투입하는 것은 지양한다.
- 문서 작업과 구현은 항상 매끄럽게 연결되어야 한다.

### [ 문제 인식 ]
문서화는 개발의 효율을 높이기 위해서 하는 행동임을 잊으면 안된다.
문서를 작성하는 시간이 개발하는 시간을 침해하면 안된다.
개발자의 문서화

## 5. 공동 책임
- 공개된 문서는 그 문서를 작성했거나 담당하게 된 사람 뿐만 아니라 그 문서를 읽는 사람도 문서를 관리해야 한다.
- 원칙에 어긋난 문서는 발견한 사람이 책임지고 수정하거나 인계해야 한다.

### [ 문제 인식 ]
'누군가 바꿔주겠지'라는 안일한 생각을 가지고 있다가 정작 문서가 필요해졌을 때도 업데이트가 안된 상황이 생길 수 있다.
문서에 접근하는 모든 사람들은 반드시 그 문서를 책임지고 최신 내용을 반영하도록 업데이트해야만 한다.

# 결론
프로젝트를 진행하면 경험적으로 문서화의 어려움을 느끼게 된다. 문서화의 어려움과 함정을 피하기 위해 세운 원칙을 다른 사람과 공유하기 위해 글을 작성했다.
위 원칙을 프로세스에 적용해 생기는 문제점은 아직 파악하지 않았기 때문에 아직 실험이 필요하다는 한계가 있으며, 지속적으로 업데이트 예정이다.