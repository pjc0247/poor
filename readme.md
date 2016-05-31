```cs
ImportAssembly("Newtonsoft.Json.dll");
ImportAssembly("Gogi.dll");

// Basic
// TokenMatching
// Deep
var result1 = TypeCandidates("json", SearchDepth.Basic);

var result2 = MemberCandidates("type_name", "tostring", SearchDepth.Basic);
```

Example
----
__basic__<br>
단순 `StartWith` 메소드와 같습니다. 최상위 우선순위를 가집니다.<br>
![1](img/1.PNG)<br>
![2](img/2.PNG)<br>
<br>
__token matching__<br>
VS에서 제공하는 기능, 중간중간 이름이 기억 안날때도 알려줌<br>
내부적으로 계층화된 인덱스를 사용하여 검색합니다.<br>
![3](img/3.PNG)<br>
![4](img/4.PNG)<br>
<br>
__deep__<br>
오타로 의심되는 경우, `JaroWinkler` 를 사용한 거리비교를 수행합니다.<br>
![5](img/5.PNG)<br>
![6](img/6.PNG)<br>