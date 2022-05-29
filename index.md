---
layout: default
---

<h1>News/Activities</h1>
<div class="myDIV"><p><a href="#LF1">BLOG ENTRY: Monday, May 2nd 2022: Lea reports on our trip to Vilnius!</a></p></div>
<div class="hide"><p>Arqus twinning workshop in Vilnius</p></div>
<div class="myDIV"><p><a href="#VS1">On Friday, April 22, Vesela Simeonova presented at the Chicago Linguistic Society</a></p></div>
<div class="hide"><p>Epistemic Future in Reflective Questions</p></div>
<div class="myDIV"><p><a href="#MC1">BLOG ENTRY: April 15th 2022 Maya Cortez Espinoza presents work in progress</a></p></div>
<div class="hide"><p>Predicting the Interpretation Probabilities with the help of the Monte Carlo Simulation</p></div>
<div class="myDIV"><p><a href="#ML1">BLOG ENTRY: March 18th 2022: Melanie Loitzl presents work in progress</a></p></div>
<div class="hide"><p>The role of gender in the usage of the definite article with proper names in German</p></div>

<div id="LF1">
    <h4>Lea reports on our trip to Vilnius! Blog entry on Monday, May 2nd 2022</h4>
    <h3 style="margin-top:0pt">Arqus twinning workshop in Vilnius</h3>
    <p>
       

<a target ="_blank" href="images/vilnius4.jpeg" title ="Click me!"> <img style="float:left; width:130px; padding: 5px;" src="images/vilnius4.jpeg" alt="vilnius pic 4"></a>

<a target ="_blank" href="images/vilnius1.JPG" title ="Click me!"> <img style="float:right; clear: none; width:130px; padding: 5px;" src="images/vilnius1.JPG" alt="vilnius pic 1"></a>

<a target ="_blank" href="images/vilnius2.JPG" title ="Click me!"> <img style="float:right; clear: right; width:130px; padding: 5px;" src="images/vilnius2.JPG" alt="vilnius pic 2"></a>
       
<a target ="_blank" href="images/vilnius5.jpeg" title ="Click me!"> <img style="float:right; clear: right; width:130px; padding: 5px;" src="images/vilnius5.jpeg" alt="vilnius pic 5"></a>
        
<a target ="_blank" href="images/vilnius6.jpeg" title ="Click me!"> <img style="float:left; clear:left; width:130px; padding: 5px;" src="images/vilnius6.jpeg" alt="vilnius pic 6"></a>

Together with <a href="https://alexandrecremers.com/">Alexandre Cremers</a>, researcher at Vilnius University, we organized a joint workshop as part of the twinning program by the <a href="https://www.arqus-alliance.eu/">Arqus European University Alliance</a>.          
Five students of our group travelled together with Edgar Onea to Vilnius for a week to work on methodological questions in empirical linguistic research. The workshop thematically connected to and built on an ongoing cooperation between Alexandre Cremers, Edgar Onea and Lea Fricke. In their joint research, they experimentally investigate different prompts and response tasks commonly used in linguistic research with regard to their validity and their efficiency. The program of our workshop included sessions on statistical model building, Bayesian statistics and experimental design as well as talks by Alexandre Cremers, Maya Cortez, Lea Fricke and Edgar Onea. We learned a lot in this week and enjoyed the exchange with students from the philology department in Vilnius. Beside the academic activities, we explored the beautiful capital of Lithuania, went on a trip to Trakai island castle, and got to know plenty of local delicacies.
  </p> 
    </div>

<div id="VS1">
    <h4>Vesela presented at the <a href="http://chicagolinguisticsociety.org/">CLS 58 </a> on April 22nd</h4>
    <h3 style="margin-top:0pt">Epistemic Future in Reflective Questions</h3>
    <p>Find her poster and additional information [here](/previous_talks/vesela_cls.md)!
        <a href="mailto:vesela.simeonova@uni-graz.at">Write me an e-mail</a>
    </p>  
</div>

<div id="MC1">
    <h4>Maya presents work in progress. Blog entry on April 15th, 2022</h4>
    <h3 style="margin-top:0pt">Predicting the Probability of an Interpretation with the help of the Monte Carlo Simulation</h3>
    <p>
    [Lea Fricke](https://homepage.uni-graz.at/de/lea.fricke/) and I recently conducted an experiment on the effect of tense on scalar implicatures (SIs in the following). In this study, subjects had to judge sentences like (1) and (2) with respect to contexts in which everybody of a relevant set of people performed an activity or just a subset of these people. The idea is that for past tense sentences like (1), a scalar implicature is very likely to arise and “some” will be interpreted as “some and not all”. This means, in a context in which the whole set of people performed the respective activity, the sentence will likely be judged false, but sentences, in which just a subset of people performed the activity, the sentence will be true. For future tense sentences like (2), the SI will not be present, “some” will mean “some and possibly all”, and for both kinds of context, the sentence will be judged true. 
      <img 
           src="images/example_sis.jpg" 
           alt="A linguistic example showing Scalar Implicatures" 
           style="
                  height:100px;
                  float: left;
                  padding:7px;">
    
We hypothesize, however, that subjects can access both readings ([+SI ~ “some and not all”] and [-SI ~ “some and possibly all”]) and have beliefs about how likely a sentence is to have a certain reading. We further believe that these reading probabilities vary for each person and for each of the two tenses (additionally to varying between other factors as well), and to judge a sentence a certain way, the respective reading has to have sufficiently high probability. More concretely, we assume that for each tense, the probability of a reading is “beta-distributed” within a population. Just like with a normal distribution, there are values (of reading probabilities), that are more likely to be found in members of the population and there are values that are less likely to be found. Finding the parameters of this distribution is, however, not quite trivial. 
Our goal is to do this using a Markov-Chain-Monte-Carlo-Simulation. This is a mathematical method for solving complex statistical problems with the help of chance. The underlying idea is the law of large numbers: When running independent tests repeatedly, the found parameters will converge with the real parameters as the number of trials approaches infinity. As can be seen in the following, this principle is in accordance with one’s intuition. When throwing a coin, the higher the number of throws, the better we know the probabilities for getting heads/tails as a result.  This means that drawing random samples is the key to estimating probabilities if the probabilistic space is too large to be covered entirely. 
Applying this idea, we create parameters for a possible distribution of reading probabilities. From this distribution, we draw random samples, i.e. we sample random people from an imagined population. We then compare how close these randomly sampled people are to the people we had in our experiment, considering the data we gathered. What we get is a likelihood with which our data fits the distribution. Then, we change the parameters of our distribution slightly and sample randomly again to see whether the new distribution fits our data better. If it does, we accept the new distribution and move on from there, if not, we use the old distribution again, change the parameters slightly and see where we get. We do this very, very often (e.g. 2000 times) and eventually, we will have many distribution parameters, most often those that fit our data best. And with that, we know which parameters of a distribution are likely to be in the population we experimented on. So in the end, we expect to find significantly different distributions for both tenses. And just like that, we will know whether the interpretation of “some” differs between future and past sentences. 

</p>  
</div>

<div id="ML1">
    <h4>Melanie presents work in progress. Blog entry on March 18th, 2022. </h4>
    <h3 style="margin-top:0pt"> The Role of Gender in the Usage of the Definite Article with Proper Names in German </h3>

    Last week Melanie gave first insights into our research project on the use of definite articles with proper names.
    We tested a previous work’s hypothesis that there is a difference between the article usage before male and female first names. 
    (Other gender identities cannot be taken into account because our corpus of language data does not provide specific information about this.) 
    Based on our current data, there seems to be little difference between the two genders, both in terms of the usage of a definite article in general 
    (i. e. optional + required definite articles together) and in terms of only the optional usage of a definite article. However, 
    as to the case of the general usage of the definite article an article appears to be used more often with female names in dative. 
    If this difference is statistically significant, we have yet to find out, because we are still calculating our data at the moment.
    Our working hypothesis is that the use of definite articles often expresses a relationship of proximity but can also have pejorative purposes.
</div>
