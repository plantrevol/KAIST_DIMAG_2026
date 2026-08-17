# Matroid 1 — Greedy and Duality

## Lecture Summary

matroid의 독립 집합 공리를 바탕으로 uniform, partition, vector, graphic matroid의 예를 확인했다. 이어 basis의 exchange property를 이용한 greedy algorithm의 최적성과 dual matroid, deletion, contraction의 관계를 정리했다.

## Key Definitions

- **Matroid**: 독립 집합 family가 hereditary property와 augmentation property를 만족하는 구조.
- **Basis**: maximal independent set.
- **Circuit**: 최소 dependent set.
- **Dual Matroid**: 원래 matroid의 basis의 여집합을 basis로 갖는 matroid.

## Main Ideas

- 모든 basis는 같은 크기를 가지며 이를 rank라 한다.
- basis exchange property가 성립하기 때문에 greedy가 maximum-weight basis를 찾을 수 있다.
- deletion과 contraction은 matroid의 minor를 만드는 기본 연산이다.
- dual과 관련하여 deletion과 contraction이 서로 대응된다.

## What I Understood

matroid는 여러 조합적 문제의 **독립성 조건을 하나의 추상 구조로 묶은 것**이라고 이해했다. 특히 greedy의 최적성이 특정 문제의 성질이 아니라 matroid의 exchange 구조에서 나온다는 점이 핵심이었다.

## Questions / Points to Review

- basis exchange property의 정확한 증명.
- greedy algorithm의 교환 논증.
- dual에서 deletion과 contraction이 대응하는 이유.

## Related Topics

- Matroid
- Greedy Algorithm
- Dual Matroid
- Matroid Minors

## Reference Note

The corresponding handwritten lecture note is [`Matroid1_greedy_and_duality.jpg`](../handwritten_notes/Matroid1_greedy_and_duality.jpg).
