Taxation and Investment Returns
===============================

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

============    =====   =============== =============== ====    ====    =====   ====    ================    ====    ====    ====
Yr              1       :math:`1^{yr3}` :math:`1^{yr3}` 2       3       4       4'      :math:`1^{yr13}`    ...     13      13'
============    =====   =============== =============== ====    ====    =====   ====    ================    ====    ====    ====
Net Cap Gain    1000    400             0                       -600    -1000   -600    0                           2000    1400
EBT             500     200                                                                                                 700
Tax 40%         200     80                                      -120            -80                                         280
============    =====   =============== =============== ====    ====    =====   ====    ================    ====    ====    ====


    - EBT = Nat Cap Gain * Capital Gains Inclusion Rate
    - x_y = recalculation of year x after year y
    - x' = recalculation of year x after recalculation of some previous year

CCA
---

1. Calculate net additions

    - :math:`Acquisiton - Disposals`

        - acq: valued at cost
        - disp: losses of cost and selling price

2. If positive, add CCA = half of net additions to UCC and calc CCA

    - UCC: Undepreciated Capital Cost

3. If negative, add the (neg) number to UCC and calculate CCA


Example
```````

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

Year    Start UCC   Net additions   CCA         End UCC
1       4000        300 (a)         2075 (b)    2225 (c)
2       2225        0               1112.5 (d)  1112.5 (e)
3       1112.5      -100 (f)        506.25 (g)  506.25 (h)
4       506.25      0               253.12      253.12

(a) &= 800-500=300
(b) &= (1/2 year rule * 3000 + 4000) * CCA rate
    &= (0.5*3000+4000)*0.5
    
(c) &= 4300-2075 = 2225 
(d) &= CCA rate * UCC
    &= 0.5 * 2225 = 11125

(e) UCC_{end} = UCC_{start} - CCA
    = 1112.5

(f) Net Add = 400 - 500 = -100
(g) CCA = CCA rate * (1112.5 - 100) = 506.25

(h) UCC_{end}   = UCC_{start} - CCA
                = (1112.5 - 100) - 506.25
                = 506.25

Another Example
---------------

Buy a vehicle for 80000
        :math:`\net CCA = 50000`


                Scenario 1              Scenario 2
                -----                   ------
UCC =           30000   
Sell for        20000                   40000
                -----                   ------
                10000                   -10000
Terminal Loss   10000   CCA Recapture   10000
                -----                   ------
                0                       0

Loss of value = 80000-20000=60000

Terminal loss ~ (can be thought of extra CCA)

    - only occurs if balance is positive and the last asset is sold

CCA Recapture ~ "we, the CRA, gave you too much CCA in past and now we're reclaiming taxable income"

    - only whenever the balance goes negative


Another Example
---------------

- some examples of taxable income

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
Fed Tax
0 - 40000   15%     6000
40k-80000   22%     8800
80k-120k    26%     7800
> 120k      29%
                    -----
Tax paid            22600


(b)
Basic Fed Tax               22600 (a)
Basic Personal Tax Cr       -1500 (given)
Div Tax Cr (30% of div)     -3000
                            -------
Net Federal Tax             18100


