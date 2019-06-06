Corporate Financial Planning
============================

Example Problem
---------------

::

    FL      monthly Sales       60000
    Nov     dues paid           20000
    Dec     tax payment         65000
    Sep 30  Cash Balance        221000
    Sep 30  Short Term DOL      0
    P M     Cash Bal Allowed    100000

    Borrow Short Debt --------------^             
    Cash is less than

    Pay Ang Short Debt 
    if cash is above    -------------^

    Oct Cap example             340000
    Int Paid on Short DOL       1 + 1/3% / month

    Int Received on Cash        1%/month
    Sept 30 LTD                 400000
    Interest on LTD             1% / month

    Monthly repayment on LTD    5738.84 / month


    COGS                        65% of sales
    Purchase goods              1 month before sale
    Assume depreciation == CCA
    Dep Rate                    3% per quater
    % of sales as cash          20%
    Cr sales                    collected after 1 month
    AP period                   2 months
    Sep 30 NFA                  250000
    Sep 30 Taxes payable        100000
    Miscellaneous accrurals     20000
    (not expected to change)
    Tax Rate                    33%
    Jan Sales Prediction        153,846


    Today is Sep 30

                Sales
    Aug         140000
    Sep         200000
    --------------------
    Oct         200000
    Nov         300000
    Dec         400000


Principal Repayment Projection
``````````````````````````````

Principal Payment = Montly Repayment - Interest Accumulated for Month

:: 

            Start Debt  Int         Principal Payment   End Debt
    Oct     400,000     4000        1738.84             398,261.16
    Nov     398,261.16  3982.61     1756.23             396,504.93
    Dec     396,505     3965        1774                394731      (rounded to nearest dollar)

    Q1 (jan-mar)        11788       5429                  
    Q2 (apr-jun)        11624       5593                  
    Q3 (jul-sep)        11454       55962               idk                   
    Q4 (jul-sep)        11279       idk                 idk

Cash Projection
```````````````

:: 

                    Aug     Sep     | Oct       Nov         Dec         Jan (forecasted)
    Sales           140,000 200,000 | 200,000   300,000     400,000     153,846   
    Cash Sales*     280,000 400,00  | 40,000    60,000      80,000  
    Cr Sales        112,000 160,000 | 160,000   240,000     320,000
    Collections*            112,000 | 160,000   160,000     240,000
    Purchases       130,000 130,000 | 195,000   260,000     100,000
    Payments*                       |-130,000  -130,000    -195,000
    Wages (unrelated to manufact)*  |-60,000   -60,000     -60,000
    CAPEX*                          |-340,000
    Dividends*                      |          -20,000
    Taxes*                          |                      -65,000
    Interest Received on Cash       | 2100  
    Int Paid STD                    | 0                 
    Int Paid LTD                    |-4000     -3983.23
    Princ LTD                       |-1738.84  -
    \               \       \       | \         \           \
    :math:`\delta` Cash*            |-333,529   2427        -7549
    Cash Balance Start              | 221,000   100,000     100,000
    Cash Before Bef Borrow          |-112,529   102,427     92,480
    ST Borrowing                    | 212,529   -2427       7840
    End Cash                221,000 | 100,000   100,000     100,000
    ST Debt                         | 212,529   210,101     217,642

- \delta Cash is the sum of all of the Cash* flow stuff

* : this is a cash flow

- left some historical stuff blank because we didn't need them for projections
- wages 

Income Statement
````````````````

=========   =====================   =====================================
            1st 9 Months to Sep30   3 Months to Dec 31
=========================================================================
\           \                       \
Revenue     2,000,000*              900,000
COGS        1,300,000               585,000 = Purchases for Sep, Oct, Nov
Other       540,000                 180,000
\           \                       \
EBITDA      160,000                 135,000
Dep         30,000*                 17,700
\           \                       \
EBIT        130,000                 17,300
Interest    30,000*                 13,373
\           \                       \
EBT         100,000                 103,927
Taxes       33,000                  34,296
\           \                       \
NetInc      67,000                  69,631
=========   =====================   =====================================


Total NFA = Initial NFA + added NFA = 250,000 + 340,000 = 590,000
Dep = 0.03 * Total NFA = 0.03 * 590,000 = 17,700

* : given

=========   ==========  ==========  =============   ==========  ========
\           Sep 30      Dec 31      \               Sep 30      Dec 31
========================================================================
Cash        220000      100000      AP              260,000     360,000
AR          160000      320000      STD             0           217642
Inv         600000*     570000      Curr LTD        22053       22721
                                    Tax Payable     100000      
                                    Misc Accruals   20000       20000
                                    
                                    LTD             377947      372010
NFA         250000      572300      Equity          451000      1562300
\           \           \                           \           \
            1123000     1562300                     1231000     1562300
=========   ==========  ==========  =============   ==========  ========

Inv_Dec31   &= Purchases_Oct + Purchases_Nov + Purchase_Dec ??
            &= 600,000 + 555000 - 585000
            &= 570000

NFA_Dec31   &= 250000 + 340000 - 17700
            &= 572300

AP_Sep30    = Purchases Over the last 60 days
            = Purchase_Aug + Purchase_Sep

CurrLTD_Sep30   &= Principal Payments for the previous 12 months
                &= Princ_Oct + Princ_Nov + Princ_Dec + Princ_Q1 + Princ_Q2 + Princ_Q3

CurrLTD_Dec31   &= Princ_Q1 + Princ_Q2 + Princ_Q3 + Princ_Q4

TaxPayable_Dec31    &= TaxPayable_Sep30 - TaxPayment_Dec30 + Taxes Accrued Last Year
                    &= 100000 - 65000 + 34296

Equity_Sep30 = Sep30 - All other stuff

Equity_Dec31    = Sep30 - All other stuff 
                = 451000 + RE 
                = 451000 + (Net Income - Dividends)
                = 451000 + (Net Income - 20000)
                = 1562300


- what this type of analysis allows you to do

    - if you're noticing you're going to be cash tight given an expansion
        
        - ease up opposing sides of the balance sheet
        - convert to cash

    - examples:

        - you can talk to suppliers and ask them to give you breathing room given your expansion (and increase in purchase of their product)
        - offer collateral to... somewhere?
        - offer discount for paying by cash to increase liquidity
        - sell AR (factoring) (convert AR to CASH)
        - run inventory down: buy less inventory, burn through your current inventory
        - go to tax man and say "can we delay payment"
        - cut the dividend
        - 


* : given

New Example
-----------

- Pay 40 days later

                Sep     Oct     Nov     Dec
Sales                   100000  200000  300000
COGS @ 50%      50000   100000  150000


.. image:: weird_payment_graph

.. math:: 
    
    Payments in November    &= Purchases Made in September to be paid in November + Purchases Made in October to be paid in November
                            &= Purchases from Sep20 to Sep30 + Purchases from Oct1 to Oct20
                            &= Purchases for 10 days in September + Purchase for 20 days in October
                            &= PP_S + PP_O
                            &= 10/30*50 + 20/30*100

    Purchase Portion    &= PP
                        &= Days Accounted For/Total Days In Month * Purchases For Month

    - assuming 30 days/month

