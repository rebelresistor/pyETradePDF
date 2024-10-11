# pyETradePDF

This tool is a generic parser to convert the PDFs downloaded from the E-Trade website into a usable CSV format. 
This is primarily a tool to help you do your taxes! 

Supported PDFs are:

* Trade Confirmations
	* **Accounts** > **Documents** > **Documents & Statements** > **Trade Confirmations**
* RSU and ESPP Confirmations
	* **Stock Plan** > **My Account** > **Stock Plan Confirmations**

## Getting Started

As of Python 3.12, you should install all packages in their own virtual environments.

```bash
# create a new virtual environment to install pyETradePDF
python3 -m venv venv

# activate the virtual environment
source venv/bin/activate

# install
pip install git+https://github.com/rebelresistor/pyETradePDF

# test
etradepdf
```

Each time you want to use `etradepdf`, you must activate the virtual environment by running the `source` command above again. 

### Installation for Developers

This installation method is only for people who want to build extra functionality for pyETradePDF.

Firstly, fork this project, and then `git clone` your URL in place of this repo below:

```bash
git clone git@github.com:rebelresistor/pyETradePDF.git
cd pyETradePDF
python3 -m venv devenv
source devenv/bin/activate
pip install -e .
```

If everything above worked, you should be able to run `etradepdf` as above and see the help message.
