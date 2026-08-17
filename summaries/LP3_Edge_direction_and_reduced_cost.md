# LP3 — Edge Direction and Reduced Cost

## Lecture Summary

Standard form의 LP에서 basic feasible solution(BFS)을 기준으로 인접 vertex로 이동하는 edge direction을 구하고, 그 방향으로 이동했을 때 목적함수가 얼마나 변하는지를 reduced cost로 표현했다. 이를 이용해 simplex의 한 iteration을 구체적으로 정리했다.

## Key Definitions

- **BFS**: basis $B$에 대해 non-basic variable을 0으로 두고 $x_B=A_B^{-1}b\ge0$를 만족하는 feasible solution.
- **Edge Direction**: 한 vertex에서 인접한 vertex로 이동하기 위한 feasible direction.
- **Reduced Cost**: 현재 basis에서 특정 non-basic variable을 증가시킬 때 목적함수가 변하는 정도.

## Main Ideas

- basis $B$와 entering index $j$가 주어지면
$$
w_j=-1,\qquad w_B=A_B^{-1}A_j
$$
같은 형태로 edge direction을 구한다.
- reduced cost를 통해 해당 방향으로 이동했을 때 objective가 개선되는지 판단한다.
- 최대화 문제에서 모든 reduced cost가 적절한 부호를 가지면 현재 BFS가 optimal이다.
- 방향이 feasible한 범위가 무한하면 LP는 unbounded일 수 있다.

## What I Understood

Simplex의 한 단계가 단순히 vertex를 옮기는 것이 아니라 **basis 변경 → edge direction 계산 → reduced cost로 개선 여부 판단 → step size 결정**의 과정이라는 것을 이해했다. 특히 reduced cost가 최적성 판단과 직접 연결된다.

## Questions / Points to Review

- reduced cost 부호 convention의 차이.
- ratio test와 leaving variable의 정확한 유도.
- degenerate BFS에서 step size가 0이 되는 경우.

## Related Topics

- Linear Programming
- Simplex Method
- Basic Feasible Solution
- Pivot

## Reference Note

The corresponding handwritten lecture note is [`LP3_Edge_direction_and_reduced_cost.jpg`](../handwritten_notes/LP3_Edge_direction_and_reduced_cost.jpg).
