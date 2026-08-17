# LP5 — Smoothed Analysis of the SSP Algorithm

## Lecture Summary

local step에서 tangent cone을 이용해 simplex의 이동 방향을 해석하고, 이를 shortest s-t path(SSP) 문제와 연결했다. residual network과 successive shortest path algorithm을 정리하고, 작은 perturbation을 가정하는 smoothed analysis를 통해 worst-case와 실제 성능 사이의 차이를 살펴봤다.

## Key Definitions

- **Tangent Cone**: 한 점에서 feasible set 내부로 이동 가능한 국소적 방향들의 집합.
- **Residual Network**: 현재 flow에서 추가로 보낼 수 있는 방향과 기존 flow를 되돌릴 수 있는 방향을 나타낸 네트워크.
- **SSP Algorithm**: residual network에서 반복적으로 shortest s-t path를 선택해 flow를 증가시키는 알고리즘.
- **Smoothed Analysis**: 입력에 작은 무작위 perturbation을 가한 뒤 평균적인 실행시간을 분석하는 방법.

## Main Ideas

- tangent cone을 이용하면 simplex의 local step을 국소적인 최적화 문제로 표현할 수 있다.
- min-cost flow는
$$
\min c^Tf\quad\text{s.t. }Af=b,\ 0\le f\le u
$$
형태의 LP로 표현할 수 있다.
- SSP는 residual network에서 가장 싼 s-t path를 반복적으로 선택한다.
- 입력 비용을 조금 perturb하면 최단 경로 비용 사이의 우연한 근접성이 완화되어 simplex/SSP의 실제 평균적 성능을 설명할 수 있다.

## What I Understood

shortest path와 LP가 별개의 문제가 아니라 **simplex의 local pivot과 SSP의 augmenting path가 비슷한 구조**를 가진다는 점이 흥미로웠다. Worst-case만 보면 알고리즘이 비현실적으로 느릴 수 있지만, smoothed analysis는 작은 입력 변화까지 고려해 실제 성능을 설명하려는 관점이라는 것도 이해했다.

## Questions / Points to Review

- tangent cone program과 simplex edge direction의 정확한 대응.
- residual network에서 negative-cost reverse edge가 생기는 이유.
- smoothed complexity의 정확한 perturbation model과 bound.

## Related Topics

- Shortest Path
- Min-Cost Flow
- Simplex Method
- Smoothed Analysis

## Reference Note

The corresponding handwritten lecture note is [`LP5_Smoothed_Analysis_of_the_SSP_Algorithm.jpg`](../handwritten_notes/LP5_Smoothed_Analysis_of_the_SSP_Algorithm.jpg).
