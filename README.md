<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![LinkedIn][linkedin-shield]][linkedin-url]
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="HUDK4054.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Urban Population Analysis(1950-2050)-READM</h3>

  <p align="center">
    Looking into Global Population and Urbanization Trends!
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Report Bug</a>
    ·
    <a href="https://github.com/othneildrew/Best-README-Template/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#dataset overview and features">Dataset Overview and Features</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#models">Models</a></li>
        <li><a href="#r libraries">R Libraries</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#results and conclusion">Results and Conclusion</a></li>
    <li><a href="#data storage">Data Storage</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#References">References</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

Title: Urban Population Analysis(1950-2050) Research Project

Creator: Yifan Lei

Principal Investigator(s): Yifan Lei, Girish Chowdary, Haines City

Data Manager: Yifan Lei

ORCID iD: 0009-0006-6915-6750

DOI: https://doi.org/10.1145/3473714.3473820

Affiliation: Teachers College, Columbia University

Research Date: 02-19-2024

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Dataset Overview and Features
Dataset: [dataset.csv](https://www.kaggle.com/datasets/girishchowdary22/urban-population-analysis1950-2050?resource=download&select=dataset.csv)

File Format: csv

This table provides estimates from 1950 to 2021 and projections (medium fertility variant) from 2022 to 2050 of total population and urban population, expressed in thousands and as a percentage of total population, respectively. Population refers to de facto population in a country, area or region as of 1 July of the indicated year.

Year - This column records the years from 1950 to 2050

Economy - Represents the code of the country or region's economy that the data pertains to

Economy Label - This is the specific name or description of the economy, providing a readable label for the economy code

Absolute value in thousands - Records the total population of the economy in a specific year, in thousands

Absolute value in thousands Missing value - Indicates the cases where absolute population value data is missing, helping to identify incomplete entries in the dataset

Urban population as percentage of total population - Shows the proportion of the urban population relative to the total population, expressed as a percentage

Urban population as percentage of total population Missing value - Indicates the cases where data on the percentage of urban population is missing, used to identify records in the dataset lacking information on urbanization ratios

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
### Installation

_You need to configure the environment_

1. Install Git using Homebrew at [git](https://git-scm.com/)

   1.1 If you don’t have Homebrew, install Homebrew first.
    ```sh
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)
    ```
   1.2 Install Git using Homebrew
    ```sh
    brew install git
    ```

3. Clone the repo
   ```sh
   git clone https://github.com/YifanLei/HUDK4054.git
   ```
4. Install all packages needed
   ```sh
   packages_name install
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Models
1. **Linear Regression**
- Used to analyze the relationship between year and urban population proportion, or the growth trend of the absolute value of population.
2. **Time Series Analysis**
- Especially if you want to predict urbanization trends or population growth trends in the next few years, you can use ARIMA models, etc.
3. **Logistic Regression**
- If you want to predict whether an economy will reach a certain level of urbanization based on other variables.
4. **Cluster Analysis**
- Used to group economies based on factors such as urbanization rate, population growth, etc.



### R Libraries
In order to properly run the models, the following R libraries are used:
 ```sh
 # dplyr and tidyr - for data manipulation and cleaning
library(dplyr)
library(tidyr)

# ggplot2 - for creating visualizations like trend plots, scatter plots, etc.
library(ggplot2)

# forecast - for time series analysis and forecasting
library(forecast)

# lmtest and car - for diagnostic checking and hypothesis testing of linear regression models
library(lmtest)
library(car)

# factoextra and cluster - for performing cluster analysis and visualizing the results
library(factoextra)
library(cluster)

# caret or tidymodels - for a unified interface to train models, evaluate and compare them
library(caret)
# or
library(tidymodels)

# plm - for panel data analysis if the data structure is applicable
library(plm)

# gganimate - for creating dynamic visualizations that change over time
library(gganimate)

 ```



<!-- USAGE EXAMPLES -->
## Usage

You can see what the chart looks like and an example of the analysis here.

<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="Demo copy.png" alt="Logo" width="600" height="400">
  </a>
</div>
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="Analysis copy.png" alt="Logo" width="600" height="400">
  </a>
</div>

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish

See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- Results and Conclusion -->
## Results and Conclusion
Our comprehensive analysis of the "Urban Population Analysis (1950-2050)" dataset has yielded several key insights into global urbanization and population dynamics over a century. We observed significant trends in urban population growth, with the rate of change varying notably across different economies.

Key Findings:

A clear trend of urbanization was noted, with an increasing percentage of the global population residing in urban areas over time.
The growth patterns in urban populations showed [specific trends or anomalies], reflecting the impact of [economic developments, migration, policy changes, etc.].
[Economy or region] stood out due to its [remarkable growth rate, unique pattern, or some other noteworthy feature].

Trends:

The data revealed a [steady increase, plateau, or decline] in the urban population percentages across most economies, suggesting [possible reasons or implications].
Temporal patterns suggest that the rate of urbanization [accelerates, decelerates, remains constant] as economies develop.
Comparative Insights:

When comparing different economies, we found that [developed economies, emerging markets, specific regions] exhibited distinct characteristics in terms of their urbanization trajectories.

Predictions and Speculations:

Based on the observed data, we predict that by 2050, urban populations will [exceed, stabilize, or follow a specific trend], implying [potential outcomes or challenges].
The data suggests that [certain economies or regions] may face [specific urban challenges such as overpopulation, underdevelopment, etc.].

Potential Impacts:

These findings have critical implications for policy-making, urban planning, and sustainability efforts. They highlight the need for [targeted policies, infrastructure development, resource management, etc.].

Recommendations and Suggestions for Improvement:

Based on our findings, we recommend [specific actions or strategies] to manage the challenges of urbanization effectively.
Further research is suggested to delve deeper into the nuances of [population distribution, urban infrastructure, socio-economic factors, etc.].
As urban landscapes continue to evolve, this dataset serves as a crucial tool for understanding and navigating the complexities of population growth and urban planning. The trends observed warrant careful consideration by policymakers, urban planners, and researchers alike, as they hold the key to sustainable and equitable urban development.



<!-- Data Storage -->
## Data Storage
Data will primarily be stored as a .csv file on the computers of the researchers. For
data backups, the 3-2-1 backup rule will be followed. In addition to the data on the
researchers’ devices, every researcher will have a designated backup USB-drive where a
backup has to be stored every time the respective researcher worked with the data.
Additionally, a cloud backup on the Columbia University CUIT servers will be performed
twice a week. All researchers will not work with the original “raw” data which will be
stored once on each researcher’s computer, once on a general hard drive at the
research laboratory, once on the Columbia University CUIT servers, and once on the
online repository. Researchers are encouraged to save a new file everytime they work
with the data starting the file name by “YYYY-MM-DD…” so that one knows which file is
the newest (Broman & Woo, 2018). Public use data and associated documentation will be
made available to the research community free of charge through Open Science
Foundation (OSF) data repository.

Final submission and release of the study data will occur approximately 3 to 6 months
after the end of our data collection. Study data deposited in OSF will be available to
the research community in perpetuity.



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the Apache 2.0 open source license. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Yifan Lei - [Facebook](https://www.facebook.com/profile.php?id=100011185567211&mibextid=LQQJ4d) - yl5526@tc.columbia.edu

Project Link: [https://github.com/YifanLei/HUDK4054](https://github.com/YifanLei/HUDK4054)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- References -->
## References

Kaggle - [Urban Population Analysis(1950-2050)](https://www.kaggle.com/datasets/girishchowdary22/urban-population-analysis1950-2050?resource=download)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0)
* [UNCTAD](https://unctadstat.unctad.org/EN/)
* [Kaggle](https://www.kaggle.com/datasets/girishchowdary22/urban-population-analysis1950-2050?resource=download)
* [DCC](https://www.dcc.ac.uk/resources/subject-areas/social-science-humanities)
* [DDI](https://ddialliance.org/resources/tools)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/yifan-lei-9049a4157?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
