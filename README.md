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
function reverse(arr) {
  var len = arr.length;
  for (var i = 0; i < len / 2; i++) {
    var temp = arr[i];
    arr[i] = arr[len - 1 - i];
    arr[len - 1 - i] = temp;
  }
  return arr;
}
</code></pre>

## 质数又称素数。一个大于1的自然数，除了1和它自身外，不能整除其他自然数的数叫做质数；否则称为合数。
<pre><code>
function isPrime(N) {
  if (N < 2) return false;
  for (var i = 2; i * i <= N; i++)
    if (N % i === 0) return false;
  return true;
}
</code></pre>

## 调和级数（Harmonic series）是一个发散的无穷级数。
<pre><code>
function H(N) {
  var sum = 0;
  for (var i = 1; i <= N; i++)
    sum += 1 / i;
  return sum;
}
</code></pre>

## 随机返回
<pre><code>
// [a,b)
function uniform(a, b) {
  return a + Math.random() * (b - a);
}
// [0..N)
function uniform(N) {
  return Math.random() * N;
}
// [lo, hi)
--- StdRandom.uniform(lo-)
// 根据离散概率随机返回int值
function discrete(arr) {
  var r = Math.random();
  var sum = 0;
  for (var i = 0; i < arr.length; i++) {
    sum = sum + arr[i];
    if (sum >= r) return i;
  }
  return -1;
}
// 随机排序

</code></pre>






