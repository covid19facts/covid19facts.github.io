---
layout: default
---

# Q: Is COVID-19 just a bad flu?

Here we inspect the question based on the <strong>overall death toll</strong> of United States. Generally speaking, the confirmation of death is quite straight forward. The numbers below include the deaths of all causes, i.e. heart attack, cancer, influenza, car accidents, etc.


||2016| 2017 | 2018 | 2019 | 2020 |
|:-----|:-----|:-----|:-----|:-----|:-----|
|Death Toll|2,744,248|2,813,503|2,839,205|2,854,838|<strong>3,358,814</strong>|


<div>
  <canvas id="myChart"></canvas>
</div>



Even when the numbers are big and y-axis begins from zero, one could easily notice the obvious uprise in 2020.

Based on the statistics alone, we may conclude that <strong>something deadly must have happened in 2020</strong>.

<strong>Unless there are some hideous huge disasters that happened in 2020</strong>, which is overlooked by every one in the country, COVID19 related deaths would best match this number abnormality so far.

<br/>
## How About Flu

CDC reports also provided detailed information of death cases by flu. Here are the <strong>death cases per 100,000 standard population</strong>, of each year for all causes vs influenza. 



||2016| 2017 | 2018 | 2019 | 2020 |
|:-----|:-----|:-----|:-----|:-----|
|Deaths per 100,000|728.8|731.9|723.6|715.2|<strong>828.7</strong>|
|Deaths due to influenza and pneumonia per 100,000|13.5|14.3|14.9|12.3||

Flu data of 2020 is not yet available. Yet, we could still see that, <strong>the flu related cases will hardly impact the total death toll in a significant way</strong>.


<br/>
#### References:
[CDC: Mortality in the United States, 2016](https://www.cdc.gov/nchs/products/databriefs/db293.htm)<br/>
[CDC: Mortality in the United States, 2017](https://www.cdc.gov/nchs/products/databriefs/db328.htm)<br/>
[CDC: Mortality in the United States, 2018](https://www.cdc.gov/nchs/products/databriefs/db355.htm)<br/>
[CDC: Mortality in the United States, 2019](https://www.cdc.gov/nchs/products/databriefs/db395.htm)<br/>
[CDC: Provisional Mortality Data — United States, 2020](https://www.cdc.gov/mmwr/volumes/70/wr/mm7014e1.htm)



  <script>


    $(document).ready(function(){

      const labels = [
	'2016',
        '2017',
        '2018',
        '2019',
        '2020',
      ];

      const data = {
        labels: labels,
        datasets: [{
          label: 'Death Toll',
          backgroundColor: ['rgb(255, 159, 64)', 'rgb(255, 159, 64)', 'rgb(255, 159, 64)', 'rgb(255, 159, 64)', 'rgb(255, 99, 132)'],
          data: [2744248, 2813503, 2839205, 2854838, 3358814],
        }],
      };
      
      const config = {
        type: 'bar',
        data: data,
	options: {
		plugins: {
			legend: false
		}
	}
      };

      var myChart = new Chart(
          document.getElementById('myChart'),
          config,
	  	
        );
    });

  </script>