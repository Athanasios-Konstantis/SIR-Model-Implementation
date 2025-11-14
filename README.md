# SIR Model Implementation

*A hands-on implementation of the classic SIR (Susceptible-Infected-Recovered) epidemic model in Python via Jupyter Notebook.*

## Overview

This project provides an interactive notebook that:

- Implements the SIR model dynamics (susceptible → infected → recovered)

- Demonstrates how the infection spreads over time and how model parameters affect outcomes

- Visualises the results with plots, making it easy to experiment and learn

## Features

- A clear, commented Jupyter Notebook (SIRModel.ipynb) showing each step of setup, solution, and visualisation

- Adjustable parameters for infection rate, recovery rate, population size, initial conditions

- Graphical output to illustrate how changing parameters alters the epidemic curve

- Built with accessibility and education in mind – ideal for students or those learning epidemiological models

## Prerequisites

- Python (version 3.x recommended)

- Jupyter Notebook environment

- Recommended packages: `numpy`, `matplotlib`, `scipy`

## How it Works

* The SIR model divides the total population into three compartments:

    - **S** = susceptible (can catch an infection) 
    - **I** = infected (currently infectious)
    - **R** = recovered (and immune)

* The model is governed by differential equations:

``` $\dfrac{d\boldsymbol{S}}{dt} = - \beta \dfrac{\boldsymbol{S}\boldsymbol{I}}{N}, \;\;\; \dfrac{d \boldsymbol{I}}{dt} = \beta \dfrac{\boldsymbol{S}\boldsymbol{I}}{N} = \gamma \boldsymbol{I}, \;\;\; \dfrac{d \boldsymbol{R}}{dt} = \gamma \boldsymbol{I}$```

where: 

    - ```$ \beta $```