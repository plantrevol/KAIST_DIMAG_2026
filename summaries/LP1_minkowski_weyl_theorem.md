# LP1 — Minkowski–Weyl 정리

## Lecture Summary

볼록함수의 최적해가 꼭짓점에서 얻어진다는 사실에서 출발해, polyhedron의 face와 recession cone을 정의하고 Minkowski–Weyl 정리를 통해 polyhedron을 꼭짓점과 extreme ray의 convex/conic combination으로 표현했다. 이어 Carathéodory 정리를 이용해 필요한 생성자의 수를 줄일 수 있음을 확인했다.

## Key Definitions

- **Face**: polyhedron의 특정 선형 제약이 등호로 tight해지는 부분집합.
- **Vertex**: 0차원 face.
- **Recession Cone**: $P$에서 임의의 점을 일정 방향으로 계속 이동해도 $P$를 벗어나지 않는 방향들의 집합.
- **Extreme Ray**: recession cone의 극단적인 방향.

## Main Theorem

**Minkowski–Weyl 정리**: polyhedron $P$는 꼭짓점의 convex combination과 recession cone의 extreme ray의 conic combination으로 표현할 수 있다.

$$
P=\mathrm{conv}(V(P))+\mathrm{cone}(R(P)).
$$

bounded polyhedron에서는 recession cone이 사라져 $P=\mathrm{conv}(V(P))$가 된다.

## Key Ideas

- polyhedron의 모든 face는 적절한 제약식들의 intersection으로 표현할 수 있다.
- $\dim F=n-\mathrm{rank}(A_I)$ 관계를 통해 face의 차원과 active constraint의 rank가 연결된다.
- Carathéodory 정리에 따라 한 점의 표현에 필요한 생성자 수를 차원에 맞게 제한할 수 있다.

## What I Understood

LP의 최적해가 왜 vertex를 중심으로 설명되는지 이해할 수 있었다. Minkowski–Weyl 정리는 단순히 도형을 표현하는 정리가 아니라, LP feasible region의 구조를 **vertex + ray**로 분해해 이후 simplex와 연결해 주는 핵심 결과라고 이해했다.

## Questions / Points to Review

- Minkowski–Weyl 정리의 내·외부 표현 사이의 정확한 증명.
- Carathéodory 정리의 생성자 제거 과정.
- recession cone과 unbounded LP의 관계.

## Related Topics

- Linear Programming
- Convexity
- Extreme Points
- Simplex Method

## Reference Note

The corresponding handwritten lecture note is [`LP1_minkowski_weyl_theorem.jpg`](../handwritten_notes/LP1_minkowski_weyl_theorem.jpg).
