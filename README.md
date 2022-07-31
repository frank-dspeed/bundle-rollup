# bundle-rollup
This is a rollup distribution build with rollup to get used as dependencie in other projects that depend on rollups internal source.

## Why?
Rollup is a key dependencie as it contains algos that do solve many issues when dealing with 3th party Javascript/ECMAScript Modules
it self is distributed in a way to work like a Application while it contains many usefull functions that can get used indipendent.

as i do never intend to replicate functionality that already exists and even is as well maintained and tought of as rollup.
I am Forced to rebundle it from the source into something usefull for reuse in my projects that even do run on diffrent platforms.

## Content of this Fork
- Better Code splitting
  - creates rollup as ESM only package including a CJS Wrapper that offers Methods to sync spawn rollup 
    - this allows usage inside projects that depend on Nativ Side Effects of the JS Engine as the CJS version can be used Sync while ESM is always Async
- Correct Typescript definitions and files 
- Bundels Many common used Plugins
  - Includes Typescript Version that also follows the same patterns bundle-typescript. 
