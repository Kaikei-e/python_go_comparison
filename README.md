# Go Python サーバー比較

### パフォーマンス比較

コンパイラ言語のGoの方が当然高速になる。最も遅くて同等か、最速で20倍近くなど環境によって大きく変わる場合もあるが、基本的にGoの方がかなり高速に処理できることが以下のリンクのベンチマークからわかる。

<br>
- [the link](https://itnext.io/compare-c-js-python-python-numba-php7-php8-and-golang-in-prime-number-calculation-55e82b6f82a9)
- [General benchmark](https://benchmarksgame-team.pages.debian.net/benchmarksgame/fastest/go-python3.html)

- [Collatz数列のベンチマーク](https://rheotommy.hatenablog.com/entry/2020/07/18/205343)
  - Go is 10~25x faster

- APIレスポンス
  - Go is 4x faster [link](https://djangostars.com/blog/my-story-with-golang/)

  <br>

  <img src="./imgs/go-pyhon.jpeg" width=70%>
  <br>

  *[the source](https://djangostars.com/blog/my-story-with-golang/)

  <br>

  - web framework benchmark : Go is 1.5x~11x faster

  <img src="./imgs/benchmark2.jpeg" width=70%>

  <br>

  *[the source](http://ziutek.github.io/web_bench/)

- Switched from Python to Go
  - [thought](https://softwareengineeringdaily.com/2021/03/03/why-we-switched-from-python-to-go/)



### テスト容易性

- テストを書くことでソースの質が上がる。事前にバグを見つけることができ、未知のバグや原因不明のバグが減る。

  - Goには言語に標準でテストツールが揃っており、結果を用いた分析なども容易に可能
  - Pythonにも標準のテストモジュールは存在する。大きくわけて3つの段階のものが存在する。ソースに書き込むもの、より一般的な、Goのように別ファイルに記載し実行するもの、フレームワークのpytestなどを利用したもの

### 型付けの強み
- 静的型付け言語は、極論すればソースがよりドキュメントに近くなりえて、ソースの可読性やバグ追跡のしやすさも向上する。
