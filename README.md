# Mini Test

A small repository with TypeScript pre-configured.

- [Setup](#setup)
- [Execute](#execute)
- [Data](#data)
- [Objectives](#objectives)

## Setup

```sh
$ git clone https://github.com/tempo-video/mini-test.git
$ cd mini-test
$ npm install
```

## Execute

The `package.json` features a test command that will execute `test.ts`

```sh
$ npm test

hello world

```

## Data

The project includes a dataset in the `test.json` file.

This is a list of subtitles with their properties:

- the `text` that should be displayed
- the `timestamp`, in milliseconds, from which the subtitle becomes visible
- the `duration`, in milliseconds, until the subtitle disappears
- a unique `identifier`

## Objectives

The goal is to be able to run the test (`npm test`) with the following results:

1. the `test.json` file is read
2. the list of subtitles is displayed
3. the order of the subtitles is corrected
4. the list of subtitles is displayed in the correct order
5. the overlaps are removed by moving subtitles further in time
6. the subtitles are displayed in the correct order, with no overlap
