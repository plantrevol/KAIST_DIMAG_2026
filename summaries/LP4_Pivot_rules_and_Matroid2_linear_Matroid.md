# LP4 — Pivot Rules and Matroid 2: Linear Matroid

## Lecture Summary

simplex에서 pivot을 어떤 기준으로 선택할지 살펴보고, shadow vertex rule을 통해 cycle을 피하면서 이동하는 방법을 정리했다. 이어 matrix의 선형 독립 집합으로 정의되는 linear matroid를 소개하고 partition matroid, duality, minors, truncation, union 등의 기본 구조를 다뤘다.

## Key Definitions

- **Pivot Rule**: 다음 basis를 선택하는 규칙. 속도와 cycle 회피가 중요하다.
- **Shadow Vertex Rule**: 목적함수와 보조 방향을 이용해 vertex의 이동 순서를 정하는 방법.
- **Linear Matroid**: 행렬 $A$의 열벡터들 가운데 선형 독립인 부분집합들을 independent set으로 가지는 matroid.
- **Minor**: deletion과 contraction으로 얻는 matroid.

## Main Ideas

- pivot rule은 simplex의 실제 수행 횟수와 cycle 발생 가능성에 영향을 준다.
- linear matroid는 행렬의 열 독립성을 추상화한 구조다.
- partition matroid와 같은 기본 예를 통해 matroid가 다양한 제한 조건을 표현할 수 있다.
- dual matroid는 적절한 block matrix 표현을 통해 linear matroid의 형태로 다시 표현할 수 있다.

## What I Understood

Simplex의 pivot 선택 문제와 matroid의 basis/exchange 구조가 모두 **basis를 바꾸면서 좋은 해를 찾아가는 과정**이라는 점에서 연결된다는 느낌을 받았다. Linear matroid는 선형대수에서의 독립성을 조합적 구조로 옮긴 것이라고 이해했다.

## Questions / Points to Review

- shadow vertex rule의 정확한 기하학적 의미.
- linear matroid의 dual matrix 구성.
- deletion, contraction, truncation이 rank에 미치는 영향.

## Related Topics

- Simplex Method
- Pivot Rules
- Matroid
- Linear Matroid
- Matroid Duality

## Reference Note

The corresponding handwritten lecture note is [`LP4_Pivot_rules_and_Matroid2_linear_Matroid.jpg`](../handwritten_notes/LP4_Pivot_rules_and_Matroid2_linear_Matroid.jpg).
