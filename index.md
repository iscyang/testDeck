---
title       : Why Develop Our Own Cloud Service
subtitle    : Competitors are monitoring us
author      : Isaac
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [quiz, bootstrap, mathjax]     # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Motivation
- Our company has been processing and approving hundreds of mortgage applications each year.
- Most of them requires services and information provided by third parties.
- Recently, we discovered some of those third parties were leasing, renting, selling, trading and/or lending our applicants' information with others, which may include our competitors.
- Impacts of such information leaking
  - Clients being approached by competitors
  - Competitors undercut and invade our market
  - Competitors understands our loan processing flow
  - Clients' confidence to us could become lower
- We need to reduce our dependency on third party services.

---

## First In-house Cloud Service
- Mortgage payment calculator
- A simple but useful tool
- Work anywhere as long as you have internet access
- No information shared with 3rd party
- Everything under company's control
- High security measure
- Expandable to other tools and applications
- Input
  - Loan amount, Loan term, Interest rate
- Output
  - Monthly payment

---

## Technical details
- Written in Shiny (an R package)
- Deployed in shinyapp.io (a service from RStudio)
- Includes two files, ui.R and server.R.
- Fully interactive and works on different browsers
- Based on formula

$$\frac{Lr}{1-\frac{1}{(1+r)^n}}$$

, where $L$ is the loan amount, $r$ is monthly interest rate, and $n$ is the total number of payments.

<sub>Note to peer assessment reviewer: please refresh this page if the formula is not shown correctly.  My Chrome browser needs it every time.</sub>


---&radio

## See how senior you are as a loan approval advisor



What is the monthly payment for a $500,000 30-year loan with annual interest rate 5.5%?

1. $4129.76
2. $1844.22
3. _$2838.95_
4. $3365.13

*** .hint

As a senior loan approval advisor, you don't need a hint

*** .explanation

Use the formula in previous slide

