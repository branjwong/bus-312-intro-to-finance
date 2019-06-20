The Mathematics of Finance
==========================

Introduction
------------

Suppose:

::

    PV = 100
    FV = 110

What's more valuable?

Answer: depends on interest = r


Present Value vs Future Value
-----------------------------

.. math::

    FV  &= PV + rPV \\
        &= PV(1+r) \\

.. math:: 

    FV_{t=2} &= PV(1+r)^2 \\

.. admonition:: Future Value of Investement

    .. math::

        FV_{t=n} = PV(1+r)^n
        
        
    - n = the number of compounding periods  
    - PV = the present value of investment (capital)  
    - :math:`FV_{t=n}` is the future value of an investment at the nth period  

.. note:: 

    - r and n should talk in terms of the same time frame

        - e.g. if r is a per annum percentage, then n should be # years
        - e.g. if r is a monthly rate, then n should be # months



Effective Interest Rates
------------------------

- **Effective Annual Rate (EAR)**, the interest rate as if it were compounded yearly instead of its actual compounding period


Example: Basic Effective Annual Rate
````````````````````````````````````

:: 

    invest                      $100
    each half year get          10%

then

    after 1/2yr you will get    $10
    at t = 1 (year)             $121

    effective half year return = 10%
    eff 1 year return = 21% = EAR = effective annual rate


Effective Interest Rate For 1/n Year
````````````````````````````````````

.. admonition:: Effective Rate for 1/n Year

    .. math::

        \frac {j_n} {n} = eff rate for 1/n year


- **Annual Percentage Rate (APR)**, an interest rate that is expressed as an EAR for an interest rate compounded twice per year (in Canada), often used for expressing the interest rate on items like car financing, etc.


Example: Converting Between Rates
`````````````````````````````````

:: 

    if
    20% p.a. (per annum) compounded twice a year
    APR - compounded twice per year in Canada
    j_2 = 20%

        J implies per year
        2 implies compounded twice per year

.. admonition:: Converting Between Rates


    .. math:: 
        
        EffRate_A = (1 + EffRate_B)^p - 1

    - p = number of A periods in an A period


.. math:: 

    j_2 = 20\% \\
    => eff 1/2 yr   &= 0.2/2 \\
                    &= 0.1 

.. math:: 

    EAR &= (1 + 0.1)^2 - 1 \\
        &= 0.21 

.. math:: 

    eff month rate = (1 + 0.1)^{\frac 1 6} - 1 \\

.. math:: 

    r_d = 10\% - APR

==  ============    ======
n   eff 1/n yr r    EAR
==  ============    ======
1   0.10            0.10
2   0.05            0.1025
4   0.025           0.1038 
12  0.0083          0.1043
==  ============    ======

.. math::

    EAR_n = (1 + eff 1/n yr r)^n - 1 \\
    \\
    EAR_2 = (1 + 0.05)^2 - 1 = 0.1025 \\
    EAR_4 = (1 + 0.025)^4 - 1 = 0.1038 \\
    \\
    EAR = e^q - 1, \\
        e = Euler's Constant \\
        q = Continuously Compounded Rate \\
    \\
    EAR = e^0.1 - 1 \\
        = 0.10517

Inflation
---------

::

    Invest          100
    nominal r       12%
    Exp r_inf       8%

=========           ====    ======
t =                 0       1       
=========           ====    ======
$/muffin            1       1.08
Cash                100     112     
# muffins           100     103.7   
=========           ====    ======

- :math:`\therefore` real rate of return = r* = 3.7%

- muffins is an analogy for t=0 dollars = real dollars we have at t=1

.. math::

    r*  &= \frac {1+r} {1 + r_{inf}} - 1 \\
    \\
        &= \frac {1 + 0.12} {1 + 0.8} - 1 \\
    \\
        &= 0.037

Perpetuity
----------

- *perpetuity*, a constant, regular stream of cash flows continuing forever and starting in exactly one period

    - constant -> same amount of cash flows every period
    - regular -> periods are regular

Calculating the PV of perpetuity cash flows

Suppose cash flow every period = C

.. math:: 

    PV = \frac {C} {1 + r} + \frac {C} {(1 + r)^2} + \frac {C} {(1 + r)^3} + ...    (1) \\
    PV(1+r) = PV + rPV = C + \frac {C} {1 + r} + \frac {C} {(1 + r)^2} + ...        (2) \\
    \\ 
    rPV = C                                                                         (1 - 2) \\
    \\
    PV = \frac {C} {r}

Example: Basic Perpetuity
`````````````````````````

::

    r = 10%, 
    C = $1000 p.a, starting at t=1

.. math::
    
    PV_{t \geq 1}   &= \frac {C} {r} \\
                    &= \frac {1000} {0.01} \\
                    &= 10000 

Example 2: Displaced Perpetuity
```````````````````````````````

:: 

    r = 10%, 
    C = $1000 p.a, starting at t=0

Method 1
''''''''
.. math::


    PV_{t \geq 0} = PV_{1000} + PV_{t \geq 1}

Method 2
''''''''

.. math::

    PV_{t \geq -1}   &= \frac {C} {r} \\
    \\
    PV_{t \geq 0}   &= PV_{t \geq -1} * (1 + r) \\
                    &= \frac {1000} {0.1} * (1 * 0.1) \\
                    &= 10000


Example: Fractionally Displaced Perpetuity
``````````````````````````````````````````

::

    r = 10%, 
    C = $1000 p.a, starting at t=0.5

.. math::

    PV_{t \geq -0.5} &= \frac {C} {r} \\
    \\
    PV_{t \geq 0}   &= PV_{t \geq -0.5} * (1 + r)^{0.5} \\
                    &= \frac {1000} {0.1} * (1 + 0.1)^{0.5} 


Generalization: Displaced PV
````````````````````````````

.. math::

    PV_{t \geq -n}      &= \frac {C} {r}, n > 0 \\
    => PV_{t \geq 0}    &= PV_{t \geq -n} * (1 + r)^n

and

.. math::

    PV_{t \geq n}      &= \frac {C} {r}, n > 0 \\
    => PV_{t \geq 0}    &= PV_{t \geq n} * \frac 1 {(1 + r)^n}

- multiply PV by :math:`r^n, r = \text{interest rate}, n = \text{number of times r is compounded}` if moving PV forward, divide by it if moving PV back

Annuity
-------

- **annuity**,  a constant, regular, finite cash flow stream starting in exactly one period

    - difference between Annuity and Perpetuity is that the cash flow ends at some point

.. math::

    PV_{1 \leq t \leq n}    &= PV_{t \geq 1} - PV_{t \geq n} \\
                            &= (\frac {C} {r}) - (\frac {C} {r} * \frac {1} {(1+r)^n})  \\
                            &= \frac {C} {r} * (1 - \frac {1} {(1+r)^n}) \\
    \\
    where, \\
    \\
    n = \text{number of cash flow periods}

Example: Basic Annuity
``````````````````````

::

    r = 10%
    Annual cash flows starting in 1 yr
    n = 20

.. math::

    PV  &= \frac {C} {r} * (1 - \frac {1} {(1+r)^n}) \\
        &= \frac 1000 0.1 * (1 - \frac 1 {1.1^{20}}) \\
        &= 8513


Example: Displaced Annuity
``````````````````````````

:: 

    r = 10%
    Annual cash flows starting today
    Last cash flow in 20 years

.. math::

    PV  &= \frac {C} {r} * (1 - \frac {1} {(1+r)^n})*(1+r) \\
        &= \frac {1000} {0.1} * (1 - \frac 1 {1.1^{21}}) * 1.1 \\
        &= 9513.56


Example: Displaced Annuity 2
````````````````````````````

::

    What is the value today of a policy that pays $1000 a year. 
    20 cash flows. 
    1st cash flow in 5 year. 
    r = 10%

.. math::

    PV_{0 \geq t \geq 25}   &= PV_{t \geq 5, n=20} \\
                            &= PV_{5 \geq t  \geq 25} \\
                            &= \frac {\frac {C} {r} * (1 - \frac {1} {(1+r)^n})*(1+r)} {(1+r)^4} \\
                            &= \frac {1000} {0.1} * (1 - \frac 1 {1.1^{20}}) * 1.1

Steps
`````

1. Draw good timeline
2. Idenfity cash flow stream
3. Apply std formula
4. this gives PV exactly one period before first cash flow
5. adjust as necessary


Geometric Growth
----------------

- e.g. "g by 10% per year"

Growth Perpetuity 
`````````````````

C = 1st cash flow

.. math::

    \text{if } g < r \\ 
    \text{then } P = \frac C {r-g} \\
    \\
    \text{if } g > r \\
    \text{then P doesn't converge} \\


Growth Annuity
``````````````

.. math:: 

    PV = \frac C {r-g} * (1-(\frac {1+g} {1+r})^n)

    \text {as } n \rightarrow \infty , (\frac {1+g} {1+r})^n \rightarrow 0 , \text{ and } PV = \frac C {r-g}


Example: Retirement Savings Plan
````````````````````````````````

::

    r = 10% 
    Today birthday t=20
    Deposit starting one year
    last deposit on birthday t=65
    first withdrawl birthday t=66
    last withdrawl on t=85
    withdrawl to grow at 3%
    first withdrawl to be 100k
    how much must you deposit each year?

.. image:: _static/cash_flows.png

.. math::

    \text{Amount needed at t=65}    &= PV_{66 \leq t \leq 85} \\ 
                                    &= \frac {C_{First Withdrawl}} {r-g} * (1-(\frac {1+g} {1+r})^n) \\
                                    &= \frac {-100000} {0.1-0.03} * (1-(\frac {1.03} {1.1})^{20})

.. math::

    PV_{21 \leq t \leq 65}  &= - PV_{66 \leq t \leq 85} \\
                    &= - \frac {C_{deposit}} {0.1} * (1-(\frac {1} {1+0.1})^{45}) *(1+0.1)^{45} \\

.. math::

    C_{deposit} = \text{how much we must deposit each year}


Assignment Questions
--------------------

Question 8
``````````

.. image:: sometng

.. math::

    \text{eff q rate} = \frac {0.08} 4 = 0.02

.. math::

    \text{eff 1/2 rate} &= (1+0.02)^2 - 1 \\
                        &= 0.0404 

.. math::

    PV_\text{bank acc today t=0}    &= \frac {4000} {0.0404} * (1 - \frac 1 {1.0404^{10}} * (1 + 0.0404)^{11} \\
                                    &= 50057

.. math::

    PV_\text{bank acc today t=0} &= PV_\text{withdrawls from today} \\
    PV_\text{bank acc today t=0} &= PV_\text{withdrawls from today PT1} + PV_\text{withdrawls from today PT2} \\
    50057 &= [2C + \frac {2C} {0.035} * (1 - \frac 1 {1.035^5})] + [\frac C {0.035} * (1 - \frac 1 {1.035^6}) * \frac 1 {1.035^5}] 


Question 9
``````````

.. math:: 

    EAR = 10\%, EAR = e^q - 1 \\

.. math:: 

        0.1 &= e^q - 1 \\
        e^q &= 1.1 \\
        ln e ^ q &= ln 1.1 \\
        q &= ln 1.1 
        cont comp r = ln 1.1

.. math:: 

    eff m rate = (1+0.10)^{\frac 1 {12}} - 1

Question 3
``````````

.. math:: 

    Borrow $10000, r = 20\%
    Int = 2000/12000 \rightarrow $1000/month \text{in interest payments}

.. math::

    PV = 10000 = \frac {1000} r * (1 - \frac 1 {(1+r)^{12}})

    emr = (1 + EAR)^{1/12} - 1