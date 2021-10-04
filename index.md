---
layout: default
---

# Q: Is COVID-19 just a bad flu?

Since the COVID-19 death cases are still controversial sometimes, we would only inspect the question based on the death toll of the country. Generally speaking, the verification of death is much straight forward.

This includes the deaths caused by all reasons, e.g. heart attack, cancer, influenza or even car accidents. So this number won't try to differentiate the deaths caused by COVID19 or not.


|| 2017 | 2018 | 2019 | 2020 |
|:-----|:-----|:-----|:-----|:-----|
|Death Toll|2,813,503|2,839,205|2,854,838|<strong>3,358,814</strong>|


<div>
  <canvas id="myChart"></canvas>
</div>



The charts <strong>begin from zero</strong>.

So, based on the statistics alone, we may conclude that somethings did happen in 2020 that caused significant increase of death toll. Some thing so big that's highly unlikely to be totally ignored by the media.


As a matter of fact, CDC also provided [detailed information of death cases by flu](./death-by-flu.html).

## Death by Flu

The CDC data also contains the death count of different diseases. Here are the death count of each year for all causes vs influenza.

|| 2017 | 2018 | 2019 | 2020 |
|:-----|:-----|:-----|:-----|:-----|
|Deaths per 100,000 population|731.9|723.6|715.2|<strong>828.7</strong>|
|Deaths due to influenza and pneumonia per 100,000 population|14.3|14.9|12.3||


## References:
[CDC: Mortality in the United States, 2017](https://www.cdc.gov/nchs/products/databriefs/db328.htm)<br/>
[CDC: Mortality in the United States, 2018](https://www.cdc.gov/nchs/products/databriefs/db355.htm)<br/>
[CDC: Mortality in the United States, 2019](https://www.cdc.gov/nchs/products/databriefs/db395.htm)<br/>
[CDC: Provisional Mortality Data — United States, 2020](https://www.cdc.gov/mmwr/volumes/70/wr/mm7014e1.htm)



  <script>


    $(document).ready(function(){

      const labels = [
        '2017',
        '2018',
        '2019',
        '2020',
      ];

      const data = {
        labels: labels,
        datasets: [{
          label: 'Death Toll',
          backgroundColor: ['rgb(255, 159, 64)','rgb(255, 159, 64)','rgb(255, 159, 64)', 'rgb(255, 99, 132)'],
          data: [2813503, 2839205, 2854838, 3358814],
        }],
      };
      
      const config = {
        type: 'bar',
        data: data,
      };

      var myChart = new Chart(
          document.getElementById('myChart'),
          config,
	  	
        );
    });

  </script>