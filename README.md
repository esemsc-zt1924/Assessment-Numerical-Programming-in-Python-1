# NPP Pandas Assessment

**Deadline: 4.30pm BST 11th October 2024**

## Task description

In this exercise you will use Pandas to process and analyse weather station data in mutiple files in `.csv` format into a form which is easier to work with. The assessment requires no specialist knowledge of weather data and can be completed by any EDSML/GEMS student.

The `inputs` directory contains 5 weeks of weather data recorded at three weather stations across the UK.

Each file contains the following headings
- `id`: A unique id for the data.
- `site`: The human readable site of the weather station.
- `longitude`: The longitude of the station.
- `latitude`: The latitude of the station.
- `dateTime`: The date and time for which the reading is valid.
- `airTemperature`: The recorded air temperature in degrees Celcuius.
-	`dewPoint`: The recorded dew point temperature (see definitions.ipynb) in degrees Celcius.
- `meanSeaLevelPressure`: The pressure recorded in hPa.
-	`relativeHumidity`: The relative humidity % recorded.
-	`windSpeed`: The mean wind speed in m/s.
- `windDirection`: The wind direction in degrees.
-	`windGust`: The highest 5% wind speed.
-	`visibility` Visibility on a ten point scale (0-9).

These files should not be changed. You will write code to generate new dataFrames, and may write files into an "output" directory.

### Suggested Workflow

You are strongly advised to work on either the `answer.ipynb` file or the `answer.py` file, but **not both**. Please delete the file you choose not to update using the command `git rm answer.X`, replacing `X` with `.ipynb` or `.py`.

You will receive 1 mark for deleting the file you do not use.

You may use any editor (e.g. Jupyter or VS Code), but we strongly recommend against switching between them in a single workflow.

### Submission

The entire repository should be uploaded to GitHub before the submission deadline. For this we recommend using either:
1. A `git` based GUI such as GitHub Desktop
2. The source control tab in VS Code
3. The `git` tool on the command line. If no additional files have been created, then this can be achieved by running:
  ```
  git add -u
  git commit -m "<A useful message>"
  git push -u origin main
  ```
  If you have created additional files to be submitted (e.g. additional code tests) then these should be staged using commands such as `git add test_answr.py` before committing.

  You will receive up to 2 marks for committing your work regularly (i.e. making at least 2 commits, and not too close together).

### Problem Specification

You must:

1. Write appropriate Python code to complete and implement the functions requested in `answer.ipynb`/`answer.py` (the information is identical). See the docstrings in each function for details of key functionality required. Other functions, method or classes can be added if appropriate, either in the same file, or additional ones.
2. Update the `references.md` file with any books, videos or websites you use to help you in writing this code, as well as links to any relevant Chat GPT sessions you created. For tutorial sites, the main URL will surfice. For Q&A sites (e.g. Stack Overflow/Stack Exchange) please link to the specific question. (you will receive a maximum of 3 marks for this, but it is a good habit to get into anyway).
3. use any Python modules in the [standard library](https://docs.python.org/3/library/) and any modules supplied in the course `npp2024` conda enviroment (e.g. `pandas`, `scipy`, `numpy`, `matplotlib`).

### Mark scheme

The code will be assessed in an "essay style" where partial credit is available for incomplete code. Marks will be awarded for each part of the assesment completed, independent of the other functions. The primary source of marks will be providing functionality in line with what the the docstrings asked for, with robustness (both to user error & data errors) and maintainability (with features such as clarity and ease of reading of code) also key considerations. Marks will not be significantly lost for time or memory inefficiency, unless it is particularly egregious (e.g. regularly causing your machine to crash will be penalized).

The grades will be on the UK 100 point scale:

- 50% : Pass/fail boundary. Code solves at least part of the problem, but some key functionality is still missing or incorrect.
- 60% : Pass/Merit boundary. Code solves the main problem well. Some corner cases or error handling may be missing.
- 70% : Merit/Distnction boundary. Code solves the main problem well, with some additional functionality or error handling.
- 80% : High Distinction. Code solves the main problem well, with some evidence of additional thought or effort. Reasonable thought towards error handling and corner cases.

