# Matroid 5 — Matroid Intersection Problem and Matroid Parity Problem

## Lecture Summary

두 matroid의 independent set에 동시에 속하는 최대 집합을 찾는 matroid intersection problem과, 원소를 쌍으로 묶어 문제를 구성하는 matroid parity problem을 살펴봤다. 두 문제 모두 matroid 구조를 이용해 조합적 최적화를 수행하지만, parity problem은 추가적인 쌍 구조 때문에 더 어렵다는 점을 확인했다.

## Key Definitions

- **Matroid Intersection**: 두 matroid $M_1,M_2$에서 동시에 independent인 최대 크기의 집합을 찾는 문제.
- **Common Basis**: 두 matroid의 basis이면서 동시에 공통인 집합.
- **Matroid Parity**: 원소를 미리 pair로 묶고, 선택한 pair들의 원소 집합이 matroid-independent가 되도록 최대한 많은 pair를 선택하는 문제.

## Main Ideas

- 두 matroid에 공통 basis가 존재하는지 확인하는 문제를 matroid intersection으로 볼 수 있다.
- 강한 교환 구조를 이용해 공통 independent set을 증가시키는 방식으로 알고리즘을 생각할 수 있다.
- matroid parity는 pair 단위의 선택을 요구하므로 일반 matroid intersection보다 추가적인 구조와 제약이 생긴다.
- 특수한 matroid에서는 parity problem을 다른 조합적 문제로 변환해 볼 수 있다.

## What I Understood

matroid가 하나일 때는 greedy가 강력하지만, **두 matroid의 제약을 동시에 만족시키면 단순 greedy만으로 해결되지 않는다**는 점이 중요했다. matroid intersection은 exchange 구조를 활용해 이를 해결하고, parity는 pair라는 추가 조건 때문에 한 단계 더 복잡해진다고 이해했다.

## Questions / Points to Review

- matroid intersection augmenting path의 정확한 구성.
- common basis와 maximum common independent set의 관계.
- matroid parity가 NP-hard인 일반적인 경우와 tractable한 특수 경우.

## Related Topics

- Matroid Intersection
- Matroid Parity
- Augmenting Path
- Combinatorial Optimization

## Reference Note

The corresponding handwritten lecture note is [`Matroid4_MatroidIntersectionProblem_and_MatroidParityProblem.jpg`](../handwritten_notes/Matroid4_MatroidIntersectionProblem_and_MatroidParityProblem.jpg).
