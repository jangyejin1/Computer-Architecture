# 23-2 Computer Architecture 
# 03 ISA

- Instruction Set Architecture(ISA) : Language of the computer & an interface between SW and HW  <br>
intructions의 유형, 데이터 사용법, 데이터 형식, instructions 형식

- Design principle 1: Simplicity favors regularity  <br>
  " 1 operation & 3 operands " <br>

- Design principle 2: Smaller is faster  <br>
  피연사자는 레지스터라는 하드웨어로 직접 구현된 특수 위치 몇 곳에 있는 것만을 사용할 수 있다. <br>
  레지스터는 32비트, 32비트를 한 덩어리로 word <br>
  " 산술 명령어의 각 피연산자는 32개의 32비트 레지스터 중 하나이어야 한다." <br>
  왜 32개의 레지스터를 사용하는가? (추가)
   <br>
  --레지스터 개수보다 많은 데이터 원소는? <br>
  "메모리를 사용한다." -> 산술연산은 레지스터에서만 실행되므로 메모리와 레지스터간 주고받는 명령어 필요
  <br>
- data transter instruction
 lw (메모리 -> 레지스터) <br>
 sw (레지스터 -> 메모리)
 <br>
- 명령어가 메모리 주소를 지정, 메모리는 0부터 시작
- 워드는 4바이트(32bits) -> 주소 4씩 차이남,레지스터 또한 32bit 데이터 범위
 <br>
- alienment restrictions : 메모리 내에서 데이터는 자연스러운 경계를 지켜서 정렬되어야 한다. <br>
n의 배수 데이터 주소, n size의 데이터  <br>
 <br>
- big endian: 앞쪽이 앞  <br>
 <br>
- Design principle 3: Make the common case fast  <br>
  "16-bit 수치 피연산자 처리를 위한" addi, $zero <br>
- Design principle 4: Good design demands good compromise
  "모든 지침을 동일한 길이로 균일하게 유지"
  <hr>
  -R-format
  -I-format (mips 표 참고)

  
