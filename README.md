# **BRlist** <img src="man/figures/BRlist.png" align="right" width="30%" min-width="120px"/>

<!-- badges: start -->

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/paulobarros/amphiBR/blob/master/LICENSE.md)
[![Twitter
Follow](https://img.shields.io/twitter/follow/pbarrosjr?color=%2315202B&label=Seguir%20%40pbarrosjr&style=social)](https://twitter.com/pbarrosjr)
[![pix](https://img.shields.io/badge/Apoie%20com-PIX-brightgreen)](https://nubank.com.br/pagar/v67wv/tuh5iRS2YJ)

<!-- badges: end -->

## Brazilian Red List of Species

This package contains datasets from the official Brazilian Endangered Species List published by the Ministério do Meio Ambiente [MMA 300/2022](https://www.in.gov.br/en/web/dou/-/portaria-gm/mma-n-300-de-13-de-dezembro-de-2022-450425464). The package provides separated datasets for Plants, Invertebrates (Land and Aquatic), Amphibians, Reptiles, Birds, Fishes and Mammals.

## Instalation

```{r}
#install.packages("devtools")

devtools::install_github('paulobarros/BRlist')

library(BRlist)
```

## Usage

Once the package is loaded the following datasets will be available:

`amphibiaBRlist`: Amphibians

`avesBRlist`: Birds

`fishesBRlist`: Fishes

`invertebratesBRlist`: Invertebrates (Terrestrial and Aquatic)

`mammaliaBRlist`: Mammals

`plantsBRlist`: Plants

`reptiliaBRlist`: Reptiles

All datasets have information on taxonomic `order`, `family` and `species`, `category` of threat and if the species was evaluated in the previous list `MMA2014`. The `invertebratesBRlist` dataset provides the additional fields `phylum` and `class`, this information is not present in the MMA 148/2022 and was added to the dataset using the package `taxsize`.

## Notes

**Please feel free to report any mistakes on the datasets.** Taxonomic classification follows the MMA 300/2022. For the Birds list I intend to incorporate the Brazilian and US common name since it is avaiable online, if anyone has this information for the other groups and want to contribute please contact me at <pbarrosbio@gmail.com>.
