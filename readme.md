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
![1](img/1.png)<br>
<br>
__token matching__<br>
![2](img/2.png)<br>
![3](img/3.png)<br>
![4](img/4.png)<br>
<br>
__deep__<br>
![5](img/5.png)<br>
![6](img/6.png)<br>