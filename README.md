# React Native FlatList Performance Issue

This repository demonstrates a common performance issue in React Native when using FlatList with large datasets. The app becomes unresponsive when rendering many items.

## Problem

The provided `bug.js` file contains a simple FlatList implementation that renders 30 items.  With a larger dataset, scrolling becomes laggy and the app may freeze. This is due to the default behavior of FlatList which renders all items at once if not optimized.

## Solution

The `bugSolution.js` file provides a solution utilizing `windowSize` and `removeClippedSubviews` props to optimize the rendering process, dramatically improving performance.