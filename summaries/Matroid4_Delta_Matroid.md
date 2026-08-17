# Matroid 4 — Delta Matroid

## Lecture Summary

delta matroid의 feasible set family와 symmetric exchange axiom을 정의하고, matching delta matroid와 signed greedy algorithm을 살펴봤다. 이어 twist와 mirror operation을 통해 delta matroid의 구조를 변환하는 방법과 skew-symmetric matrix, Pfaffian을 이용한 표현을 연결했다.

## Key Definitions

- **Delta Matroid**: feasible set family $\mathcal F\subseteq2^E$가 symmetric exchange axiom을 만족하는 구조.
- **Symmetric Exchange**: 두 feasible set의 차이에서 원소를 적절히 하나 또는 두 개 교환해 다시 feasible set을 얻는 성질.
- **Twist**: 집합 $S$에 대해 feasible set을 $F\triangle S$ 형태로 변환하는 연산.
- **Mirror**: deletion과 contraction을 포함하는 delta matroid의 기본 연산 관점.

## Main Ideas

- matroid는 basis의 크기가 일정하지만 delta matroid에서는 feasible set의 크기가 달라도 된다.
- matching delta matroid는 그래프의 perfect matching 구조와 연결된다.
- signed greedy algorithm은 가중치의 부호까지 고려해 feasible set을 선택한다.
- skew-symmetric matrix의 principal minor와 Pfaffian은 matching 및 delta matroid 표현과 연결된다.

## What I Understood

delta matroid는 matroid의 구조를 더 넓힌 개념으로, **feasible set의 크기가 달라도 exchange 구조를 유지할 수 있게 확장한 것**으로 이해했다. 특히 twist를 통해 서로 다른 feasible set 구조를 같은 관점에서 바라볼 수 있다는 점이 중요했다.

## Questions / Points to Review

- symmetric exchange axiom의 정확한 교환 조건.
- twist와 dual-like operation의 관계.
- Pfaffian과 perfect matching의 구체적인 계산 관계.

## Related Topics

- Matroid
- Delta Matroid
- Symmetric Exchange Property
- Matching
- Pfaffian

## Reference Note

The corresponding handwritten lecture note is [`Matroid5_Delta_Matroid.jpg`](../handwritten_notes/Matroid5_Delta_Matroid.jpg).
