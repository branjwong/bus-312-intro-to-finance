Fixed Income and Debt
=====================

- difference bewtween debt and equity as financial assets
    
    - payments on debt are *contractually* promised

        - debtholders can sue the issuer for default of principal or interest payments
        - tax deductible b/c interest is contractually proised and is an expense of the corporate issuer 

    - payments on equity are not
        
        - board of directors of a corporation can cut or eliminate dividends on a common share or a preferred share and the holders of these equity securities cannot (typically) sue the firm
        - not tax deductible because dividends are not contractually *guarenteed*, they are not an expense of the firm

- difference between private and public debt

    - private borrowing contracts = loans
    - public borrowing contracts = bonds

Public Debt Markets and Bond Valuation
--------------------------------------

- **bond**, a public financial asset that makes contractually promised payments for a finite term
- **bond's maturity**, the remaining term over which repayments are promised

- bond payments are often fixed and do not vary over the investment term
- interest on a floating bond varies in a predefined way with the general level of interest in the economy

- **coupons**, income payments on a bond

    - North America: bonds typically make semi-annual coupon payments
    - Europe: bonds typically make annual coupon payments

- **par value**, the value of the final payment made which is paid at maturity

    - par value :math:`\neq` not the value of the bond, but value of bond = f(par value)
    - par value :math:`\neq` not necessarily the amount originally borrowed, but amount original borrowed = f(par value)
    - establishes the coupon and maturity payments

- bonds are often sold as sets of bonds, called bond issues
- most public bond issues are between approx 10mill and 100million dollars

.. admonition:: Calculating Bond Coupons

    - coupons on a bond are calculated as a per annum coupon rate of interest times par divided by number of payments per year

    .. math::

        C_{\text{bond coupons}}     &= \frac {r_{c}} {n} * M \\

    - :math:`r_{c} = \text{annual coupon rate}`
    - :math:`M = \text{the par value of the bond}`
    - :math:`n = \text{number of payments per year}`

Yield to Maturity
`````````````````

- **yield to maturity**, the IRR on an investment in a bond on the promised payments to maturity, expressed as a :math:`j_2`, a rate compounded semi-annually

.. math:: 

    y = j_{2,y} \\
    EIR_{2,y} = \frac {j_{2,y}} 2 

.. admonition:: How YTM relates to IRR and NPV

    - recall: the IRR is that hypothetical discount rate which makes net present value of a set of predicted future payments equal zero
    - **invoice price of a bond**, the dollar amount required to purchase a bond 

    .. math::

        NPV &= CF_{\text{purchasing bond}} + A_{coupons} + M_{\text{par value}} \\
        0 &= - \text{Invoice Price} + \frac {C_{coupons}} {EIR_{2,y}} * (1 - \frac 1 {(1 + EIR_{2,y})^n}) + \frac M {(1 + EIR_{2,y})^n}

    - :math:`C_{coupons}` is value of the semi-annual coupon
    - y is the yield (per annum) compounded semi-annually
    - n is the number of six-month coupon periods to maturity
    - M is the par value of the bond

    Thus you can calculate the invoice price if you have everything else.

    .. math::

        \text{Invoice Price} = \frac {C_{coupons}} {EIR_{2,y}} * (1 - \frac 1 {(1 + EIR_{2,y})^n}) + \frac M {(1 + EIR_{2,y})^n}


    - the bond matures in n/2 years
    - the invoice price of a bond is the presevent value of the annuity of the coupons plus the present valu eof the lump sum par value payment
    - because the bond value is established in trading between bond market participants, the coupons and par value repayment are fixed, while **the yield is a market determined rate**.

- the promised payments are the remaining coupons and par value
- relative to required expenditure, the yield to maturity is the discount rate which makes the NPV of the investment equal zero

- yield on a bond changes contiuously over time as conditions in bond markets change

    - when bond market traders pay greater prices for a bond, yields fall because coupons and par are fixed
    - when rates of interest in the economy rise, the yields on bonds also tend to rise (and bond prices fall)

- linked to the coupon rate and risk premium

    - risk -> price -> YTM, where the arrow shows what influences what


Example - Simple Bond
`````````````````````

::

    Face Value = Par Value = $1000
    Coupon Rate = 8%, twice / yr
    Coupon = 0.08/2 * 1000 = 40
    Time to Maturity = 14 years

.. image:: _static/simple_bond.png


- Coupon's are paid out during bond maturation
- Face Value paid out at time of maturity

- rate that is used to valuate the bond fluxuates depending on the expecation that the company will survive

    .. math::

        r = r_f + \text{risk premium}

- **yield to maturity (YTM)**, used to calculate the bond price which fluxates daily

YTM = 6%

.. math::

    Bond Pr &= \text{Annuity of Coupons} + \text{PV of Bond Payment} \\
            &= \frac {40} {0.03} * (1 - \frac 1 {(1 + 0.03)^{28}}) + \frac {1000} {(1.023)^{28}} \\
            &= 1187.64

- YTM = f(price of the bond, news about the bond issuing firm, time on bond)


Random Bond Facts
`````````````````

.. admonition:: Bonds Priced at Par Value

    .. math::

        Pr = M \Rightarrow EIR_{y,2} = r_c

.. admonition:: YTM and Invoice Price are inversely related

    .. math::

        YTM \uparrow \text{ } \rightarrow \text{ } Pr \downarrow


Holding Period Rate Of Return and YTMs
--------------------------------------

- **holding period**, the period of time between buying a financial asset and selling it
- **holding period rate of return (HPRR)**, measures the rate of growth of wealth as a result of owning a financial asset over a holding period

.. math::

    HPRR_{f - i\text{ periods}} = \frac {V_{t=f} - V_{t=i}} {V_{t=i}}

- :math:`V_{t=i}` (what you purchase the investment for)
- :math:`V_{t=f}` (what you sell the investment for)

:math:`HPRR_{m\text{ months}}` can be converted to a :math:`j_2`.

.. admonition:: Converting Monthly EIRs

    .. math::

        EIR_{12} = (1 + EIR_1)^{\frac 1 {12}} - 1 \\
        EIR_{monthly} = (1 + EIR_{12 \text{ monthly}})^{\frac 1 {12}} - 1 

    .. important:: 

        .. math::
            
            EIR_{n \text{ monthly}} = (1 + EIR_{m \text{ monthly}})^{\frac n m} - 1 


.. admonition:: Calculating HPRR as a :math:`j_2`


    - Suppose that our HPRR was calculated over m months.

    .. math::

        EIR_{6 \text{ monthly}} &= (1 + EIR_{HPRR, m \text{ monthly}})^{\frac 6 m} - 1 \\
        EIR_{2} &= (1 + EIR_{HPRR, m \text{ monthly}})^{\frac 6 m} - 1 \\
        \frac {j_2} 2 &= (1 + EIR_{HPRR, m \text{ monthly}} )^{\frac 6 m} - 1 

    .. important:: 

        .. math::
            
            j_2 = ((1 + EIR_{HPRR, m \text{ monthly}} )^{\frac 6 m} - 1) * 2

Yield as an HPRR
````````````````

- suppose we measure our HPRR as a :math:`j_2`
- yield to maturity is the annualized holding period rate of return (appropriately compounded) on the investment iff

    1. over the holding period, the yield on the bond does not change
    2. over the holding period, interest rates in the economy do not change
    
        - if interest rates have changed and you sell bond before maturity, you will receive an unexpected capital gain or loss on your bond  
        - this affects your HPRR relative to YTM

    3. over the holding period, you reinvest received coupons over the holding period at a rate of interest equal to the yield to maturity

        - if you reinvest coupons at a rate less than the yield, the HPRR will be lesser than the yield
    

Example - Showing YTM = HPRR given conditions
'''''''''''''''''''''''''''''''''''''''''''''

::

    Coupons             2/yr
    Buy 5 months before a coupon
    CR = Coupon Rate    = 7%/annum
    Face Value          = 10000
    29 coupons
    YTM = 8%

    keep for 4 years 9 months - sell
    YTM unchanged

    Back a/c r = j_2 = 8%

.. math::

    \text{Invoice Price}    &= V_{t=0, A_{coupons}} + V_{t=0, M} \\
                            &= V_{t=-\frac 1 6, A_{coupons}} * (1 + r) ^ {\frac 1 6} + V_{t=-\frac 1 6, M} * (1 + r) ^ {\frac 1 6} \\
                            &= (V_{t=-\frac 1 6, A_{coupons}} + V_{t=-\frac 1 6, M}) * (1 + r) ^ {\frac 1 6} \\
                            &= [\frac {350} {0.04} * (1 - \frac 1 {1.04^{29}}) + \frac {10000} {1.04^{29}}] * 1.04^{\frac 1 6} \\
                            &= 9210.83

.. math::

    Selling Price   &= [\frac {350} {0.04} * (1 - \frac 1 {1.04^{20}}) + \frac {10000} {1.04^{20}}] * 1.04^{\frac 4 6} \\
                    &= 9567.40

.. math::

    Bank Account    &= \frac {350} {0.04} * (1 - \frac 1 {1.04^9}) * 1.04^{9 + \frac 4 6} \\
                    &= 3802.10


.. math::

    \text{4 yrs 9 months} = \text{57 months} 

.. math::

    EIR_{HPRR, 57\text{ monthly}}   &= \frac {9547.4 + 3802.10 - 9210.83} {9210.83} \\
                                    &= 0.4515

.. math::

    EIR_2 &= (1 + EIR_{HPRR, m\text{ monthly}})^{\frac 6 {m}} - 1 \\
    EIR_2 &= (1 + EIR_{HPRR, 57\text{ monthly}})^{\frac 6 {57}} - 1 \\
    EIR_2 &= (1 + 0.4515)^{\frac 6 {57}} - 1 \\
          &= 0.04 

.. math::

    j_2 &= 0.04 * 2 \\
        &= 0.08


Premium vs. Discount Bonds
--------------------------


- **premium bond**, a bond that trades with a coupon rate that is greater than its yield to maturity

.. admonition:: Definition of Premium Bond

    .. math:: \text{coupon rate} > YTM \Rightarrow \text{premium bond}

    - coupons are more than expected for that time period, given the current YTM
    - offers an *attractive* coupon rate relative to what is available in the bond market from similar risk new issue bonds
    - because of higher coupon rate, bond purchasers are willing to pay a greater price

- **discount bond**, a bond that trades with a coupon rate that is less than its yield to maturity

.. admonition:: Definition of Discount Bond

    .. math:: 
        
        \text{coupon rate} < YTM \Rightarrow \text{premium bond}

    - coupons are less than expected for that time period, given the current YTM

- **par value bond**, a bond that trades with a coupon rate that is equal to its yield to maturity

.. admonition:: Definition of Par Value Bond

    .. math:: \text{coupon rate} =YTM \Rightarrow \text{premium bond}

.. admonition:: Bond Valuation Over Time

    .. image:: _static/bond_valuation_over_time.png

    - premium bond decreases in value as bond matures because

        - coupons are being paid out, and 

    - jagged shape because 

        - as t approaches the time to receive a coupon, the valuation of the bond increases
        - when t passes the time to receive a bond, the valuation of the bond sharply decreases, since that coupon is no longer apart of the valuation
        - after the first coupon is paid, the value of the bond decreases
        - between coupon payment periods, the value increases as you'd rather a bond that pays your first coupon sooner rather than later (e.g. in 1 month vs 6 months)


Discounted Bonds
````````````````

-  why would a bond be valued at less than the par value?

    - the coupon rate is lower than prime rate?
    - characterized by high YTM: why?

.. admonition:: Discontinued Bonds

    .. math::

Current Yield
-------------


.. important::

    .. math:: 
        
        r_c < \text{current yield} < YTM \iff 
        M < Pr \iff 
        \text{discount bond}

Example
```````

::
    
    Apartment
    6 months $120
    Selling Price = Invoice Price = Accrued Int + Quoted Price

YTM = r_f + risk premium
Bought for $500k

What does the rate of return depend on?
    Income Returns:
    Revenues
    Taxes you have to pay
    Insurance
    
    And:
    Capital Gain (even if apartment not sold)

.. math::

    YTM &= \text{Income Component} + \text{Capital Gain} \\
        &= \frac {\text{Annual Coupons in a year}} {Price} + \text{Capital Gain} \\
        &= \text{Current Yield (CY)} + \text{Capital Gain}

Random Table

\           Income      Capital Gain
========    ========    ============
Discount    small +     small +
Premium     big +       small -
        
- overall, Discount and Preimum are expected to be equal (in expected value?)

Risk
----

- There a number of risks associated with fixed income financial assets.

Price Risk + Interest Rate Risk
```````````````````````````````

- Lower coupon rate bonds one have greater prime risk than lower coupon rate bonds, all else equal.
- Longer term bonds have greater price risk than shorter term bonds, all else equal.

Default Risk
````````````


Reinvestment Risk
`````````````````

- uncertainty about reinvesting the coupons
- uncertainty about what rates you will get for a coupon at a later stage
- reinvestment gives uncertainty about what rate you will get
- if YTMs drop in the future, you suffer because you can only invest at a lower rate, value of existing bond increases

Inflation Risk
``````````````


Principal and Interest Payment Deconstruction
---------------------------------------------

.. note:: This section is incomplete.

A period's repayment can be broken up into it's principal and interest portions.

.. math:: 

    C = Princ_{p} + Int_{p}

- C = repayment for any period
- p = some period

-- 

A period's interest portion can be derived from the debt still owed at the period before.

.. math::

    Int_{p} &= r * Debt_{p-1} \\
    Debt_{p-1} &= \frac C r * (1 - \frac 1 {(1 + r)^n}), \text{how do n and p interact?} 

- :math:`Int_{p}` = interest portion debt payment at period p
- :math:`Debt_{p}` = value of debt at period p
- :math:`Princ_{p}` = principal repayment portion of debt repayment at period p
