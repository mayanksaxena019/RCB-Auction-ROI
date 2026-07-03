# Data Challenges & Assumptions

## Why the Analysis Starts from 2016

   Although IPL auction data exists before 2016, the player performance dataset used in this project contains season-wise statistics only from 2016 onwards. Since ROI analysis requires matching auction expenditure with player performance from the same season, auctions prior to 2016 were excluded to maintain consistency and avoid incomplete comparisons.

## Player Name Standardization

   The auction dataset and player performance dataset used different naming conventions. Several player names required manual mapping before merging.

   Examples include:

   | Auction Dataset | Performance Dataset |
   |-----------------|---------------------|
   | AB de Villiers | AB De Villiers |
   | Chris Morris | Christopher Morris |
   | Tim David | Timothy David |

   Additional player names were also manually standardized wherever inconsistencies were found.

   Manual mappings were created to ensure every player's auction record matched the corresponding performance record.

## Team Name Standardization

   Some franchises changed names during the IPL.

   For consistency across datasets, historical franchise names were standardized:

   - Delhi Daredevils → Delhi Capitals
   - Kings XI Punjab → Punjab Kings
   - Royal Challengers Bangalore → Royal Challengers Bengaluru

## Duplicate Player Purchases

   Several players were bought by RCB in multiple auction years.

   Instead of treating them as one player, each auction purchase was considered an independent    investment.

   Example:

   | Player | Auction Year |
   |---------|--------------|
   | Josh Hazlewood | 2022 |
   | Josh Hazlewood | 2025 |

   This allowed the dashboard to compare investments made across different seasons.

## Performance Matching

   Player statistics were merged using a composite key consisting of:
   - Player Name
   - Auction Year

   This ensured that each auction investment was matched with the player's performance from the corresponding IPL season.

## Custom Value Score
  
   A custom Value Score was designed to estimate a player's return on investment by combining batting performance, bowling performance, economy rate (where applicable), and auction expenditure. The metric was created solely for analytical comparison and is not an official cricket statistic.

## Missing Values

   Rows with missing auction or player information were cleaned or standardized before analysis to avoid inaccurate KPIs and visualizations.

## Data Validation

   After merging the datasets, the following validation steps were performed:

   - Verified player counts
   - Checked for duplicate records
   - Cross-validated auction expenditure totals
   - Randomly inspected player records to ensure accurate merges

## Limitations

   - The analysis is limited to Royal Challengers Bengaluru (RCB).
   - ROI is based on available player statistics and auction expenditure.
   - Factors such as injuries, leadership, fielding performance, and team strategy are not included.
   - The custom Value Score is intended as an analytical metric and should not be interpreted as an official cricket performance metric.