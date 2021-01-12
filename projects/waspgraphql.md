---
title: Wasp GraphQL
layout: page
---

## Inspiration

While at Codesmith, I gained a passion for GraphQL. After an update for Apollo, the community on Reactiflux and Hackernews expressed concerns on their already robust Redux codebase. The Apollo Client made Redux redundant for React developers. I wanted to continue sticking to DRY Code principles and ensure that developers would not have to completely overhaul their codebases or give up on Apollo. 

## What it does

In order to remove the feeling that Redux would be redundant with Apollo Client's new state management, I developed a bridge between Redux and Apollo. It allowed developers to continue using GraphQL and save considerable development time. The project is on NPM. It simultaneously updates the state management between Apollo and Redux and simplifies GraphQL queries in one line of code. Since it is a micro library, it also significantly decreases latency.

## How we built it

We built the micro library by creating the base of Wasp GraphQL as a simple fetch request. A graphQL query is passed just like a URL in fetch in one line of code. 

## Challenge we ran into

GraphQL is a pretty new language, the documentation is pretty robust, and there was no information on how to create this bridge. My team and I in Black Wasp Tech spent countless hours researching GraphQL queries, subscriptions, and how they were passed within the code base in order develop the bridge. Besides lack of documentation on how to get this done, how to properly pass the prop drill GraphQL queries between both stores in the state management library was difficult.