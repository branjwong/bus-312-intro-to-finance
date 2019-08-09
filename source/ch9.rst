Ch 9: Business Investment Analysis
==================================

- **business investment analysis**, an investigation into the merits of long-term business investments

    - a.k.a. Capital Expenditure Analysis, Real Asset Investment Analysis, or Capital Budgeting

- common finance question: "what is the return on this business investment?"

    - "how does this business investment compare to a financial investment with the same risk?"

Pitfalls of Business Investment Analysis
----------------------------------------

- prediction of future cash flows is a limitation of business investment analysis

    - cash flows typically depend upon revenues, and realized cash flows can vary tremendously from forecasts
    - analysis can help you learn about your investment
    - analysis can help you uncover ways to increase cash flows
    - analysis can help you uncover ways to reduce cash flow variability

- the quantitative nature of business investment analysis is a pitfall

    - placing a dollar value on future benefits has a way of suggesting exactness/certainty that does not actually exist in one's business environment
    - can be good to have optimistic, most likely, and pessimistic sales forecasts

- cash flow predictions have a way of being overly optimistic

    - any investment in an organization has a *champion*
    - champions are often incentivized to exaggerate the prospects for future benefits in order to see their investment accepted
    - benefits may not be realized for many years -> can be difficult to discipline an investment champion for exaggerated claims 

- business investment analysis is occaisonally used to justify a decision that has been already made for political reasons
- companies grow but typical business investment does not

    - there is no expectation that the investment will end at any fixed future date
    - no expectation that cash flows will grow

NPV and Business Investment
---------------------------

- NPV of a business investment can answer whether the investment is good or not

    - NPV > 0 -> the business investment creates wealth

- **cost of capital**, the opportunity cost for business investment analysis

Payback
-------

- does not take time value of money into account
- does not take into account future cash flows

======  =====   =====   =========
period  1       2       3
======  =====   =====   =========
0       -1000   -1000   -1000
1       100     400     200 
2       200     300     200
3       300     200     200
4       400     100     200
5       1000    1000    200
6                       10000000
PB      4yrs    4yrs    5yrs
======  =====   =====   =========

ARR
---

- accounting rate of return


year        0       1       2       3       4       5
Inv         1000
Inv Value           800     600     400     200     0
Net Inc             200     200     200     200     200

Return              20%*    25%     33%     50%     100%

* 200/1000 = 20%

ARR = Average of Yearly Returns = (20+25+33+50)/5

- does not take time value of money into account
- doesn't take non cash items into account


Internal Rate of Return
-----------------------

.. admonition:: Example of Calculating IRR

    Suppose:

    .. math:: 
        
        CF_{t=0} = -1000 \\
        CF_{t=1} = +1200

    Direct Way:

    .. math:: 

        IRR &= \frac {1200-100} {1000} \\
            &= \frac {200} {1000} \\
            &= 0.2
    

    NPV Way

    .. math:: 

            NPV                         &= 0 \\ 
            -1000 + \frac {1200} {1+r}  &= 0, r = IRR \\
         => r                           &= 0.2


.. admonition:: Easy way to think about IRR

    - what is our actual rate of return (== IRR ?)
    - what is the required rate of return (== prime rate ?)
    - if actual > required, good project!

Difficult NPV Calculations
``````````````````````````

::

    t   CF
    0   -1000
    1   400
    2   600
    3   700
    4   300
    5   -200

- what r will make NPV = 0?

.. math:: 

        NPV &= 0 \\ 
        -1000 + 400 / (1+r) + 600 / (1+r)^2 + ... - 200 / (1+r) ^ 5 &= 0 \\ 
    =>  r &= \text{... kind of hard to solve for}


Net Present Value
------------------

Example - A Poor Investment?
````````````````````````````

r = 10%

Cash flows      Leo         Tony
CF_0            +100        -100
CF_1            -150        +150

Leo's Perspective

NPV = 100 - 150/(1+IRR) = 0
100 = 150/(1+IRR)
IRR = 50%

Tony's Perspective

NPV = -100 + 150/(1+IRR) = 0
100 = 150/(1+IRR)
IRR = 50%


.. image:: IRR_vs_interest_rate

Conventional Cash Flows: Out's only followed by Ins only

    - Good if IRR > r

Opposite to Conventional Cash Flows: Ins only followed by Outs only

    - Good if IRR < r


Example - Mulitple Sign Changes
```````````````````````````````

CF_0    -1000
CF_1    +600
CF_2    +600
CF_3    -100
CF_4    +800
CF_5    +800
CF_6    -100


.. math:: 

    NPV     = CF_0 + CF_1/(1+r) + CF_2/(1+r)^2 + ... + CF_6/(1+r)^6 = 0
            => CF_0*(1+r)^6 + CF_1*(1+r)^5 + CF_2*(1+r)^4 + ... + CF_6 = 0

    - solving a polynomial of rank 6
    - 6 roots
    - 6 possible solutions 

.. image:: many_possible_IRRs.png


Example - When to Invest in Which Project?
``````````````````````````````````````````

======  ======= =======
CF_x    A       B
======  ======= =======
0       -100    -1000
1       200     1320
\       \       \
IRR     120%    32%
======  ======= =======

r = 10%

NPV_A = NPV_B
-100+320/(1+r) = -1000 + 1320/(1+r)
900 = 1100/(1+r)
r = 1100/900 - 1 = 0.22

if 10% <= r < 22.2%     both good, B better
if 22.2% < r < 32%      both good, A better
if 32% < r < 120%       A good, B bad
if r > 120%             both bad


Idk Wtf he's going on about here
`````````````````````````````````

Investment in Cash Flows only

- Ignore Financing Cash Flows

Types of Investment

    - Investment in NFA
        
        - also Salage

    - Investment in TC

Things to Consider when Investing in a new Project

    - Substitution Effects

        - A product that satisfies the same basic want as another product is a substitute good

    - Complementary Effects
        
        - suppose you sell burgers, but people want fries: if you sell fries, you will by nature sell more burgers

    - Opportunity Cost
    - Ignore Sunk costs

Example
```````

Investment needed       80000
Sell old today          20000
Salavge new             25000 at t = 4
Project life            4 yrs      
Old Salvage t = 4       10000

CCA = 20% of something?

    Start UCC   Net Add     CCA     End UCC
1   0           60000       6000    54000
2   54000       0           10800   43200
3   43200       0           8640    34560
4   34560       -15000      3912    15648

================    =========   =========   ========    =========   ========
time                0           1           2           3           4    
================    =========   =========   ========    =========   ========
Investment          -80000
Salage old          20000
Salage new                                                          25000
Lost Salavge                                                        -10000
TC                  -8000                                           8000
Rev                             60000       60000       60000       60000
VC                              -20000      -20000      -20000      -20000
FC Saving                       5000        5000        5000        5000
CCA                             6000        10800       8640        3912
\
EBT                             39000       34200       36360       41088
Tax                             -15600      -13680      -14544      -16435
================    =========   =========   ========    =========   ========

- somehow you can calculate NPV from this

NPV = NPV if you ignore CCA + PV CCA Tax Shields

.. image:: _static/tax_shields_over_time.png

.. math::

    \text{PV CCA TS Gained} &= C/(r-g) \\
                            &= Id*\tau/(r+d)

.. math::

    \text{PV CCA TS Gained with half year correction}   &= \text{PV CCA TS Gained} * \text{half year correction} \\
                                                        &= Id*\tau/(r+d) * (2+r)/(2*(1+r))

.. math:: 

    \text{PV CCA TS Loss}   = S*d*\tau/(r+d)/(1+r)^n


- S = salvage value ??
- when you sell you lose your tax shields or something

.. math:: 

    \text{PV CCA Tax Shields}   &= \text{PV CCA TS Gained with half year correction} - \text{PV CCA TS Loss} \\
                                &= Id*\tau/(r+d) * (2+r)/(2*(1+r)) + S*d*\tau/(r+d)/(1+r)^n

PV Investment               -60000*
PV Salvage                  17075 = 25000/1.1^4
PV Salvage lost             -6830 = -10000/1.1^4
Inv in TC                   -8000
TC recovered                5465 = 8000/1.1^4
PV Operational Cash Flows   85586 = 27000**/0.1*(1-1/1.1^4)
PV CCA TS Gained            15215 = 60000 * 0.2 * 0.4 /(0.4 + 0.2) * 2.1 / (2*1.1)
PV CCA TS Losst             -2732 = -15000 * 0.2 * 0.4 / ((0.1 + 0.2) * 1.1^4)
\                           \
NPV                         45836

- *: Investment + Salave old
- **: 

    Extra cash coming in = 60000 - 20000 + 5000 = 45000
    Tax = 18000
    Extra cash coming in - tax = 27000


Example
```````


Buy fro     50000
Sell for    20000       
\tau = 0.4

End UCC     25000

25000
20000
\
5000
5000 - terminal loss
\
0 

Investment = 50000
S = 25000

Tax saving of 5000
    5000 * 0.4 = 2000
    - saving from terminal loss at year 5

.. math::

    \text{PV Tax Saving From Terminal Loss} = 5000*0.4/(1+\tau)^5



Example
```````

Sell for    30000

==========  ======
UCC         25000
Sell        30000
\           \
\           -5000
CCA Recapt  5000
\           \
\           0       
==========  ======


Extra Tax = 5000 * \tau = 2000

Example
```````

Buy for     50000           
Sell for    60000

USS         25000
Disp        50000
            \
            -25000
            25000
            \
            0

I = 50000
S = 25000

PV Recap Tax = -25000 * \tau / (1+r)^5

PV Cap gain tax effect = -10000 * 0.5 * \tau / (1+r)^5

Example
````````

- suppose person says "if IRR higher than rate of return, then good project"
- person saying this doesn't know about the pitfalls
- when does he make incorrect judgements, for any required rate of return
- note: pretty sure that IRR doesn't change as the required rate of return does, but NPV changes as the required rate of return changes

