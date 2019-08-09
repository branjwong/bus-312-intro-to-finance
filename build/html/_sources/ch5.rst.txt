Ch 5: Taxation and Investment Returns
=====================================

Capital Gains
-------------

.. math:: Taxable Income = \frac {Taxes} {Net Income}

- capital gain occurs when you sell an asset for more than it costs
- capital loss only occurs if you sold a non-depreciable asset for less than it cost.

- capital gains inclusion rate: 50%

    - better to have cash coming in as capital gain vs. say interest b/c capital gains are taxed less
    - 50% is the number that's currently used as per current tax regulations


1. Determine net gapital gain
2. If Positive, add 50% to taxable Income
3. If negative, can go back 3 years to write off 

    - if you paid capital gains tax within 3 years before, you can get a tax refund against your current year's capital loss

4. If still negative, can carry fowards indefinitely

Example: Calculating Tax against Capital Gain
``````````````````````````````````````````````

============    =====   =============== =============== ====    ====    =====   ====    ================    ====    ====    ====
Yr              1       :math:`1^{yr3}` :math:`1^{yr3}` 2       3       4       4'      :math:`1^{yr13}`    ...     13      13'
============    =====   =============== =============== ====    ====    =====   ====    ================    ====    ====    ====
Net Cap Gain    1000    400             0                       -600    -1000   -600    0                           2000    1400
EBT             500     200                                                                                                 700
Tax 40%         200     80                                      -120            -80                                         280
============    =====   =============== =============== ====    ====    =====   ====    ================    ====    ====    ====

.. math::

    EBT = Net Cap Gain * Capital Gains Inclusion Rate \\
    \\
    where, \\
    \\ 
    x_y = \text{Recalculation Of Year X After Year Y} \\
    x' = \text{Recalculation Of Year X After Recalculation Of Some Previous Year}

The Capital Cost Allownace System
---------------------------------

- expenditures that firms make on fixed assets are not expensable for financial statement purposes or deductable for tax purposes

    - e.g. plant, equipment

- these expenditures are amortized over time
- in financial statements, the amortized amount in a period is called depreciation
- in taxation, the government of Canada allows a capital cost allowance instead of depreciation

    - this is to avoid the adverse incentive for firms to exaggerate financial statement depreciation to reduce their taxes

- **capital cost allownace (CCA)**, an allowance given by the government of Canada to a firm for expensing and receiving a tax break on fixed assets

    - CCA reduces taxable income

- there isn't a definition of depreciable assets in the Income Tax Act, but assets that are subject to CCA are typically what you'd think of as depreciable

.. admonition:: CCA Asset Classes

    .. image:: _static/cca_asset_classes.png

    - CCA is not taken on individual assets but on prescribed classes of similar assets
    - when a taxpayer has several assets in a class, they are treated as a unit with respect to the calculation of CCA
    - **undepreciated capital cost (UCC)** of an asset class is the declining balance of that asset class
    
        - the maximum CCA that may be claimed in a year calculated on the UCC


.. admonition:: Calculating CCA and UCC's Ending Balance

    .. warning:: CCA and UCC are calculated on a per-asset class basis. Don't mix up cashflows, CCAs, and UCCs from different asset classes.

    let...

    .. math:: 

        UCC_i &= \text{Opening Balance UCC}  \\
        CF_x &= \text{CCA Asset cashflow (acquisition or disposal) x} \\
        \Sigma CF &= \text{net additions} \\
        rate_{CCA} &= \text{CCA Rate} \\
        UCC_f &= \text{Ending Balance UCC} 

    such that...

    .. math::

        \Sigma CF = CF_1 + CF_2 + CF_3 + ... + CF_n 

    .. math::
        :nowrap:

        \[ \text{multiplication factor}_{CCA} = 
        \begin{cases} 
            UCC_i + \frac 1 2 * {\Sigma CF}, \Sigma CF > 0 \\
            UCC_i + \Sigma CF, \Sigma CF < 0 
        \end{cases}
        \]

    .. math::

        CCA = rate_{CCA} * \text{multiplication factor}_{CCA}

    .. math::

        UCC_f = UCC_i + \Sigma CF - CCA


Example: UCC Over Time
``````````````````````

:: 

    Starting UCC = 4000
    CCA rate = 50%

    Yr 1:

    - buy an asset for 800
    - and sell another for 500 (original cost = 900)

    Yr 2: nothing

    Yr 3: 

    - buy an asset for 400
    - and sell another for 800 (original cost = 500)

    Yr 4: nothing

======  =========   ==============  ==========  ===========
Year    Start UCC   Net additions   CCA         End UCC
======  =========   ==============  ==========  ===========
1       4000        300 (a)         2075 (b)    2225 (c)
2       2225        0               1112.5 (d)  1112.5 (e)
3       1112.5      -100 (f)        506.25 (g)  506.25 (h)
4       506.25      0               253.12      253.12
======  =========   ==============  ==========  ===========

.. math:: 

    (a) &= 800 - 500 \\
        &= 300

.. math:: 

    (b) &= (HalfYearRule * 3000 + 4000) * Rate_{CCA} \\
        &= (0.5 * 3000 + 4000) * 0.5
    
.. math:: 

    (c) &= 4300-2075 \\
        &= 2225 

.. math:: 

    (d) &= CCA rate * UCC \\
        &= 0.5 * 2225 \\
        &= 11125

.. math:: 

    (e) UCC_{end}   &= UCC_{start} - CCA \\
                    &= 1112.5

.. math:: 

    (f) Net Add &= 400 - 500 \\
                &= -100

.. math:: 

    (g) CCA &= Rate_{CCA} * (1112.5 - 100) \\
            &= 506.25

.. math:: 

    (h) UCC_{end}   = UCC_{start} - CCA \\
                    = (1112.5 - 100) - 506.25 \\
                    = 506.25

Example: Terminal Loss vs CCA Recapture
```````````````````````````````````````

Buy a vehicle for 80000

    :math:`\Sigma CCA = 50000`

=============   ==========  =============   ==========
\               Scenario 1  \               Scenario 2
=============   ==========  =============   ==========
UCC =           30000       \               \
Sell for        20000                       40000
\               \           \               \
\               10000       \               -10000
Terminal Loss   10000       CCA Recapture   10000
\               \           \               \
\               0           \               0
=============   ==========  =============   ==========

Loss of value = 80000-20000=60000

- **Terminal loss**, can be thought of extra CCA

    - only occurs if balance is positive and the last asset is sold

- **CCA Recapture**, "we, the CRA, gave you too much CCA in past and now we're reclaiming taxable income"

    - only whenever the balance goes negative


Example: Taxable Income Sources
```````````````````````````````

::

    Salary                  Directly
    +- Alimony              Directly
    - RRSP contribution     Directly
    + Interest received     Directly
    + Capital gains         * 0.5
    + Canadian Divs         Gross up by 40% (increase?)
    + Non Canadian Divs     Directly

    Salary                      60000
    Interest                    20000
    Capital gain    60000 ->    30000
    Can Divs        10000 ->    14000
    Non Can Divs                40000
                                -------
    Taxable Income              110000
    Net Federal Tax (b)         18100
    Net Provincial Tax (given)  17000
                                -------
    Net Income                  74900


(a)

:: 

    Fed Tax
    0 - 40000   15%     6000
    40k-80000   22%     8800
    80k-120k    26%     7800
    > 120k      29%
                        -----
    Tax paid            22600


(b)

:: 

    Basic Fed Tax               22600 (a)
    Basic Personal Tax Cr       -1500 (given)
    Div Tax Cr (30% of div)     -3000
                                -------
    Net Federal Tax             18100


Assignment 4, Question 3
------------------------


Asset Class X 
``````````````

::

    UCC =               32000
    Capital Loss (?)    -45000
                        ------
                        -13000

    CCA recapture       13000
        is added to earnings

Asset Class Y
``````````````
::

    Suppose
    Asset Bought for    20000
    Sold for            50000

    Therefore
    Capital Gain        30000   (add 15% to earnings b/c inclusion rate)
    UCC Loss of         -20000


    UCC             67000
                    -20000
                    -------
                    470000
    Terminal Loss   470000


Asset Class Z
``````````````

UCC         150000

Old Asset is Sold Off

.. math::

    Z   &= net additions \\
        &= 80000 - 25000 \\
        &= 55000

.. math::

    CCA = 0.4 * (150000 + 0.5 * 55000)

is subtracted from earnings




