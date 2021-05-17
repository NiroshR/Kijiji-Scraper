# Kijiji-Scraper 3.0.1

A Kijiji Scraper used for finding Yamaha WR450F engines for the 
University of Waterloo Formula Motorsport's (UWFM) 2022 season.
The [original code](https://github.com/CRutkowski/Kijiji-Scraper)
 was created by [Chase Rutkowski](https://github.com/CRutkowski)
who did a great job making a general purpose tool for scraping
Kijiji for ads. This repo will help UWFM members quickly get
setup and running to find potential engines.

## Install

### Intalling Pip package manager

You will need to have a few components installed before starting to use this project

- MacOS: [Brew Package Manager](https://brew.sh)
- Linux: `sudo apt install python3-pip`
- [Python 3](https://docs.python-guide.org/starting/install3/osx/)
- You will need to install `pip3` to get python packages
- `pip3 install virtualenv`

Once you have these prerequisites, you can build the project and run the web scraper.

### Cloning the repo
   ```bash
   git clone https://github.com/NiroshR/Kijiji-Scraper.git
   cd Kijiji-Scraper
   ```

### Creating the virtual environment

Run this everytime you want to run the project, it will allow you
to run the code in its own contained environment that will help in 
managing multiple package versions and version conflicts.

   ```bash
   # To activate environment
   python3 -m venv env && \
   source env/bin/activate && \
   pip3 install -r requirements.txt

   # To deactivate environment
   deactivate
   ```

### Install the package 
   ```bash
   python3 setup.py install
   ```


## Try it out!
For instance `kijiji --url https://www.kijiji.ca/b-kitchener-waterloo/wr450f/k0l1700212?ll=43.464258%2C-80.520410&address=Waterloo%2C+ON&radius=435.0&dc=true`. The scraper will
output all the links for relevant ads as well as show the location of the files
it saves to disk.
