# algorithms-javascript

## 计算两个非负整数p和q的最大公约数
function gcd(p, q) {
  if (q === 0) return p;
  var r = p % q;
  return gcd(q, r);
}

