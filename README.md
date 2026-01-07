### **Project Execution Guide: Bayesian Lynx-Hare Inference Analysis**

#### **Step A: Software Installation**

1. **R & RStudio:** Install [R](https://cran.r-project.org/) and [RStudio](https://posit.co/download/rstudio-desktop/).
2. **C++ Compiler:** Necessary for Stan:
* **Windows:** Install [RTools](https://cran.r-project.org/bin/windows/Rtools/).
* **Mac:** Install **Xcode** from the App Store.

#### **Step B: Folder Setup**

Ensure the following files are in the same folder:

* `analysis.R`
* `lotka_volterra.stan`
* `hudson-bay-lynx-hare.csv`

#### **Step C: Library Initialization**

Open RStudio and run these in the Console:

1. `install.packages(c("tidyverse", "posterior", "bayesplot", "gridExtra"))`
2. `install.packages("cmdstanr", repos = c("https://mc-stan.org/r-packages/", getOption("repos")))`
3. `library(cmdstanr); install_cmdstan()`

#### **Step D: Opening the Project**

1. In RStudio, go to **File > New Project**.
2. Select **Existing Directory**.
3. Browse and select the folder containing the project files, then click **Create Project**.
*(RStudio will now automatically know exactly where all your files are located).*

#### **Step E: Running the Analysis**

1. In the **Files** tab, click on `analysis.R` to open it.
2. Click the **Source** button on top right of the script window.
