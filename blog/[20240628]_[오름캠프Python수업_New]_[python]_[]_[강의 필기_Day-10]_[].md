# Day-10
1. 정적 메서드 (`@staticmethod`):
    - 정적 메서드는 기본적으로 클래스 내부에 정의된 일반 함수와 유사합니다.
    - 기본 메서드와의 주요 차이점은 다음과 같습니다:
        - 클래스나 인스턴스의 상태에 접근하거나 수정하지 않습니다.
        - 클래스나 인스턴스를 통해 호출할 수 있지만, 첫 번째 인자로 self나 cls를 받지 않습니다.
    - 주로 클래스와 관련은 있지만, 클래스나 인스턴스의 상태와는 독립적인 기능을 구현할 때 사용합니다.
2. 클래스 메서드 (`@classmethod`):
    - 개념 설명
        - `__init__`에 있는 속성뿐만 아니라, 클래스 레벨의 속성(클래스 변수)을 조작할 때 주로 사용됩니다.
        - 클래스 전체에 대한 동작을 정의하는 데 사용되는 것은 맞습니다.
    - 주요 특징:
        - 첫 번째 인자로 클래스 자체를 받습니다 (관례상 `cls`로 명명).
        - 인스턴스를 생성하지 않고도 클래스 레벨에서 호출할 수 있습니다.
        - 주로 대체 생성자를 만들거나 클래스 전체에 영향을 미치는 메서드를 정의할 때 사용합니다.