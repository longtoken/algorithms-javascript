# algorithms-javascript

## 计算两个非负整数p和q的最大公约数

<pre><code>
function gcd(p, q) {
  if (q === 0) return p;
  var r = p % q;
  return gcd(q, r);
}
</code></pre>

## 数组倒序
<pre><code>
var len = arr.length;
for (var i = 0; i < len / 2; i++) {
  var temp = arr[i];
  arr[i] = arr[len - 1 - i];
  arr[len - 1 - i] = temp;
}
</code></pre>
