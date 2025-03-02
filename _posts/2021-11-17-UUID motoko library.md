---
layout: post
title:  "Bounty - ICDevs.org UUID motoko library"
date:   2021-11-17 00:00:00 -0600
categories: "Bounties"
author: Austin Fatheree
---

# Create a UUID Library in Motoko - #4

## Current Status: Discussion

* Discussion (11/17/2021) <- We are here
* Ratification (11/19/2021)
* Open for application (11/19/2021)
* Assigned (11/19/2021)
* **In Review** (11/23/2021) <- We are here
* Closed

[Issue Link - Discussion Forum](https://forum.dfinity.org/t/icdevs-org-bounty-4-uuid-motoko-library/8648)

## Bounty Details

* Current Bounty Amount: 20 ICP
* ICDevs.org Match Available: 20 ICP - (For every ICP sent to 66083bb3c940c7de2a70aa127ec771da75d60deadc10f5f66b280f203d8f6e73, ICDevs.org will add one more ICP to the bounty, up to 20 ICP, After 20 ICP, Donations to the above address will add .25 ICP to this issue and .75 ICP to fund other ICDevs.org initiatives)
* Time Left: Expires 12/31/2022
* Project Type: Single Contributor
* Opened: 11/17/2021
* Time Commitment: Days
* Project Type: Traditional
* Experience Type: Intermediate - Motoko; Intermediate - Encoding
* Issue Type: Application Development

## Description

This bounty gives the opportunity to

* learn how motoko works
* learn about unique ID encodings
* learn about randomness on the IC

A donor(The Dragginz Team) generously funded a full bounty for ICDevs to help find a dev that would like to build a UUID library.

The spec for UUID v4 can be found at https://datatracker.ietf.org/doc/html/rfc4122

Quint has done a ton of work on this already at https://github.com/aviate-labs/uuid.mo. As a result we'll give him first dibs on this bounty if he wants to update the library to add the psudorandom non-await branch.

There are a number of example libraries in other languages.  You will need to transcode the library into motoko.  This may require the construction of other sub libraries for encoding, string manipulation, and decoding.

There are unique properites that the IC has that you should take advantage of.  The IC provides randomness via the [Random](https://sdk.dfinity.org/docs/base-libraries/random) base library.  This library should have two modes. One where true randomness is used and another where an alternative form of randomness that does not require an async await to be used.  Perhaps hashing the Principal of the canister plus an always increasing nonce might do the trick but a healthy discussion should ensue about what will work and what won't.

## Application:

Github user @di-wu (everyone's favorite quint) has applied for this bounty.

## Selection:

Github user @di-wu was selected for this bounty.

## Bounty Completion:

The code at the following repo was submitted by github user di-wu:  [https://github.com/aviate-labs/uuid.mo](https://github.com/aviate-labs/uuid.mo)  and is available for review.

## Funding

The bounty was generously funded by a donor(The Dragginz Team). If you would like to turbocharge this bounty you can seed additional donations of ICP to 66083bb3c940c7de2a70aa127ec771da75d60deadc10f5f66b280f203d8f6e73.  ICDevs will match the bounty 1:1 for the first 20 ICP and then 0.25:1 after that.  All donations will be tax deductible for US Citizens and Corporations.  If you send a donation and need a donation receipt, please email the hash of your donation transaction, physical address, and name to donations@icdevs.org.  More information about how you can contribute can be found at our [donations page](https://icdevs.org/donations.html).

## General Bounty Process

### Discussion

The draft bounty is posted to the DFINITY developer's forum for discussion

### Ratification

The developer advisor's board will propose a bounty be ratified and a vote will take place to ratify the bounty.  Until a bounty is ratified by the Dev it hasn't been officially adopted. Please take this into consideration if you are considering starting early.

### Open for application

Developers can submit applications to the Dev Forum post.  The council will consider these as they come in and propose a vote to award the bounty to one of the applicants.  If you would like to apply anonymously you can send an email to austin at icdevs dot org or sending a PM on the dev forum.

### Assigned

A developer is currently working on this bounty, you are free to contribute, but any splitting of the award will need to be discussed with the currently assigned developer.

### In Review

The Dev Council is reviewing the submission

### Awarded

The award has be been given and the bounty is closed.

# Matches

We are waiting on our first community match.


[Other ICDevs.org Bounties](https://icdevs.org/bounties.html)

