# cse474-assignment-3-channel-equalization-solved
**TO GET THIS SOLUTION VISIT:** [CSE474 Assignment 3-Channel Equalization Solved](https://www.ankitcodinghub.com/product/cse474-assignment-3-channel-equalization-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96550&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE474 Assignment 3-Channel Equalization Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
Channel Equalization

Problem Description

When a sequence of bits is transmitted through a channel, they may get distorted because of intersymbol interference (ISI) &amp; noise. The task of channel equalization is to regenerate originally transmitted bit sequence from the received, possibly distorted values.

Assume, the k-th transmitted bit is Ik &amp; received sample is xk. If we assume ISI spans over n successive bits, xk can be expressed as follows.

xk =f(Ik,Ik−1,Ik−2,…,Ik−(n+1))+ηk (1) Here f(.) represents the action of the channel &amp; denotes ηk noise for

k-th bit. We assume f(.) to be a linear function represented as:

n−1 f(Ik,Ik−1,Ik−2,…,Ik−(n+1)) = 􏰀wjIk−j (2)

j=0

We can also assume noise to follow a normal distribution with mean =

0 &amp; variance = σ2.

The task of equalizer is to predict k-th transmitted bit from previous l

successively received samples.

Iˆ =g(x ,x ,x ,…,x ) (3)

</div>
</div>
<div class="layoutArea">
<div class="column">
k k k−1 k−2 k−(l+1)

</div>
</div>
<div class="layoutArea">
<div class="column">
In the above equation, g(.) is the equalizer method. There are several ways for implementing it such as using markov chain model or cluster based approach. In this assignment you have to implement the markov chain model with proper selection of states &amp; Viterbi algorithm for predicting transmitted bit sequence.

1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Input

Read the parameters from a file named ”config.txt”. The description of this file is as follows.

• The first line contains two positive integers n and l.

• Next line contains n space separated real numbers denoting w0, w1, …

, wn−1

• Next line contains a single real number denoting variance of noise, σ2

From another file named ”train.txt”, read a single bit string consisting of 0’s and 1’s, lets call it trainBits.

Finally, read another bit string from ”test.txt” file, lets call it testBits.

Sample

config.txt

32

0.7 0.5 0.1 0.225

train.txt

<pre>00000101001110010111011110100111001011010011100101110111
</pre>
test.txt

0110100011

Here,n=3,l=2,w0 =0.7,w1 =0.5,w2 =0.1,σ2 =0.225

trainBits = 00000101001110010111011110100111001011010011100101110111 testBits = 0110100011

2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
Tasks

<ol>
<li>Construct a markov chain model for which the following is required.
<ul>
<li>Define all possible states based on value of n.</li>
<li>Calculate prior probabilities of all states from trainBits. Note that each consecutive n bits in trainBits refer to a state. [Hint: Prior probability of a state is related to the number of appearances of the state in trainBits]</li>
<li>Calcuate transition probabilities from trainBits. [Hint: Transis- tion probability from state A to state B is related to the count of state transition from A to B in trainBits.]</li>
<li>Assume observation probability follows normal distribution &amp; cal- culate the means of observations.</li>
</ul>
</li>
<li>Transmit testBits, calculate xk’s and use Viterbi algorithm on your markov model to reconstruct originally transmitted bits.</li>
<li>Calculate accuracy by comparing originally transmitted and predicted bit sequence.</li>
</ol>
Marks Distribution

Task Mark Calculate &amp; show prior probabilities 1 Calculate &amp; show transition probabilities 2 Calculate &amp; show observation means 1 Implement Viterbi algorithm for equalization 5

</div>
</div>
<div class="layoutArea">
<div class="column">
Calculate &amp; show accuracy Total

</div>
<div class="column">
1 10

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
