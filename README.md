<!-- CSS only -->
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">
<!-- JS, Popper.js, and jQuery -->
<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js" integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js" integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.5.0/Chart.min.js"></script>

<!DOCTYPE html>
<html lang="en">
<head>
  <title>Demo</title>
</head>
<body style="background-color: darkgrey;">
    <canvas id="bar-chart" width="100" height="25"></canvas>
    <img src='static/Images/bcr-logo.png' style='position:absolute; bottom:0; right:0;' width='20%' height='' alt='' />
</body>
</html>

<script>
    new Chart(document.getElementById("bar-chart"), {
        type: 'bar',
        data: {
          labels: ["t2.micro", "t2.small", "t2.medium", "t2.large", "t2.xlarge"],
          datasets: [
            {
              label: "Price (per hour)",
              backgroundColor: ["#bb86gfc", "#3700b3","#03dac5","#cf6679","#c45850"],
              data: [0.0116,0.023,0.0464,0.0928,0.1856]
            }
          ]
     
    });
    </script>
