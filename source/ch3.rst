Corporate Risk
==============


example
-------

==========  ==========
sell price  = 5
cost        = 3
----------- ----------
margin      = 2 or 40%
----------- ----------
FC          = 5000
==========  ==========

Sales
VC = Variable Costs
FC = Fixed Costs
-----------------
EBITDA (Breakeven)

- imagine two companies with same product, price point, etc.etc., except only that they have different cost structures

    - could amount to different risk
    - e.g. better machinery, less workers vs. worse machienery, more workers

        - machinery -> FC, workers -> VC

Degree Of Operating Leverage (DOL)
----------------------------------

.. math:: 

    DOL = Percent Change In EBITDA + Percent Change in Sales

.. admonition:: Derivation of DOL

    .. math::

        EBITDA &= Sales - VC - FC                           (1)

        if Sales \uparrow 1% then

        EBITDA*         &= 1.01 * Sales - 1.01 * VC - FC    (2)

        \delta EBITDA   &= 0.01 * Sales - 0.01 * VC         (2 - 1)

        % \delta EBITDA &= \frac {\delta EBITDA} {EBITDA} \\
                        &= \frac {0.01 * Sales - 0.01 * VC} {Sales - VC - FC}

        DOL &= \frac {\frac {0.01 Sales - 0.01 VC} {Sales - VC - FC}} {0.01} \\
            &= \frac {Sales - VC} {Sales - VC - FC}

.. math::

    S - VC = Units Sold * \frac {Contribution Margin (CM)} {Unit}
    DOL = \frac {\frac {CM} {Unit} * Unit Sales} {\frac {CM} {Unit} * Unit Sales - FC}

    also 

    S - VC = Sales * \frac {Contribution Margin (CM)} {$}
    DOL = \frac {\frac {CM} {$} * Sales} {\frac {CM} {$} * Sales - FC}


- when fixed costs are high, risk is high

    - when times are bad, FC owns you
    - when times are good, you get a lot of $$ b/c of low VC


=================== =================================================   ===============================================
\                   Capital Intensive                                   Labour Intensive
=================== =================================================   ===============================================
Sales               10,000                                              10,000
VC %                20%                                                 60%
VC                  2000                                                6000
FC                  6000                                                2000
\                   \                                                   \
EBITDA              2000                                                2000
\                   \                                                   \
Sales \uparrow 10%  11000                                               11000
VC                  2200                                                6600
FC                  6000                                                2000
\                   \                                                   \
EBITDA              2800                                                2400
DOL                 :math: \frac {0.8 * 1000} / {0.8*1000-6000} = 4     :math: \frac {0.4 * 1000} / {0.4*1000-2000} = 2
=================== =================================================   ===============================================

    A       B 
==  ====    ====
D   4000    6000
E   6000    4000
\   \       \
    10000   10000

:math:r_d = 10%

=========   =====   =====   =====   =====
            A       A'      B       B'
=========   =====   =====   =====   =====
EBIT        2000    2400    2000    2400
Int         400     400     600     600
\           \       \       \       \
EBT         1600    2000    1400    1800
Tax @ 40%   840     800     560     720
\           \       \       \       \
NI          960     1200    840     1080
---------   -----   -----   -----   -----
ROE         0.16    0.2     0.21    0.27
=========   =====   =====   =====   =====
