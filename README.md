# Turning Decomposition into a Forecasting Strategy

A decomposition-first forecasting framework for weekly time series, based on adaptive decomposition selection, component-wise modeling, and robust ensemble aggregation.

## Project Website
Visit the project page here:

Project Site

## Overview

This project documents a forecasting architecture designed for weekly time series with overlapping trend, seasonality, holiday effects, and irregular noise.

The key idea is to treat decomposition as a forecasting strategy rather than as a simple preprocessing step.

## Core approach

- Generate multiple decompositions of the same series
- Split each decomposition into adjusted and seasonal components
- Select the decomposition with the lowest combined residual error
- Forecast each component with a specialized model family
- Recombine and aggregate with complementary models
- Stabilize the final output with rolling median smoothing

## Methods used

- STL
- STL + classical decomposition
- AutoSTR
- ARIMA with exogenous regressors
- ETS
- Prophet
- NNETAR

## Public scope

This repository is a public showcase of the methodology, architecture, and selected implementation logic.  
It does not include full production code or private data.
