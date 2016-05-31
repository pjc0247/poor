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
![1](img/1.PNG)<br>
![2](img/2.PNG)<br>
<br>
__token matching__<br>
![3](img/3.PNG)<br>
![4](img/4.PNG)<br>
<br>
__deep__<br>
![5](img/5.PNG)<br>
![6](img/6.PNG)<br>