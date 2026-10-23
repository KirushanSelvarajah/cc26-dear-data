# Creative Coding (cc26) - Dear Data Project: Exercise Tracking

## 1. Project Overview
This repository contains the data collection and future visual design for the *Dear Data* assignment. The goal of this project is to track and log personal daily physical exercise modalities and analyze their relationship with subjective physiological and psychological states over time.

## 2. The Dataset
The data is collected daily using a hybrid workflow (on-the-go logging via mobile notes, aggregated inside Google Sheets) and exported as a clean `comma-separated values` (.csv) file. 

### Data Attributes & Types
To ensure seamless integration with the **Processing software** using `loadTable()`, data types have been strictly enforced with zero empty fields:
* `date` (String, YYYY-MM-DD) - The day of the observation.
* `activity_type` (String) - Limited to: `walk`, `cycle`, `gym`, or `rest`.
* `duration_mins` (int) - Total active execution time in minutes.
* `energy_level` (int) - Subjective energy rating scored from `1` (exhausted) to `5` (highly energetic).
* `environmental_context` (String) - Categorised as `indoor`, `outdoor`, or `none`.

## 3. Planned Processing Design Strategy
The data attributes collected above are structured to map directly onto visual properties within Processing:
* **Conditional Logic:** `activity_type` strings will determine the specific geometric shape or symbol rendered.
* **Data Mapping:** `duration_mins` integers will be passed into the `map()` function to control scale and size dynamically.
* **Color Channels:** `energy_level` metrics will dictate RGB alpha transparencies or shifting color palettes.
# cc26-dear-data
