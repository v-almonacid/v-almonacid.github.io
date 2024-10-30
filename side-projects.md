---
layout: page
title: Side Projects
permalink: /projects/
---

Here's a list of tiny projects and proofs of concept I usually develop in no more than 1-2 weeks of part-time work. I do these for fun, for learning or exploring a new tech tool or just to
share something that might be even remotely useful for somebody.

## Pigui: A Simple, Easy-to-use, Expense Tracker App

| Date | October 2024 |
| Stack | `React` `Typescript` `TailwindCSS`|

![Mnemonic scrambler preview](../assets/pigui.png)

In Chile, banks don't provide APIs to access your transactions. As a result, there no expense tracking apps where you can simply connect your bank account. As a result, I try to keep track of my expenses by using the export to excel feature provided by my bank, copy-paste the transaction in a Google Spread Sheet I built, and then classify all transactions manually.
This was time consuming though, so I've always wanted to build a better solution. That's how `pigui` was born. It allows you to drag-and-drop an `.xlsx` from your bank, auto-classify transactions and display them in a nice, filterable dashboard. All the data stays in your browser.

Credits to [@felipefaraggi](https://x.com/felipefaraggi) for the simple, elegant design.

## Simple Mnemonic Scrambler

| Date | September 2024 |
| Stack | `React` `Typescript` `TailwindCSS`|

![Mnemonic scrambler preview](../assets/mnemonic-scrambler.png)

This [app](https://mnemonic-scrambler.vercel.app/) lets you transform a BIP39 seed phrase into a scrambled version, that is, a series of strings composed by random characters that don't resemble a typical seed phrase.
**You do not need to enter your seed phrase to use this app**. Simply input a password, which will be used to encode each word of the BIP39 English set.
Then scroll around the UI to find each word of your seed phrase and write down the scrambled version. Finally, store it using the same recommended practices for storing standard seed phrases.
Just remember to save your password safely elsewhere.
To restore your seed phrase back in plain text, just follow the inverse process.

## Dumbmarketcap

| Date | December 2023 |
| Stack | `React` `Typescript` `Ionic` `Python` `fastAPI`|

![Dumbmarketcap preview](../assets/dmc.png)

Dumbmarketcap is a cryptocurrency price tracking site (much like coinmarketcap) where the prices are adjusted using the supply of a reference coin of your choice.
The idea is to show that coins that some people might consider "cheap" would actually be quite expensive if they had a smaller supply. For instance,
if WIF (dogwifhat) had the same supply than bitcoin, its adjusted price would be:

```
adjusted_price = coin_market_cap / reference_coin_supply
```

which at the moment of writing these lines equals 142 USD instead of its current trading value of 2.8 USD.

Co-authored by [@felipefaraggi](https://x.com/felipefaraggi).

## Corte Maestro (Linear Cut Optimizer)

| Date | September 2023 |
| Stack | `React` `Ionic` `Typescript` |

![Corte maestro preview](../assets/corte-maestro.png)

A while back when doing some home improvement work I had to buy a bunch of pieces of steel from some local workshops. When discussing prices with one
of these workshops I realized their costs could be reduced by optimizing the cuts on the original pieces of steel, which come in lengths of 3 m. This is actually a classic optimization
problem called the "cutting stock problem". Anyway, to help these workshops reduce their costs I coded this simple [app](https://corte-maestro.vercel.app/app).
