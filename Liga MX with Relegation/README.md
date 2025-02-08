# Liga MX with Relegation

## Introduction
This folder contains an Excel spreadsheet that simulates the Liga MX Clausura season under a hypothetical scenario where promotion and relegation were reinstated after the dissolution of the Ascenso MX league and the creation of Liga de Expansión MX.

## Explanation
After Liga de Expansión MX replaced Ascenso MX, promotion and relegation were suspended. This spreadsheet reintroduces the system by analyzing each season since the change and determining which teams should have been relegated and promoted based on historical real life performance.

### Promotion and Relegation System:
- **Promotion:**
  - The **Clausura** and **Apertura** champions of Liga de Expansión MX are promoted directly.
  - The **Runner up teams** in both the Liga de Expansión MX clausura and apertura finals play a match.
  - The winner of this match competes against the **third-lowest team in the Liga MX coefficient table** for the final promotion spot.

- **Relegation:**
  - The **bottom three teams in the Liga MX coefficient table** are at risk of relegation instead of mearly being monetarily penalized.
      - The **two lowest-ranked teams** are directly relegated.
      - The **third-lowest team** faces the playoff winner from Liga de Expansión MX for survival.

This approach ensures that teams perform competitively and rewards strong performances in the second division while maintaining a pathway for promotion.

## Data and Methodology
- The spreadsheet includes detailed calculations of past seasons, ensuring that the correct teams were promoted and relegated based on their their historic real life standings and performances since 2020 for both the Liga MX and Liga de Expansión MX .
- Coefficient rankings and league structures were carefully considered to create a realistic relegation and promotion system. In reality, the bottom three teams in Liga MX are only subjected to financial penalties rather than relegation, making it possible for the same team to finish in the bottom three across multiple consecutive seasons. In such cases, the simulation enforced relegation, with the newly promoted team from Liga de Expansión being relegated instead if their predecessor in Liga MX had already been relegated in the previous season.
    - For example, if Atlético San Luis finished last in both the Clausura and Apertura seasons in real life, the simulation would relegate them after the Apertura. The Liga de Expansión team that replaced them for the Clausura would then be relegated in the Apertura instead. The replacements were mapped according to the Clausura or Apertura seasons. If Atlético San Luis was relegated in the Apertura and Toluca in the Clausura, and Atlante and Cancún were promoted for the Apertura and Clausura respectively, then Atlante would be the team relegated for the clausura season.

### Included Data Fields:
Each club in Liga MX and Liga de Expansión MX is detailed with the following attributes:
- **Club Name** – The official name of the club.
- **Location (City)** – The city where the club is based.
- **Stadium** – The name of the club's home stadium.
- **Capacity** – The seating capacity of the stadium.
- **Value (in Euros)** – The estimated market value of the club.
- **Titles** – The number of championships won by the club.

This analysis provides insight into how Liga MX could have evolved if promotion and relegation had never been abolished.







