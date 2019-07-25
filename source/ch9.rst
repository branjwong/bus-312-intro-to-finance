Business Investment
===================

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


IRR
----

- what is our actual rate of return
- what is the required rate of return
- if actual > required, good project!

Example
```````

::

    CF_{t=0} = -1000
    CF_{t=1} = +1200

    IRR = (1200-100)/1000 = 200/1000 = 20%

NPV = -1000 + 1200 / (1+r) = 0 => r = 0.2

Example 2
`````````

::

    t   CF
    0   -1000
    1   400
    2   600
    3   700
    4   300
    5   -200

- what r will make NPV = 0?

NPV = -1000 + 400 / (1+r) + 600 / (1+r)^2 + ... - 200 / (1+r) ^ 5 = 0 => r = ... kind of hard to calc


Net Present Value
------------------

- npv (net present value of a project) = present value of benefits (of project) - present value of costs (of project)
- look at cash flows
- take present value of all outflows = today's equivalent value of the cost of the project
- take present value of all inflows = today's equivalent value of all of the benefits of the project
- benefits > costs = good project! or if benefits - costs > 0 -> good project!

Example
```````

CF_{t=0} = -100
CF_{t=1} = -120

NPV = -100 + 120/(1+r)

.. image:: _static/npv_schedule.png


Assignment 9 - Question 4
`````````````````````````

==============  ============
Elect           20  
Chem            X
\               \
MV              20+X
\               \
Sh Pr           (20+X)/n
\               \
Inv needed      24
Rights/Share    1:1
==============  ============

#Sh             2n
New MV          20 + x + 24
New Shp         (44 + x)/2n

suppose:

    .. math::     

        (44+x)/2n = 0.75*(20x)/n
        x = 28


Value of a right = 0.80

    - value of the right is a function of the share price, so you can figure out the old share price from the value of the right

Old Share Price = 0.80/0.25 = 3.20
New Share Price = 2.40

3.2 = (20 + 2.8) / n => n = 4.8/3.2 = 15