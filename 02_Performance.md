# 23-2 Computer Architecture 
# 02 Performance

- Performance = 1 / execution time (response time)
- X is N time faster then Y <br>
  <em> Executions time <sub>y</sub> / Executions time <sub>x</sub> </em>

- clock rate = 1 / clock period

<table>
  <thead>
    <tr><th>pico</th><th>nano</th><th>Micro</th><th>Milli</th><th>-</th><th>Kilo</th><th>Mega</th><th>Giga</th><th>Tera</th><th>Peta</th></tr>
    <tr><th>10<sup>-12<sup></th><th>10<sup>-9<sup></th><th>10<sup>-6<sup></th><th>10<sup>-3<sup></th><th>10<sup>0<sup></th><th>10<sup>3<sup></th><th>10<sup>6<sup></th><th>10<sup>9<sup></th><th>10<sup>12<sup></th><th>10<sup>15<sup></th></tr>
  </thead>
</table>

- cpu time = clock cycles X clock period = clock cycles / clock rate = instructions count X CPI / clock rate = instructions count X CPI X clock period
  
- 같은 명령어 집합구조면 명령어 수 같다.

++More about
- Benchmark: 컴퓨터의 성능을 비교하기 위해 선택된 프로그램

$$\sqrt{\Pi Execution time <sub>REF</sub>/ Execution time <sub> X</sub>}$$

- Amdahl's law
개선후 실행시간 = 개선에 의해 영향을 받는 실행시간 / 개선의 크기 + 영향을 받지 않는 실행시간

ex) 100s 걸리는 프로그램에서 80s는 곱하기 계산에 소요된다. 5배 빠르게 실행되게 하려면 곱셈속도를 얼마나 개선해야하는가? <br>
개선 후 실행시간 =80s / n + (100s-80s) <br>
20s = 80s / n + 20s <br>
0 = 80s / n --> 불가능 <br>




