# Matroid 2 — Linear Matroid

## Lecture Summary

matrix의 선형 독립 집합으로 정의되는 linear matroid를 소개하고, partition matroid, duality, minors, truncation, union 등의 기본 구조를 정리했다. simplex의 pivot rule과 함께 basis를 바꾸는 관점도 살펴봤다.

## Key Definitions

- **Linear Matroid**: 행렬 $A$의 열벡터들 가운데 선형 독립인 부분집합들을 independent set으로 가지는 matroid.
- **Partition Matroid**: 원소를 여러 그룹으로 나누고 각 그룹에서 선택할 수 있는 개수에 제한을 둔 matroid.
- **Minor**: deletion과 contraction으로 얻는 matroid.

## Main Ideas

- linear matroid는 선형대수의 독립성을 조합적 구조로 추상화한다.
- pivot rule은 simplex에서 다음 basis를 선택하는 규칙이며, shadow vertex rule은 이동 순서를 기하학적으로 정한다.
- dual matroid는 적절한 block matrix 표현을 통해 다시 linear matroid로 표현할 수 있다.
- deletion, contraction, truncation, union은 matroid의 구조를 변환하는 기본 연산이다.

## What I Understood

linear matroid는 행렬의 열벡터에 대한 선형 독립성을 matroid의 independent set으로 그대로 옮긴 구조다. 따라서 선형대수의 성질을 조합적 최적화의 언어로 다룰 수 있다는 점이 핵심이라고 이해했다.

## Questions / Points to Review

- linear matroid의 dual matrix 구성.
- deletion, contraction, truncation이 rank에 미치는 영향.
- simplex의 pivot rule과 matroid basis exchange의 관계.

## Related Topics

- Matroid
- Linear Matroid
- Simplex Method
- Matroid Duality
- Matroid Minors

## Reference Note

The corresponding handwritten lecture note is [`LP4_Pivot_rules_and_Matroid2_linear_Matroid.jpg`](../handwritten_notes/LP4_Pivot_rules_and_Matroid2_linear_Matroid.jpg).
