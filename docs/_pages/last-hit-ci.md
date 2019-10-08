---
title: "CI Integration"
permalink: /ci/
excerpt: "CI intergation"
last_modified_at: 2018-01-10T11:22:01-05:00
---



# Install

```
npm install last-hit-replayer
```

or

```
yarn add last-hit-replayer
```

Yarn is recommanded. For install Yarn, see [yarnpkg.com](https://yarnpkg.com/)

# Run

## Run whole workspace
```
yarn start --workspace=directory/to/your/workspace
```

## Specify Story
```
yarn start --workspace=directory/to/your/workspace --story=your-story-name
```

## Specify Flow
```
yarn start --workspace=directory/to/your/workspace --story=your-story-name --flow=your-flow-name
```

> Flow name will be ignored when story name does not specify.

