Ch 2: Financial Analysis with Financial Statements
==================================================

- not a course about accounting
- more about getting information out of financial statements

    - balance sheet
    - income statement

        - a record describing the business operations of the company over a period of time
        - revenue/sales: money that comes in from business activities
        - expenses

            - multiple categories, e.g. cost of goods sold

        - :math:`Gross Profit = Revenue - Expenses`
        - other expenses
        - .. math:: 

            EBITDA  = Earnings Before Interest, Taxation, Depreciation (DA) \\
                    = Gross Profit - Other Expenses

        - depreciation (a non-cash item)
        - :math:`EBIT = EBITDA - depreciation`
        - interest
        - :math:`EBI = EBIT - interest`
        - tax
        - :math:`net profit = EBI - tax = earnings after tax = post tax earnings`

            - distributed amongst shareholders in terms of 

                - dividends: funds paid directly
                - retained earnings: reinvestment into company on behalf of shareholders

        - problem: company determining depreciation determines taxes

            - CRA doesn't like that
            - **capital cost allowance (CCA)**, allowance CRA gives on the capital cost of an item
            - depreciation shields you from paying taxes

Income Statement Example
------------------------

=================== =================== ===============
Statement Item      Company Accountants CRA Accountants
=================== =================== ===============
Revenue             2000
Cost of Goods Sold  800
\                   \                   \
**Gross Profit**    1200
Other Expenses      500
\                   \                   \
**EBITDA**          700
Depreciation        200                 400
\                   \                   \
**EBIT**            500                 300
Interest            100                 100
\                   \                   \
**EBI**             400                 200
Tax                 160                 80
\                   \                   \
**Net Profit**      240                 120
=================== =================== ===============

What the public is shown

=========== === === === ===
Year        1   2   3   4
=========== === === === ===
EITBA       500 500 500 500
Dep         200 200 200 200
\           \   \   \   \
EIT         250 250 250 250
Tax @40%    100 100 100 100
\           \   \   \   \
Net Profit  150 150 150 150
=========== === === === ===

What is used for tax purposes

=============== === === === ===
Year            1   2   3   4
=============== === === === ===
EITBA           500 500 500 500
CCA             400 300 200 100
\               \   \   \   \
EIT             100 200 300 400
Tax @40%        40  80  120 180
\               \   \   \   \
Net Profit      60  120 180 240
=============== === === === ===

Money In Account Over Time

=============== === === === ===
Year            1   2   3   4
=============== === === === ===
Deferred Tax    60  80  60  0       
=============== === === === ===

Profitability Ratios
--------------------

- comparing to other companies (of different sizes) when making decisions about investments

    - how much of our profit company keeps (?)
    - how well are we controlling our costs
    - track performance over time
        
        - are ratios changing for good reasons? bad reasons?
        - what is the correct ratio? 
            
            - industry average?

    - how to compare across national borders?
        
        - depreciation, taxation rules, etc.
        - accounting practices
        - flexibility in expensing items

    - looking at ratio in conjunction with the reasons for that ratio's determination
    

.. math::

    Net Profit Margin   &= \frac {Net Profit} {Revenue} \\
                        &= \frac {240} {2000} \\
                        &= 0.12
        
    \newline
        
    Gross Profit Margin &= \frac {Gross Profit} {Revenue} \\
                        &= \frac {1200} {2000} \\
                        &= 0.60

    \newline

    EBITDA Margin   &= \frac {EBITDA} {Revenue} \\
                    &= \frac {700} {2000} \\
                    &= 0.35


Balance Sheet Comparison
------------------------

- income statement covers what's happen over a period of time
    
    - e.g. month, quarter, year

- balance sheet is a snapshot of an instant in time

====    ====    =========================   ====
Counting Balance Sheet
================================================
*Assets*        *Liabilities*
------------    --------------------------------
\       \       \                           \
Cash    100     AP                          160
AR      300     Short debt                  200
Inv     250     Current portion long debt   200
\    
\       \       Long debt                   1600
NF      3500    Equity                      1850
\       \       \                           \
\       4050    \                           4050
====    ====    =========================   ====


- split up into four sections

    - current assets/liabilities vs long-term assets/liabilities

- current assets: cash, ar, inv converted into cash in less than a year
- net-fix assets: not converted in less than a year
- balance sheet in order of liquidity

============    ====
Fixed assets    4000
Depreciation    600
\               \
\               3400
============    ====

=============== ====
Total Long Debt 1800
Current portion 200
\               \
\               1600
=============== ====

.. Common Stock    1500
.. Something       380


Operation Side

    - usually left hand side of balance sheet

Finance Side

    - deals with financial aspects
    - deals with people who supply of capital
    - e.g. issuing of shares
    - usually right hand side of balance sheet

        - wouldn't include AP

=============   ====    =========================   ====
Invested Capital Balance Sheet
========================================================
Operational Side        Financial Side
--------------------    --------------------------------
\               \       \                           \
Cash            100     Short debt                  200
AR              300     Current portion long debt   200
AP              -160    \                           \
Inv             250     \                           \         
\               \       Long debt                   1600
NF              3500    Equity                      1850
\               \       \                           \
Total Capital   3890    Invested Capital (IC)       3890
=============   ====    =========================   ====

- split up into four sections

    - trade capital/netfixed assets (capital expenditures)

        - trade capital = cash + AR - AP + NF
        
    - debt/equity

- answers the question: how is the money that is being **invested** into the company being **used**?
- three ways to increase investment

    - increase retained earnings, increase equity
    - borrow money, increase debt
    - issue more shares, increase equity

- can't expand your business (left hand side) if you don't expand investment (right hand side)

    - you'll run out of cash if you don't
    - running out of cash means you can can't pay suppliers, and then your business goes under when they don't supply you


Return Ratios
-------------

- net profit goes to equity holders
- interest goes to debt holders

Return on Invested Capital
``````````````````````````

.. math:: 

    ROIC    &= \frac {EBITDA} {IC} \\
            &= \frac {700} {3890}

    ROIC After Dep  &= \frac {EBIT} {IC} \\
                    &= \frac {500} {3890}

    ROIC After Dep And Tax  &= \frac {EBIT*(1 - \tau)} {IC} \\
                            &= \frac {500*(1-0.4)} {3890} \\
                            &= \frac {300} {3890}

- :math:`\tau` is the symbol used for tax rate
- both debt holders and interest rate are going to lose money on tax
- if tax rate differs between receivers, then change the formula for them
- ROIC being before/after depreciation and taxes can be vague

    - i.e. ROIC, ROIC before tax, ROIC before depreciation and taxes 
    - prof will be clear what he wants

Return on Equity
````````````````

.. math::

    ROE &= \frac {Net Income} {Equity} \\
        &= \frac {240} {1890}


Return on Equity (Du Pont Expansion)
------------------------------------

.. math::

    ROE \\
    &= \frac {Net Income} {Equity} \\
    &= \frac {Net Income} {Revenue} * \frac {Revenue} {Total Assets} * \frac {Total Assets} {Equity} \\
    &= Profit Margin * Asset Turnover * Capital Structure Measure


Return on Debt/Rate of Debt
```````````````````````````

- the average interest rate the company pays

.. math::

    r_d &= \frac {Interest} {Debt} \\
        &= \frac {100} {2000} 

Miscellaneous Ratios
--------------------

- **Capital Structure**, how the investment into the firm is made up
- the ratio of debt to equity is important
    
    - affects risk
    - debt + downturn in economy => increased risk of going bust

Debt to Invested Capital
````````````````````````

.. math::

    Debt : IC   &= \frac {Debt} {Invested Capital} \\
                &= \frac {2000} {3890} \\
                &> 0.51

Liquidity Measures
------------------

Current Ratio
`````````````

.. math:: 

    Current Ratio   &= \frac {Current Assets} {Current Liabilities} \\
                    &= \frac {650} {560} \\
                    &= 1.16 \\
                    &> 1

- this co. is reasonably flush with money
- a supermarket might have a super low current ratio while still being safe, due to the nature of the company
- suppose company that sells high end fashion clothing

    - current inventory (1-2 weeks old e.g.) could be worth a lot
    - non-current inventory (>5 weeks old e.g.) could be worth nothing

Quick Ratio/Acid Test Ratio
```````````````````````````

.. math::

    Quick Ratio &= \frac {Current Assets - Inventory} {Current Liabilities} \\
                &= \frac {400} {550} \\
                &= 0.71

Cash Ratio
``````````

.. math::

    Cash Ratio  &= \frac {Cash} {Current Liabilities} \\
                &= \frac {100} {560}

Times Interest Earned
`````````````````````

.. math:: 

    Times Interest Earned   &= \frac {EBIT} {Interest} \\
                            &= \frac {500} {100} \\
                            &= 5

- they can pay off the interest easy
- enough EBIT to cover interest

Fixed Payment Coverage
``````````````````````

- how well they are able to pay off the interest **and** the principal

- :math:`Fixed Payment Coverage \neq \frac {EBIT} {Interest + Capital Repayment}`

    - principal is not tax deductable, interest is
    - $1 of EBIT cannot pay $1 principal, but can pay $1 interest, given taxation

    - before you pay principal, tax man takes tax

.. math::

    Fixed Payment Coverage  &= \frac {EBIT} { Interest + \frac {Capital Repayment} {1-\tau} } \\
                            &= \frac {500} { 100 + \frac {200} {1-0.4} } \\
                            &= 1.15

- if :math:`\tau = 0.4`, $1.66 of EBIT will pay $1 principal


Turnover Figures
----------------

- all turnover figures have either COGS or Revenue in the numerator


Invested Capital
````````````````

.. math::

    IC Turnover &= \frac {Revenue} {Invested Capital} \\
                &= \frac {2000} {3890} \\
                &= 0.51

- the higher the better
- the ratio indicates how much a company could grow its current capital investment level
- low capital turnover generally corresponds to high profit margins

Asset
`````

.. math::

    Asset Turnover &= \frac {Revenue} {Assets} \\

- measures the efficiency of a company's use of its assets in generating sales revenue or sales income to the company
- low profit margins tend to have high asset turnover
- high profit margins have low asset turnover


Inventory
`````````

.. math::

    Inventory Turnover  &= \frac {COGS} {Inventory} \\
                        &= \frac {800} {250} \\
                        &= 3.2

- you're turning over inventory 3.2 times through the year
- 3.2 times through the year or inventory coming in, sitting, being sold, and then having to buy more
- this would be a really bad turnover for a supermarket
- might be acceptable to a jewelery store


.. math:: 

    Inventory Period    &= \frac {Days In A Year} {Inventory Turnover} \\
                        &= \frac {365} {3.2} \\
                        &= 114

- inventory sits on shelf for 114 days

Accounts Receivable
```````````````````

.. math::

    AR Turnover &= \frac {Revenue} {AR} \\
                &= \frac {2000} {300} \\
                &= 6.67 

.. math::

    AR Period   &= \frac {Days In A Year} {AR Turnover} \\
                &= \frac {365} {6.67} \\
                &= 54.75

- taking 54.75 days on average to collect cash from customers who purpose on credit

Accounts Payable
````````````````
.. math::

    AP Turnover = \frac {COGS} {AP}

.. math::

    AP Period = \frac {Days In A Year} {AP Turnover}

Activity Graph
``````````````
:: 

    day activity 
    === ========
    0   buy item        | Inventory Period          | AP Period      
    10  sell item       |                           |               
    15  pay for item                | AR Period     |
    40  collect cash from sale      |                               | Cash Conversion Cycle

.. math::

        Inventory Period + AR Period                &= AP Period + Cash Conversion Cycle \\
    =>  Inventory Period + AR Period - AP Period    &= Cash Conversion Cycle

- if AP Period is very long, this can be negative

Capital Structure Measure
`````````````````````````

.. math:: Capital Structure Measure = \frac {Total Assets} {Equity}

- if Equity makes up your entire assets, (thus you have no debt), then :math:`Capital Structure Measure == 1`
- greater the debt you have, the greater your ROE

    - but becomes riskier, as losses become more magnified

Which Equity Figure to use in ROE?
``````````````````````````````````

::

                Income Statement
      |-------------------------------------|
    BS_1                                  BS_2


- usually beginning of period (BOP) is used

.. math::

    ROE = \frac{Net Income}{Eq_{BOP}}

- question: does cash flow (properly) through the business?

:: 

    operational definition                  financial definition
    of free cash flow                       of free cash flow

    sales                   -->             <-- shared issue
    investment in NF assets -->             <-- borrow
    COGS                    <-- [QA]---[FA] --> money going out
                                            --> paying interest
    salvage machine         -->             --> share repurchase
                                            --> paying dividends



Definitions of Free Cash Flow
-----------------------------

Operational Definition
``````````````````````

.. math:: 

    Free Cash Flow = FFO (Funds From Operations) - Investment In TC - Investment In NFA

Financial Definition
````````````````````

.. math::

    Free Cash Flow = Equity + Debt              (1 + 2) \\
    where: \\
    Equity = Dividiends + Net Share Operations  (1) \\
    Debt = Interest + Net Debt Repayment        (2) 

==========  ====
Income Statement
================
Sales       4000
COGS        2800
Other       600
\           \
EBITDA      600
Dep         100
\           \
EBIT        500
Interest    200
\           \
EBT         300
Tax @ 0.40  120
\           \
\           180
==========  ====

.. math::
    :nowrap:
    
    \begin{gather}
        Dividends \rightarrow 80 \\
        Retained Earnings \rightarrow 100
    \end{gather}


====    ====    ====    ====    ====    ====
Balance Sheet
============================================
*Assets*                *Liabilities*
--------------------    --------------------
\       BEG     END     \       BEG     END
\       \       \       \       \       \
Cash    100     150     AP      300     400
AR      200     250     CPLD    200     200
Inv     400     300     \       \       \
\       \       \       LD      2500    2200
NF      5500    5800    EQ      3000    3700
\       \       \       \       \       \
\       6000    6500    \       6000    6500
====    ====    ====    ====    ====    ====

==========  ==========  =========
\           Operations  Financial
==========  ==========  =========
Sales       4000        \
COGS        2700        \
Other       600         \
\           \           \
\           600         \
Dep         100         \
\           \           \
\           500         0
\           \           \
Interest    --          -200
\           \           \
\           500         -200
Tax         200         -80
\           \           \
Net Income  300         -120
==========  ==========  =========

- these two sides adds up to the original income statement

.. math::

    FCF = FFO - Investment In TC - Investment In NFA \\
        = 600-200 \\
        = 400

=================== ====
Sales               1000
Recieved            900
\                   \
AR :math:`\uparrow` 100
=================== ====


.. math:: 

    Ending TC   &= 150 + 250 + 300 - 300 \\
                &= 300

    Start TC    &= 100 + 200 + 400 - 300 \\
                &= 400

    Investment In TC    &= 300 - 400 \\
                        &= -100

    Ending NFA = 5800 \\
    Start NFA = 5500 \\
    Investment In NFA = 5800 - 5500 = 300

    FCF &= FFO - Investment TC - Investment In NFA \\
        &= 400 - (-100) - 600 \\
        &= -100
