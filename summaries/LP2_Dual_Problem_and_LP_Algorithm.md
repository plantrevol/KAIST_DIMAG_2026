# LP2 — Dual Problem and LP Algorithm

## Lecture Summary

LP의 primal 문제에서 dual problem을 구성하고, weak duality와 strong duality를 통해 두 문제의 최적값 관계를 이해했다. 또한 Fourier–Motzkin elimination과 simplex, interior-point, ellipsoid 등의 LP 알고리즘을 비교하고, simplex의 기본 구조와 종료 조건을 살펴봤다.

## Key Definitions

- **Primal / Dual**: 하나의 LP에서 제약과 변수가 서로 대응하도록 만든 두 최적화 문제.
- **Weak Duality**: feasible primal의 목적함수값은 feasible dual의 목적함수값보다 클 수 없다(최대화 primal 기준).
- **Strong Duality**: primal과 dual이 모두 적절한 최적해를 가지면 최적 목적함수값이 같다.
- **Fourier–Motzkin Elimination**: 변수를 하나씩 제거해 projection을 구하는 방법.

## Main Ideas

- 표준형 primal

$$
\max\; c^Tx\quad\text{s.t. }Ax\le b,\ x\ge0
$$

에 대응하는 dual은

$$
\min\; b^Ty\quad\text{s.t. }A^Ty\ge c,\ y\ge0
$$

로 볼 수 있다.
- Weak duality는 dual feasible solution을 primal optimum의 상계로 사용하게 해준다.
- Strong duality에서는 두 optimum value가 일치한다.
- LP 알고리즘은 simplex처럼 vertex를 따라 이동하거나, interior-point처럼 feasible region 내부에서 접근하거나, 다른 기하학적 방법으로 해를 찾는다.

## What I Understood

Dual은 **최적값의 bound와 optimality certificate**를 제공한다는 점이 핵심이었다. 또한 simplex가 vertex 사이를 이동하는 알고리즘이라는 관점에서 이후의 edge direction과 reduced cost가 자연스럽게 연결된다.

## Questions / Points to Review

- 다양한 제약식 형태에서 dual을 만드는 규칙.
- strong duality의 정확한 가정과 증명.
- simplex와 다른 polynomial-time LP algorithm의 차이.

## Related Topics

- Linear Programming
- Primal–Dual Relationship
- Weak / Strong Duality
- Simplex Method

## Reference Note

The corresponding handwritten lecture note is [`LP2_Dual_Problem_and_LP_Algorithm.jpg`](../handwritten_notes/LP2_Dual_Problem_and_LP_Algorithm.jpg).
