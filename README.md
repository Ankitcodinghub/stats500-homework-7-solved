# stats500-homework-7-solved
**TO GET THIS SOLUTION VISIT:** [STATS500 Homework 7 Solved](https://www.ankitcodinghub.com/product/stats500-homework-7-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96601&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;STATS500 Homework 7 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
<ol>
<li>Use the stackloss data in library(faraway) and fit a model with stack.loss as the re- sponse, the other three variables as predictors – consider the following methods:
(a) Least squares

(b) Least absolute deviations

(c) Huber method

(d) Least trimmed squares

Now use diagnostic methods to detect the existence of any outlier or influential point. Remove the point(s) and then repeat the process. Please comment on your analysis outcomes.
</li>
<li>Use the aatemp data from 1881 to 2000 and let temp be the response and year as the predictor and consider the following models:
<ul>
<li>Orthogonal Polynomials to the 4-th degree.</li>
<li>Orthogonal Polynomials to the 5-th degree.</li>
<li>Orthogonal Polynomials to the 6-th degree.</li>
<li>Cubic spline with three internally evenly spaced knots (see the R-comments below)
<pre>     (a) Is there an increasing linear trend in temperature?
</pre>
<pre>     (b) Suppose we also fit the dataset using an AR-1 error structure for the 5-th
         degree orthogonal polynomial.  Select one of the tests in the outcomes from
         ‘‘interval(g)’’ below to justify the use of LS without considering correlations
         among errors.
</pre>
<pre>     (c) Based on these outcomes, would you suggest to use an polynomial with an even
         higher order to model this dataset?
</pre>
<pre>  3. Use the ‘‘ozone’’ data set from Faraway library.  You can use
</pre>
<pre>     &gt; library("faraway")
     &gt; data(ozone)
     &gt; summary(ozone)
</pre>
<pre>     to learn about each variable in the data set.  Fit a model with ‘‘O3’’ as the
     response and ‘‘temp’’, ‘‘humidity’’ and ‘‘ibh’’ as predictors and use the Box-Cox
     method to determine the best transformation on the response.  Report your outcome.
</pre>
You may file the following comments helpful

<pre>library(faraway); data(aatemp)
year&lt;-aatemp$year[-(1:3)]; temp&lt;-aatemp$temp[-(1:3)]
out5&lt;-lm(temp ~ poly(year, 5))
library(nlme)
</pre>
</li>
</ul>
</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<pre>g &lt;- gls(temp ~ poly(year, 5), correlation=corAR1(form=~year), data=aatemp,
subset=(1:115)[-(1:3)])
intervals(g)
library(splines)
</pre>
<pre>choice&lt;-seq(min(year), max(year), length =5);
knots &lt;- c(rep(choice[1],4), choice[2:4], rep(choice[5],4))
bx &lt;- splineDesign(knots, year, outer.ok = TRUE)
gs &lt;- lm(temp ~  bx-1)
</pre>
<pre>plot(year, temp)
lines(year, fitted(out5), col=2, lwd=2)
lines(year, fitted(gs), col=4, lwd=2)
</pre>
</div>
</div>
</div>
