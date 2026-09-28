---

layout: post

title: "Pollsters vs Polymarket"

---

<figure style="max-width: 800px; margin: 1.5em auto; text-align: right;">
  <img src="/assets/img/poll_vs_poly/poll_vs_poly.png"
       alt="Pollsters vs Polymarket"
       style="width: 100%; display: block;">
  <figcaption style="font-size: 0.8em; color: #000;">
    Source: ?
  </figcaption>
</figure>

The great battle of the good ol' statistics against the wisdom of the crowd. Who wins?

Recently, I read an article *Are Betting Markets Better than Polling in Predicting Political Elections?* written by Cutting, Hughes-Berheim, Johnson, Baroud, and Brett Goldstein. The authors analyze in depth the accuracy of polls conducted during the 2024 Trump vs Harris US election and compare it to the probability of winning of each of the candidates implied by Polymarket.

The case of the US elections showed that people might have been 'onto something' and perhaps were (consciously or not) aware of some subtleties undetectable via traditional polling methods. On the other hand, though, they might've simply been lucky. I genuinely couldn't tell, so I decided to put this hypothesis to a little test.

# What are the criteria?

For the sake of simplicity, I decided to take a look at all the 1 vs 1 presidential elections that took place between (?) and (?) and were decided solely by a single voting (popular vote). We've got only 20 samples due to not so secret reasons:

- There are fewer than 100 countries that are widely considered democratic.

- Many democratic countries are monarchies.

- In many democratic countries the president is chosen by a parliament. 

- In some cases a presidential election might get resolved without a 1 vs 1. 

- (TODO): A market on Poly must exist in the first place!

Another obstacle is that in some cases there was a favourite so heavy that a victory was almost trivial to foresee. If we define a 1 vs 1 election to be "interesting" if no candidate has an implied probability of winning exceeding 90% (Polymarket, the day of the election), then we are left with… 6 examples. 

I'm not gonna lie, the resulting sample size turned out to be more disappointing than I had expected. While we can't perform any meaningful statistical analysis here, it might still be interesting to take a look at the results.

# Results

<figure style="max-width: 800px; margin: 1.5em auto; text-align: right;">
  <img src="/assets/img/poll_vs_poly/poly_week.png"
       alt="Polymarket Probs"
       style="width: 100%; display: block;">
  <figcaption style="font-size: 0.8em; color: #000;">
    Source: Polymarket data
  </figcaption>
</figure>



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
    <td>USA (popular vote)</td>
    <td align="center" style="background-color:#f4cccc;">26.3%</td>
    <td align="center" style="background-color:#fff2cc;">−0.67 pp</td>
    <td align="center">Pollsters</td>
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
    <td align="center" style="background-color:#fff2cc;">*</td>
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
    <td align="center" style="background-color:#f4cccc;">7.75 pp</td>
    <td align="center">Tie</td>
  </tr>
</tbody>
  <tfoot>
    <tr>
      <td colspan="3">
        <small><sup>*</sup> There was no reputable runoff poll for Seychelles.</small>
      </td>
    </tr>
  </tfoot>
</table>

(TODO: Equador!)