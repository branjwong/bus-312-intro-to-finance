Ch 8: Equity Securities and Equity Markets
==========================================

- *incorporation* creates a corporation with **common shares** and possibly **preferred shares** as its first financial assets

    - allows corporation to enter into legal agreements required for sale of other financial assets (e.g. debt)
    - shares give you a say in the management of a company
    - value of a share is the present value of the future cash flows
    - also non-voting shares: so the share issuer can maintain control of a company


Equity
------

- if you own a share, you are a shareholder
- limited liability for share ownership

    - shareholders cannot be held responsible (for the most part) for any liability, act, or default of the corporation

- shareholder classes, e.g. common shareholders, preferred shareholders

    - a firm cannot pay a dividend to a shareholder without paying the same dividend to all shareholders of that class



Dividends
---------

- corporations pay out dividends to shareholders 
- represents the only direct payment between a firm and its shareholders
- at a regular meeting, the board of directors decides whether to pay dividends on a share-class and the dividen amount
    
    - usually meetings happen quartlerly, but always at least yearly

- board of directors can cut or eliminate common and/or preferred share dividends

    - equity holders cannot sue the firm because a corporation does not contractually guarnatee dividends
    - debt is a financial asset that makes contractually promised payments

- how to value shares? what are those cash flows going to look like?

    - valuation is far less certain than bonds
    - dividends are discretionary, they may or may not be paid out
        
        - companies don't like sending negative signals to the market, and not paying dividends is a negative signal
        - paying a dividend despite a bad year signals that the company is assured in that the bad performance is temporary
        - being conservative about paying dividends allows companys to pay dividends despite bad years

Preference Share
----------------

- also called a preferred share
- has a fixed dividend
- preferred shareholders are paid out dividends before common share holder
- preferred shareholders get paid off first if the company folds and the assets are liquidated
    
    - order of pay

        - liquidators, lawyers
        - gov't
        - employees
        - debt holders
        - preferred shareholders
        - common shareholders

- often do not have voting power


Equity Valuation
----------------

- equity promises dividends if and when declared by the board
- the only thing a shareholder receives from a firm is dividends
- the ultimate source of share valud is dividend paying potential
- even if a corporation is not currently paying dividends, common shares will still have value because of future dividend potential

Example - Price Of a Share as Dividends are Paid
''''''''''''''''''''''''''''''''''''''''''''''''

:: 

    Div = 2
    r = 0.1
    g = 0.05

Initial valuation of a share:

.. math::

    Pr_{t=0}    &= \frac {Div_0} {r - g} \\
                &= \frac {2} {0.1 - 0.05} \\
                &= 40

Valuation of a share right before a dividend has been paid:

.. math:: 

    Pr_{t=1-}   &= \frac {Div_0} {r - g} * (1 + r)^1\\
                &= \frac {2} {0.1 - 0.05} * (1 + 0.1) \\
                &= 44


Valuation of a share right after a dividend has been paid:

.. math::

    Pr_{t=1+}   &= \frac  {Div_1} {r - g} 
                &= \frac  {Div_0 * g} {r - g} 
                &= \frac {2 * 1.05} {0.1 - 0.05} \\
                &= 42


Market Capitalization Rate
--------------------------

- **market capitalization rate**, the opportunity cost rate of return for common share evaluation

    - also known as the dividend yield?


Cash Cow
````````

.. image:: _static/straight_line.png
   :scale: 50 %
   :align: center

.. math::

    Pr = \frac {Div} r

Constant Growth
```````````````

.. image:: _static/constant_growth.png
   :scale: 50 %
   :align: center

.. math::

    Pr = \frac {Div} {r - g}

Dividend Yield
``````````````

- **dividend yield**, the ratio of a company's annual dividend compared to its share price

    let...

    .. math::

        dy = \text{dividend yield}

    such that..
    
    .. math:: 

        dy = \frac {Div} {Pr}

    so for a dividend with constant growth:

    .. math:: 

        dy &= \frac {Div} {Pr} \\
        Pr &= \frac {Div} {dy} \\
        Pr &= \frac {Div} {r - g} \\
        dy &= r - g
    

Earnings, Dividends, and Growth
-------------------------------

- **retention ratio**, the ratio of earnings that is retained within the company instead of being paid out as dividends

    - This number means that for every dollar of earnings available for distribution to shareholders, the firm distributes 100*(1-b) cents as a dividend to shareholders and retains 100*b cents for business reinvestment and growth.

    let...

    .. math:

        b = \text{retention ratio}
        E = \text{earnings per share}
        D = \text{dividends per share}

    such that..

    .. math: 
        
        b = \frac {E - D} {E}

    also...

    .. math::

        \text{payout ratio} = 1 - b = \frac D E

- **forward rate of return on equity (ROE)**, the business return per annum that investors expect from a firm per incremental dollar-investment by a firm for shareholders

    - ROE here is different than the historic ROE we looked at before
    - this ROE is on new money invested

.. admonition:: Rate Of Growth

    - the rate of growth for 

        1. book equity 
        2. ex-dividend share price 
        3. dividends 
        4. earnings 
        5. sales 
        6. book assets 
        7. debt 
        8. CAPX  
        9. Trade Capital (TC)

    let...
        
    .. math::
        
        g = \text{% growth in earnings}

    such that...

    .. important::

        .. math::

            g = b*ROE 


.. admonition:: Value of a Share Using Constant Growth Discounted Dividend Model

    .. math::

        Pr  &= \frac {Div} {r - g} \\ 
            &= \frac {\text{payout ratio} * E} {r - g} \\ 
            &= \frac {(1 - b)*E} {r - b*ROE}

    - as b increases, the numerator decreases
    - as b increases, the denominator decreases
    - which effect dominates? it depends

Example - is the company doing well with the money it's retaining?
``````````````````````````````````````````````````````````````````

====    =====   =====   =====
\       base    #1      #2
====    =====   =====   =====
E       3.50    3.50    3.50
r       0.1     0.1     0.1
b       0       0.2     0.5
ROE     --      0.2     0.05
Pr      35      46.67   28.33
g       0       0.04    2.5
====    =====   =====   =====

- base standard investment rate is 0.1
- case 1, ROE = 0.2 > 0.1 = r -> company is doing well with my money its retaining
- case 2, ROE = 0.5 < 0.1 = r -> company is not doing well with the money its retaining

Price Earnings Ratio
---------------------

- **price/earnings ratio (P/E ratio)**, measures the amount that investors pay per dollar of earnings
- investors try to use value ratios to try to identify what they believe might be "cheap" or "expensive" common shares for their portfolios
- typically range from 5 to 40

.. math::

    \frac P E = \frac {1-b} {r - b * ROE}
    \frac P E = \frac {1-b} {dy}

Present Value of Growth Opportunities
-------------------------------------

.. warning:: This section is incomplete.

(N)PVGO = (net) present value of growth opportunities

    - what happens when b is 0?

Efficient Market Hypothesises
-----------------------------

- if you have a free operating market with low transaction costs and information is freely available then prices are correct

- **Weak Market Efficiency**, prices encorporate all past prices

    - inefficient in this way if people can look at historical prices to make an abnormal return

- **Semi-strong Market Efficiency**, all public information is incorporated in share prices
    
    - e.g. finding gold -> price change immediately before buyers can act, since sellers know the information too
    - inefficient in this way if people can use public knowledge to make an abnormal return
    - most people think that the market is efficient in at least the semi-strong form

- **Strong Market Efficiency**, all public and private information is incorporated in share prices

    - inefficient in this way if people can use insider knowledge to make an abnormal return

- if market is inefficient, then there are incorrect prices, and people can make an abnormal return

    - can people identify stocks for which the price is over/undervalued? if so, market is inefficient in some way


Equity Financing
----------------

- a distribution of sales is a sale of new shares to new shareholders for the purpose of financing a firm's business activities
    
    - if a firm has not had its shares traded on an organized public stock exchange, (i.e. it was an unlisted company,) the issuing firm must file a prospectus with the appropriate financial regulators
        
        - the prospectus describes the firm, its business, introduces the directors and officers, and describes the securities to be sold
    
    - if a firm has a listing on a stock exchange, (in Canada) the firm can sell new shares to new shareholders by simply notifiying the exchange and possibily provincial secruties regulators with an **exchange offering prospectus**

        - this doucment is simler and less detailed than the traditional prospectus
        - **seasoned issue**, a sale of new shares by a firm with a listing 

- this issue is called an initial public offering and the firm will then have a listing on the stock-market after the share sale

- a public firm can make a seasoned issue in one of two ways: a general cash offer or a rights issue

General Cash Offer
''''''''''''''''''

- **general cash offer**, the sale of new shares to any investor, more or less, who wishes to purchase
- on the Toronto Stock Exchange, firms can raise a maximum of 5 million over a six month period with an exchange offering prospectus

.. admonition:: Dilution in a General Cash Offer

    - when a firm sells new shares to shareholders, the fractional ownership of existing shareholders is diluted
    - earnings are shared amongst a greater number of shareholders, and the fractional ownership of any original shareholder is diminished
    - should firms avoid the use of general cash offers to avoid the impact of dilution on their shareholders?

        - not necssarily
        - if financial markets are informationally efficient, existing shareholders are not necessarily worse off because of the general cash offer (as their welath is not decreased)

    - when a firm sells new shareholders, although ownership is diluted, the size of the firm's market equity grows because of contributions from new shareholders
        
        - if the size of the growth is sufficient, the original shareholders are not worse off

Example: General Cash Offer
````````````````````````````

.. image:: _static/ch8_ex_1.png

.. math:: 

    \text{current number of shares outstanding} = 2 million

- this market value balance sheet shows the PV existing operations and planned new ventures against equity
- the existing operations could be sold for 10 million
- the new venture has not yet been financed so it has no trade capital assets, plant, property, or equipment

    - the general cash offer will raise these funds

- suppose that :math:`NPV_{\text{new venture}} = PV_{gains} - PV_{losses} = 6 million - 1 million = 5 million`
- the required investment for this new venture is 1 million

    - thus, new shares need to be sold

- financing this venture and purchasing TC, plant, property, and equipment will turn the intangible asset into a tangible operating asset of the firm

.. math:: 

    Pr_{share}  &= \frac {\text{total market equity}} {\text{number of shares}} \\
                &= \frac {$15 million} {2 million} \\
                &= $7.5
                
- suppose that investors "see through" ABC's activities and recognize that the new venture has an NPV of $5 million 

    - they are willing to pay an additional $5 million for the existing shares of ABC
    - they are willing to pay $2.5 = 7.5 - 5 per share for the growth prospects associated with ABC's planned new venture

- what price to sell new shares for?

    - if :math:`Pr_{\text{new share}} > 7.5`, investers will choose to buy shares in current secondary market instead
    - if :math:`Pr_{\text{new share}} < 7.5`, you're getting less for the shares than they're worth
    - it would be good for ABC to sell its new shares at $7.5 so that investors find the new shares more attractive than the old shares

- ABC must sell $1 million / 7.5 = 133,333 new shares at $7.5 to raise $1 million to finance its new venture
- the fractional ownership of the existing shareholders will fall from 100% to :math:`\frac {2 million} {2 million + 0.133333 million} = 93.75%`

.. image:: _static/ch8_ex_2.png

- market value of equity is increased by the $1 million contributed by the new shareholders
- the share price for existing and new shareholders after financing operation is 

.. math:: 

    Pr_{share}  &= \frac {\text{total market equity}} {\text{number of shares}} \\
                &= \frac {$16 million} {2.133333 million} \\
                &= $7.5

- no leakage of NPV of the new venture because firm set the correct price in the offer ($7.5)
- even with no leakage and new sharholders getting 0 NPV investment, they purchase because they expect a rate of return which just compensates for the risk they bear -- the market capitalization rate
- if they were to get a return > the market capitalization rate, the firm would be under-pricing its new shares

Rights Offer
''''''''''''

- in a rights issue, the existing shareholders are given first a preemptive "right" to buy new shares in proportion to their existing ownership
- a rights issue is akin to a combination of a new share issue and a *stock split*

    - the stock split aspect causes the share price to fall

- shareholders are not worse off if they do either:

    - use their rights to purchase their fractional ownership of the firm in the new issue
    - sell their rights


Example: Rights Offer
`````````````````````

=============   =========   ==============  ======================
\               general     cash offering   rights offering
-------------   --------------------------  ----------------------
\               ideal       underpricing    \
=============   =========   ==============  ======================
\               \           \               \
\               \           \               \
market value    50000
shares          1000
Sh price        50
\               \           \               \
NPV             30000
MV              80000
SH price        80
Invest needed   20000
Issue price     80          75              50
#new shares     250*        266.7           400**
\               \           \               \
MV              100000      100000          100000
# shares        1250        1266.7          1400
SH price        80          78.95           71.43
=============   =========   ==============  ======================

1 Star (*):

.. math::

    \text{# new shares} &= \frac {\text{investment needed}} {Pr_{share}} \\
                        &= \frac {20000} {80} \\
                        &= 250

2 Star (**):

.. math::

    \text{# rights needed to buy a share}   &= \frac {\text{# shares}} {\text{# new shares}} \\
                        &= \frac {1000} {400} \\
                        &= 2.5

- rights offerings must be priced at below value of shares for general case

- share price increases because shareholders expect dividends to increase as a result of investment

    - shareprice is a function of the expectation on dividend behavior

.. admonition:: Lost Value Per # rights needed to buy a share

    let...

    .. math::

        SPR = shares/right = \text{# rights needed to buy a share}

    such that...

    .. math::

        \text{lost value over SPR shares}   &= \text{value of SPR Old Shares} - \text{value of SPR new shares} \\
                                            &= \text{value of an old share} * SPR - \text{value of a new share} * SPR


.. math::

    \text{lost value over SPR shares}   &= \text{lost value over 2.5 shares} \\
                                        &= \text{value of 2.5 old shares} - \text{value of 2.5 new shares} \\
                                        &= 2.5 * 80 - 2.5 * 71.43 \\
                                        &= 200 - 178.56 \\ 
                                        &= 21.43 

A Right is granted per 2.5 shares in this ex.

.. admonition:: Value of a Right

    .. math::

        \text{value of right} = \frac {\text{lost value over SPR shares}} {SPR}


.. math:: 

    \text{value of right}   &= \frac {\text{lost value over SPR shares}} {SPR}
                            &= \frac {\text{lost value over 2.5 shares}} {2.5}
                            &= \frac {21.43} {2.5} \\
                            &= 8.57 


====================    ==========      =========   ========
\                       Exercise        Sell        Trash
====================    ==========      =========   ========
# shares                100             100         100
Start Eq                8000            8000        8000
Start Bank a/c          5000            5000        5000
Start Wealth            13000           13000       13000
\                       \               \           \
# shares bought         40              --          --
cash from rights        -2000           857         --
\                       \               \           \
# shared owned          140             100         100
End Eq                  10000*          7143        7143
End bank a/c            3000            5857        5000
End Wealth              13000           13000       12143**
====================    ==========      =========   ========

- *71.43 * 140 = 10000
- **note: 13000-12143 = 857


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
\               \
\               \
#Sh             2n
New MV          20 + x + 24
New Shp         (44 + x)/2n
==============  ============

suppose:

    .. math::     

        (44+x)/2n = 0.75*(20x)/n
        x = 28


Value of a right = 0.80

    - value of the right is a function of the share price, so you can figure out the old share price from the value of the right

Old Share Price = 0.80/0.25 = 3.20
New Share Price = 2.40

3.2 = (20 + 2.8) / n => n = 4.8/3.2 = 15

