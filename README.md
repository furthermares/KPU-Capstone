## TODO
- Need to ask what format the coordinates come as.
- Is vector necessary? Or just detecting suddent movements enough?

## Main
- 수행계획서: https://docs.google.com/document/d/1HsjvmisM-qGdgWI6HiAXHPWDTL0hCVT5uVQtCxlRNeM/edit

## Detailed Designs in docs
##### 참여도 계산
- [ ] 얼굴 인식: 눈, 코, 입, 특히 동공의 위치를 알아냄. 이를 통해 얼굴의 극좌표를 계산.
  - Ask which format they come in
- [ ] 시선 벡터: 위 극좌표에서 알아낸 얼굴의 각도와 동공의 위치를 기반으로 시선이 어디를 향하는지 계산.
  - Add to list every sec.
- [ ] 시선 분산: 시선의 위치를 실시간으로 기록하여 시선 분산도를 계산.
  - List %
- [ ] 화면 위치: 시선이 가장 많이 분포된 지점을 화면의 위치로 설정. (화면 앞에서 화면에 눈길이 가지 않기가 힘든 점과 강의 길이가 최소 50분인 점을 토대.)	
  - List % Highest
##### 참여도 활용
- [ ] 시선 고정률: 위를 토대로 화면에 얼마나 집중해 있나 가늠이 가능함.
- [ ] 참여도 급감: 클라이언트의 집중도가 갑자기 떨어질 경우, 이를 감지. 이는 클라이언트와 선택하면 호스트에게 기록. (한마디로 한 눈 파는 사람을 교수님이 불러 수업의 흐름을 방해하지 않고, 클라이언트 측에서 알림.)
- [ ] 자리 비움: 자리를 비울 경우나 기타 경우에 참여도 기록을 일시정지. (눈 깜박임부터 조는 행위까지 다룸.)
##### 참여도 집계
- [ ] 군집화: 참여도 순 클라이언트를 나열하여 상위 및 하위 군집을 가려냄.
  - 4th Report
- [ ] 기록: 이 지표는 기록이 되고, 클라이언트 별, 과목 별, 시간대 별, 호스트 별로 필터링 함.
  - 4th Report
