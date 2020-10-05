<script>
  // 1 1 2 3 5 8 13 21...
  // 수열 n = 수열 n-2번째 + 수열 n-1번째

  // 100회차 까지만 출력 (회차기준)
  var n_2 = 1;
  var n_1 = 1;

  console.log(n_2);
  console.log(n_1);

  for (var i = 0; i < 10; i++) {
    var n = n_2 + n_1;
    console.log(n);
    n_2 = n_1;
    n_1 = n;
  }

  console.log("===============");
  console.log(n_2 == n_2);
  console.log(n_1);
  //while

  n_1 = 1;
  n_2 = 1;
  console.log(n_2);
  console.log(n_1);
</script>
