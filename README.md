 Rolling Average SAS Code with Macro

## Overview

This repository contains SAS code for calculating rolling averages using a macro. The dataset includes variables such as height, weight, sex, and name. 
The code demonstrates how to compute rolling averages for numerical variables over a specified window using SAS macros.

## Variables

- height: The height of the individual.
- weight: The weight of the individual.
- sex: The gender of the individual (e.g., Male, Female).
- name: The name of the individual.

## Files

- rolling_average.sas: SAS code that includes the macro for calculating rolling averages.
- macro_definition.sas: Definition of the SAS macro used for rolling average calculations.

## Prerequisites

- SAS software (version X.X or later).
- A dataset with variables height, weight, sex, and name.

## Usage

1. *Prepare Your Dataset:*
   Ensure you have a dataset with the required variables (height, weight, sex, name).

2. *Include the Macro:*
   Ensure that the macro_definition.sas file is included in your SAS session to define the macro.

3. *Run the SAS Code:*
   Open the rolling_average.sas file in SAS. The script will call the macro to compute rolling averages for the specified variables.

4. *Review Results:*
   The results will be outputted to the specified dataset or log file. Review the results to ensure the rolling averages are computed correctly.

## Example

Here is an example of how to use the macro in the SAS code:

```sas
/* Include the macro definition */
%include 'path/to/macro_definition.sas';

/* Run the rolling average code */
%rolling_avg(data=your_data, var=height, window=5);
