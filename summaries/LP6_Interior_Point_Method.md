# LP6 — Interior Point Method

## Lecture Summary

feasible region의 내부를 따라 최적해로 접근하는 interior-point method를 정리했다. central path와 barrier function을 이용해 inequality constraint를 다루고, primal-dual central path와 predictor-corrector 방식으로 실제 반복 알고리즘을 구성했다.

## Key Definitions

- **Barrier Function**: 경계에 가까워질수록 비용이 커지도록 하여 feasible region 내부에 머물게 하는 함수.
- **Central Path**: barrier parameter에 따라 barrier problem의 최적해가 이동하는 경로.
- **Primal-Dual Central Path**: primal과 dual의 feasibility 및 complementarity를 함께 만족하도록 정의한 경로.
- **Predictor-Corrector**: 먼저 현재 경로에서 벗어나는 방향을 예측하고, 이후 correction step으로 다시 central path 근처로 보정하는 방법.

## Main Ideas

- 로그 barrier를 넣어 $\min c^Tx-\mu\sum_i\log x_i$
- 형태의 smooth problem으로 바꿀 수 있다.
- $\mu$를 점차 줄이면 barrier problem의 해가 원래 LP의 최적해에 가까워진다.
- predictor step과 corrector step을 반복해 primal-dual central path를 따라간다.
- homogeneous self-dual embedding은 초기 feasible point를 구성하고 infeasible 상황까지 함께 다루는 방법이다.

## What I Understood

simplex가 polyhedron의 **경계(vertex)**를 따라 이동한다면 interior-point method는 **내부의 central path**를 따라 최적해에 접근한다. barrier가 경계에서 발산하기 때문에 feasible region 내부를 유지하면서 최적점으로 수렴한다는 점이 핵심이었다.

## Questions / Points to Review

- central path의 정확한 정의와 수렴 과정.
- Newton system에서 predictor/corrector 식의 유도.
- homogeneous self-dual embedding의 feasibility 판정.

## Related Topics

- Linear Programming
- Barrier Method
- Primal-Dual Method
- Newton Method

## Reference Note

The corresponding handwritten lecture note is [`LP6_Interior_Point_Method.jpg`](../handwritten_notes/LP6_Interior_Point_Method.jpg).
