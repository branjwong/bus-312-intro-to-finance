Equity Securities and Equity Markets
====================================

- shares give you a say in the management of a company
- value of a share is the present value of the future cash flows

    - question: what are those cash flows going to look like?

- valuation is far less certain than bonds
- non-voting shares are so the share issuer can maintain control of a company
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

.. math::

    PV  &= P \\
        &= \frac {Div} r

Market Capitalization Rate
--------------------------

Cash Cow
````````

.. image:: _static/straight_line.png

.. math::

    Pr = \frac {Div} r

Constant Growth
```````````````

.. image:: _static/constant_growth.png

.. math::

    Pr = \frac {Div} {r - g}


Example
'''''''

:: 

    Div = 2
    r = 0.1
    g = 0.05

.. math::

    Pr_{t=0}    &= \frac {2} {0.1 - 0.05} \\
test
                &= 40

.. math::

    Pr_{t=1.00001}  &= \frac {2 * 1.05} {0.1 - 0.05} \\
                    &= 42

.. math:: 

    Pr_{t=0.99999}  &= \frac {2} {0.1 - 0.05} * (1 + 0.1) \\
                    &= 44


Example
-------

b = retention ratio

    This number means that
    for every dollar of earnings available for distribution to shareholders, the firm distributes 100*(1-b) cents
    as a dividend to shareholders and retains 100*b cents for business reinvestment and growth.

E = earnings

- ROE here is different than the historic ROE we looked at before
- this ROE is on new money invested

.. math::

    \text{% growth in earnings} &= \frac {b*E*ROE} {E} \\
                                &= b*ROE \\
                                &= g

.. math::

    Pr  &= \frac {Div} {r - g} \\ 
        &= \frac {(1 - b)*E} {r - b*ROE}

- as b increases, the numerator decreases
- as b increases, the denominator decreases
- which effect dominates? it depends

====    =====   =====   =====
\       base    #1      #2
====    =====   =====   =====
EPS     3.50    3.50    3.50
r       0.1     0.1     0.1
b       0       0.2     0.5
ROE     --      0.2     0.05
Pr      35      46.67   28.33
g       0       0.04    2.5
====    =====   =====   =====

- EPS = earnings per share (probs in form of dividend)

- is the company doing well with the money it's retaining?
    
    - base standard investment rate is 0.1
    - case 1, ROE = 0.2 > 0.1 = r -> company is doing well with my money its retaining
    - case 2, ROE > 0.5 < 0.1 = r -> company is not doing well with the money its retaining


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


Example

*MV = market value of firm

=============   =========   ==============  ======================
\               general     cash offering   rights offering
=============   =========   ==============  ======================
\               ideal       underpricing    \
\               \           \               \
\               \           \               \
MV              50000
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


- *: 250 = 20000/80
- ** 1000/400 = 2.5 rights needed to buy a new share

- rights offerings must be priced at below value of shares for general case

- share price increases because shareholders expect dividends to increase as a result of investment

    - shareprice is a function of the expectation on dividend behavior

.. math::

    \text{Lost Value over 2.5 Shares}   &= \text{Value of 2.5 Old Shares} - \text{Value of 2.5 New Shares ??} \\
                                        &= 2.5 * 80 - 2.5 * 71.43 \\
                                        &= 200 - 178.56 \\ 
                                        &= 21.43 \\ 
                                        ???

A Right is granted per 2.5 shares in this ex.

.. math:: 

    \text{Value of Right}   &= 21.43/2.5 \\
                            &= 8.57 \\
                            ??


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
``````````````````

- **general cash offer**, the sale of new shares to any investor, more or less, who wishes to purchase
- on the Toronto Stock Exchange, firms can raise a maximum of 5 million over a six month period with an exchange offering prospectus

Dilution in a General Cash Offer
''''''''''''''''''''''''''''''''

- when a firm sells new shares to shareholders, the fractional ownership of existing shareholders is diluted
- earnings are shared amongst a greater number of shareholders, and the fractional ownership of any original shareholder is diminished
- should firms avoid the use of general cash offers to avoid the impact of dilution on their shareholders?

    - not necssarily
    - if financial markets are informationally efficient, existing shareholders are not necessarily worse off because of the general cash offer (as their welath is not decreased)

- when a firm sells new shareholders, although ownership is diluted, the size of the firm's market equity grows because of contributions from new shareholders
    
    - if the size of the growth is sufficient, the original shareholders are not worse off

Example:

.. image:: _static/ch8_ex_1.png

:: 

    current number of shares outstanding    2 million

- this market value balance sheet shows the PV existing operations and planned new ventures against equity
- the existing operations could be sold for 10 million
- the new venture has not yet been financed so it has no trade capital assets, plant, property, or equipment

    - the general cash offer will raise these funds

- suppose that :math:NPV_{\text{new venture}} = PV_{gains} - PV_{losses} = 6 million - 1 million = 5 million
- the required investment for this new venture is 1 million

    - thus, new shares need to be sold

- financing this venture and purchasing TC, plant, property, and equipment will turn the intangible asset into a tangible operating asset of the firm

.. math:: 

    Pr_share    &= \frac {\text{total market equity}} {\text{number of shares}} \\
                &= \frac {$15 million} {2 million} \\
                &= $7.5
                
- suppose that investors "see through" ABC's activities and recognize that the new venture has an NPV of $5 million 

    - they are willing to pay an additional $5 million for the existing shares of ABC
    - they are willing to pay $2.5 = 7.5 - 5 per share for the growth prospects associated with ABC's planned new venture

- what price to sell new shares for?

    - if Pr_{\text{new share}} > 7.5, investers will choose to buy shares in current secondary market instead
    - if Pr_{\text{new share}} < 7.5, you're getting less for the shares than they're worth
    - it would be good for ABC to sell its new shares at $7.5 so that investors find the new shares more attractive than the old shares

- ABC must sell $1 million / 7.5 = 133,333 new shares at $7.5 to raise $1 million to finance its new venture
- the fractional ownership of the existing shareholders will fall from 100% to :math:`\frac {2 million} {2 million + 0.133333 million} = 93.75%`

.. image:: _static/ch8_ex_2.png

- market value of equity is increased by the $1 millino contributed by the new shareholders
- the share price for existing and new shareholders after financing operation is 

.. math:: 

    Pr_share    &= \frac {\text{total market equity}} {\text{number of shares}} \\
                &= \frac {$16 million} {2.133333 million} \\
                &= $7.5

- no leakage of NPV of the new venture because firm set the correct price in the offer ($7.5)
- even with no leakage and new sharholders getting 0 NPV investment, they purchase because they expect a rate of return which just compensates for the risk they bear -- the market capitalization rate
- if they were to get a return > the market capitalization rate, the firm would be under-pricing its new shares

Rights Offer
````````````

- in a rights issue, the existing shareholders are given first a preemptive "right" to buy new shares in proportion to their existing ownership
- a rights issue is akin to a combination of a new share issue and a *stock split*

    - the stock split aspect causes the share price to fall

- shareholders are not worse off if they do either:

    - use their rights to purchase their fractional ownership of the firm in the new issue
    - sell their rights


