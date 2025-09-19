# 🚀 Game Categorization 

Categorizes games our family plays, useful for learning how to code

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Build](https://img.shields.io/github/actions/workflow/status/roatanrich/andrew-learn/ci.yml)

---

## 📦 Features

- ✅ Feature 1: Finds games that a person has played
- ⚡ Feature 2: Checks when that game was last played
- 🔒 Feature 3: Shows the release date for the game
- 📝 Feature 4: Identifies the people who play each game
- 🔧 Feature 5: Identifies what people play the game on
---

## GamePlay Table Structure

| ID | GameName | GameType | Person | YearCreated | LastPlayed |
|-|-|-|-|-|-|
| 01 | Borderlands | XBox | Rich | 2009 | 2025 |
| 02 | Assassins Creed Shadows | XBox  | Rich | 2025 | 2025 |
| 03 | Risk | Board  | Andrew | 2025 | 2024 |
| 04 | Risk | Online  | Rich | 2007 | 2017 |
| 05 | Uno | Card  | Andrew | 1971 | 2024 |
| 06 | Uno | Card  | Tristan | 1971 | 2024 |
| 07 | Monopoly | Board  | Tristan | 1935 | 2024 |
| 08 | Monopoly | Board  | Andrew | 1935 | 2024 |
| 09 | Monopoly | Board  | Rich | 1935 | 2024 |
| 10 | Monopoly | Board  | Jennifer | 1935 | 2024 |

## GamePlay Table W/FK

| ID | Dim_Game_Name_ID | Dim_Game_Type_ID | Dim_Person_ID | YearCreated | LastPlayed |
|-|-|-|-|-|-|
| 01 | 1 | 1 | 2 | 2009 | 2025 |
| 02 | 2 | 1  | 2 | 2025 | 2025 |
| 03 | 3 | 2  | 1 | 2025 | 2024 |
| 04 | 3 | 3  | 2 | 2007 | 2017 |
| 05 | 4 | 4  | 1 | 1971 | 2024 |
| 06 | 4 | 4  | 3 | 1971 | 2024 |
| 07 | 5 | 2  | 3 | 1935 | 2024 |
| 08 | 5 | 2  | 1 | 1935 | 2024 |
| 09 | 5 | 2  | 2 | 1935 | 2024 |
| 10 | 5 | 2  | 4 | 1935 | 2024 |

## Game Name Dimension Table

| ID | Dim_Game_Name_ID | Game_Name |
|-|-|-|
| 01 | 1 | Borderlands |
| 02 | 2 | Assassins Creed Shadows |
| 03 | 3 | Risk |
| 04 | 4 | Uno |
| 05 | 5 | Monopoly | 

## Game Type Dimension Table

| ID | Dim_Game_Type_ID | Game_Type |
|-|-|-|
| 01 | 1 | XBOX |
| 02 | 2 | Board |
| 03 | 3 | Online |
| 04 | 4 | Card |

## Person Dimension Table

| ID | Dim_Person_ID | Person |
|-|-|-|
| 01 | 1 | Andrew |
| 02 | 2 | Rich |
| 03 | 3 | Tristan |
| 04 | 4 | Jennifer |
