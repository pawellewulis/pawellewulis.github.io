---

layout: post

title: "Pollsters vs Polymarket"

---

<figure style="max-width: 800px; margin: 1.5em auto; text-align: right;">
  <img src="/assets/img/poll_vs_poly/poll_vs_poly.png"
       alt="Pollsters vs Polymarket"
       style="width: 100%; display: block;">
  <!-- <figcaption style="font-size: 0.8em; color: #000;">
    Source: ?
  </figcaption> -->
</figure>

The great battle between statistics against the wisdom of the crowd. Who wins?

Recently, I came across a paper *Are Betting Markets Better than Polling in Predicting Political Elections?* written by Cutting, Hughes-Berheim, Johnson, Baroud, and Brett Goldstein. The authors analyzed the accuracy of polls conducted during the 2024 Trump vs Harris US election and compare it to the probability of winning for each of the candidates implied by Polymarket.

The case of the US elections suggested that people might have been 'onto something' and perhaps were (consciously or not) aware of some subtleties undetectable via traditional polling methods. On the other hand, though, they might've simply been lucky. I genuinely couldn't tell, so I decided to put this hypothesis to a little test.

# What are the criteria?

For the sake of simplicity, I decided to include only the 1 vs 1 presidential elections that took place since 2024 and were decided by nationwide voting. We've got only 20 samples due to not-so-secret reasons:

- There are fewer than 100 countries that are widely considered democratic.

- Some democratic countries are monarchies.

- In many democratic countries, the president is chosen by a parliament or another institution.

- In some cases, a presidential election might get resolved without a 1 vs 1. 

- Sometimes there isn't a Polymarket market for some event (especially true for anything before mid 2024).

Another obstacle is that in some cases one candidate had such an enormous advantage that a victory was almost trivial to foresee. If we define a 1 vs 1 election to be "interesting" if no candidate has an implied probability of winning exceeding 90% (Polymarket, the election day midnight), then we are left with… 6 examples. 

I'm not gonna lie, the resulting sample size turned out to be more disappointing than I expected. While we can't perform any meaningful statistical analysis here, I was still interested in which side would come on top.

# Results


<figure style="max-width: 800px; margin: 1.5em auto; text-align: right;">
  <img src="/assets/img/poll_vs_poly/poly_week.png"
       alt="Polymarket Probs"
       style="width: 100%; display: block;">
  <figcaption style="font-size: 0.8em; color: #000;">
    Source: Polymarket data
  </figcaption>
</figure>

Below, <b>Adjusted Polling Margin</b> represents the average advantage of the winning candidate in the runoff election polls, with the two most extreme measurements discarded. Of course, there are no runoff elections in the US, so I had to make a compromise and consider the final polling averages instead. 

For the Polymarket, I considered the implied probability at midnight just before the election day.

The colours in this table were chosen rather arbitrarily. In the APM column, we award the yellow label to those within 1 pp. of 50%. As for the Polymarket columns, I wasn't exactly certain whether Romania's 46.5% should be yellow or red, but eventually I went with red.


<table style="width:100%; table-layout:fixed;">

  <colgroup>
    <col style="width:25%;">
    <col style="width:25%;">
    <col style="width:25%;">
    <col style="width:25%;">
  </colgroup>

  <thead>
    <tr>
      <th>Country</th>
      <th align="center">Polymarket Implied Probability</th>
      <th align="center">Adjusted Polling Margin</th>
      <th align="center">Winner</th>
    </tr>
  </thead>
 <tbody>
  <tr>
    <td>Slovakia</td>
    <td align="center" style="background-color:#fff2cc;">50.0%</td>
    <td align="center" style="background-color:#f4cccc;">−1.05 pp</td>
    <td align="center">Polymarket</td>
  </tr>

  <tr>
    <td>USA (popular vote)*</td>
    <td align="center" style="background-color:#f4cccc;">26.3%</td>
    <td align="center" style="background-color:#fff2cc;">−0.67 pp</td>
    <td align="center">Pollsters</td>
  </tr>

  <tr>
    <td>Equador</td>
    <td align="center" style="background-color:#f4cccc;">42.5%</td>
    <td align="center" style="background-color:#f4cccc;">−1.27 pp</td>
    <td align="center">Neither</td>
  </tr>

  <tr>
    <td>Romania</td>
    <td align="center" style="background-color:#f4cccc;">46.5%</td>
    <td align="center" style="background-color:#f4cccc;">−1.38 pp</td>
    <td align="center">Neither</td>
  </tr>

  <tr>
    <td>Poland</td>
    <td align="center" style="background-color:#f4cccc;">36.2%</td>
    <td align="center" style="background-color:#fff2cc;">−0.55 pp</td>
    <td align="center">Pollsters</td>
  </tr>

  <tr>
    <td>Seychelles</td>
    <td align="center" style="background-color:#d9ead3;">74.0%</td>
    <td align="center" style="background-color:#fff2cc;">**</td>
    <td align="center">Polymarket by W.O.</td>
  </tr>

  <tr>
    <td>Bolivia</td>
    <td align="center" style="background-color:#d9ead3;">53.6%</td>
    <td align="center" style="background-color:#f4cccc;">−7.95 pp</td>
    <td align="center">Polymarket</td>
  </tr>

  <tr>
    <td>Colombia</td>
    <td align="center" style="background-color:#d9ead3;">83.5%</td>
    <td align="center" style="background-color:#d9ead3;">7.75 pp</td>
    <td align="center">Tie</td>
  </tr>
</tbody>
  <tfoot>
    <tr>
      <td colspan="3">
        <small><sup>*</sup>  Not exactly a proper 1v1. </small>
        <br>
        <small><sup>**</sup> There was no reputable runoff poll for Seychelles.</small>
      </td>
    </tr>
  </tfoot>
</table>

If I were forced to pick a winner, I would say: neither? As already said, the sample is very limited, but apparently if the chances look roughly 50/50, they might indeed be 50/50, and no one truly knows what will happen.

I am, however, impressed by how well Polymarket fared in Bolivia's case. I am far from an expert on Bolivian politics, so I can't tell whether it happened because of unusual restrictions on pollsters or a massive, rapid shift in sentiment.

Another interesting case is Peru, where the wave function of Polymarket failed to collapse even a full day after the election.

Honorable mention goes to Poland for the most dramatic swing.
