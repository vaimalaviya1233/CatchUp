<p>
  <img src="https://github.com/hzsweers/CatchUp/blob/master/app/src/main/play/en-us/listing/featureGraphic/feature.png?raw=true" width="250" height="250"/>
</p>

CatchUp
=======

An app for catching up on things.

## Motivations

There's a lot of services I like reading up on throughout the day. Most of these services have 
dedicated apps for consuming them, but often times I just want to skim the front page and only deep
dive occasionally. Enter CatchUp: a high level presentation of the "front page" of several services 
in short form, and intelligent deeplinking into dedicated apps if you want to go further.

CatchUp is not an all-purpose client for each of these services, just the concierge for at-a-glance
details and router for getting on your way. It does not support login for any service, it does not 
support customization/filtering of their feed. CatchUp is dumb, and you should use one of the many
great dedicated apps for this if you want more integration features.

CatchUp is also very much a testing ground for things I personally dive into, from architecture, 
libraries, patterns, API quirks, and more. It's been a very fun project to spike test new things.

## Features

- Multiple services
  - Hacker News
  - Reddit
  - Medium
  - Product Hunt
  - Slashdot
  - Designer News
  - Dribbble
  - GitHub
- Infinite scrolling on supported services
- Pleasant, simple, consistent UI for across services
- Night mode
- Smart deeplinking into dedicated apps

## Technologies

- Kotlin
- RxJava 2/AutoDispose
- Debugging tooling as a first class citizen in the debug build
  - Leak Canary, Chuck, Scalpel, Debug drawer, the works
- Conductor
- Dagger 2
  - One of the more interesting parts of CatchUp is that its service architecture is a Dagger-powered plugin system
- AutoValue + extensions
- Firebase
- Glide
- Apollo GraphQL
- Standard Square buffet of Okio/OkHttp 3/Retrofit 2/Moshi
- ThreetenABP
- Inspector
- PSync

There's a lot of neat/interesting little tidbits in the CatchUp source code that I plan to write a 
mini blog series about. Each service has its own nuances that make them unique to work with in code.

## Testing

While this is a personal pet project, extensive tests can be found [here](https://youtu.be/oHg5SJYRHA0).

## Influences

This app owes a lot of its inspiration, implementation details, and general inner workings to the 
work of others. Particularly:
- [Nick Butcher](https://twitter.com/@crafty) and his [Plaid](https://github.com/nickbutcher/plaid) app
- [Jake Wharton](https://twitter.com/@jakewharton) and his [u2020](https://github.com/jakewharton/u2020) demo app

License
-------

    Copyright (C) 2017 Zac Sweers

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
