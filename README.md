# -CSEG483-CSE5483-HW-1-reduction-
[CSEG483/CSE5483] HW 1: 간단한 reduction 응용

**Download Link:https://programming.engineering/product/cseg483-cse5483-hw-1-%ea%b0%84%eb%8b%a8%ed%95%9c-reduction-%ec%9d%91%ec%9a%a9/**

Description
5/5 – (2 votes)
제출 마감: 4월 10일(수) 오후 8시 정각 이전에 조교가 사이버 캠퍼스에 공지한 방식으로 제출

참고: LATE 없음

0과 1 사이의 n개의 31-비트부동 소수점 숫자 x0, x1, · · · , xn−1의 평균, 분산, 최소값, 그리고최대값을 구해주는 CUDA 프로그램을작성하라.

입력데이터는수업 시간의사용한예제 코드의방법을사용하여 생성하라.

분산 값은 Var(X) = E(X2) − E(X)2 공식을사용하여 계산하라.

방법

[방법 1] Host에서 작동하는다음함수를 구현하라.

void HW1 host(int n, float* A, float* average, float* variance, float* maximum, float* min-imum);

[방법 2] 수업 시간에 설명한 reduce1 커널의 방식을 적절히 확장하여 구현하라.

void HW1 reduce1(int n, float* A, float* average, float* variance, float* maximum, float* minimum);

[방법 3] CUDA에서 제공하는 thrust 라이브러리 함수를 적절히 사용하여 구현하라. (참고: https://nvidia.github.io/cccl/thrust/와 https://docs.nvidia.com/cuda/에서 관련 문서를 찾을 것.)

void HW1 thrust(int n, float* A, float* average, float* variance, float* maximum, float* minimum);

참고: 자신의 실험은다음의 내용을 포함해야 한다.

먼저 보고서 가장 앞에 자신이 실험을 수행할 때어떤 GPU를사용했는지를 반드시 기술하라.

각함수가동일한입력 n과 A에 대하여 동일한 결과값 average, variance, maximum, 그리고 minimum

을산출하는지, 아니면방법에 따라약간의차이가 있는지 확인하라.

각함수에 대한 수행 시간은 수업 시간에 설명한 host에서의측정 방법을사용하라.

충분히 큰 서로다른 데이터크기 n에 대하여 thread block의 크기를 바꾸어 가면서속도변화가 있는지관찰하라.

제출물: 자신이 구현한 코드를이름이 HW 1 학번인 디렉터리 아래의 Visual Studio 프로젝트를생성한 후, zip으로압축하여 제출할 것.

자신이작성한코드: Visual Studio 2022를 통하여 확인할 수 있도록 위의 directory를 제출하되 .vs

파일 등 코드 수행에불필요한 파일들은 반드시 제거한 후 제출할 것.

프로그램 실행결과: 자신의 코드를 실행한 결과를 증빌할 수 있는자료(예를 들어, 콘솔 윈도우의 내용을캡춰한 영상)를 보고서에포함할 것.

보고서: 자신의 실험 결과를 바탕으로분석한 내용을 기술할 것.

– [CSEG483/CSE5483] 기초 GPU 프로그래밍 HW 1 (2024년 4월 10일 (수) 오후 8:00 마감) –
