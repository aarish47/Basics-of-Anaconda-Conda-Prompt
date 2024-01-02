## **Explore the Fundamentals of Conda: A Beginner's Guide**
### **Written by: Dr. Aarish Khan**
### **Date: 2nd January 2024**

## **Introduction to Anaconda Navivagtor:**

#### Anaconda Navigator serves as a visual interface for utilizing conda, a package manager. To launch Navigator, simply double-click the desktop icon, or in a Terminal or Anaconda prompt, enter the command: anaconda-navigator.

> Conda basics:
* Verify conda is installed, check version number:\
**conda info**

* Command line help:\
**COMMANDNAME --help**\
**conda install --help**

# **Fundamentals:**

> How to activate base?

#### (base) C:\Users\Administrator> **conda activate conda**

This command is used to switch from one environment to another in the Anaconda distribution. The "conda" keyword refers to the use of Anaconda

> What does conda env list mean?

#### (base) C:\Users\Administrator> **conda env list**

This command is used to display a list of all the environments that have been created using conda. It shows the name of each environment

> How to remove env from conda prompt?

#### (base) C:\Users\Administrator> **conda env remove -n (name of env)**

To delete a specific environment, use the following command followed by the name of your environment

> How to create an enviroment?

#### (base) C:\Users\Administrator> **conda create -n my_env**

To create a new environment named "my_env", you would type in the following code into the terminal or Anaconda Prompt

> How to install a package in the active enviroment "my_env"?

#### (base) C:\Users\Administrator> **cd my_env**

First you will need to change directories and you can do that by applying this code

Now, to install a package you will use this code below:

#### (my_env) C:\Users\Administrator> **pip install (package-name)**

> How to run an installed package?

#### (my_env) C:\Users\Administrator> **(package-name)**

You just have to put in the name of the package that you just installed, for example:

I installed jupyter and now to run jupyter notebook I'll write this code:

#### (my_env) C:\Users\Administrator> **jupyter-notebook**

> How to update a package?

#### (base) C:\Users\Administrator> **conda update (package name)**

In order to get the latest version of the package that you installed, just write "conda update" and then the name of your package like scikit-learn

Make sure you don't add the paranthesis which i added it's just to tell you that you need to write your package name

> How to remove one or more than one packages in specific environment?

(my_env) C:\Users\Administrator> **conda remove --name (package name)**

This is how you can remove a package from an environment that you created, you just have to type in: "conda remove --name" and further the name of the package

# How to manage the multiple verison of Python

**Managing multiple versions of Python**

* Install different version of Python in 
a new environment named py34:\
**conda create --name py34 python=3.4**

* Switch to the new environment that has a different version of Python:\
  **activate py34**

* Display the paths of all existing Python versions currently included in the system's environment variables:\
 **where python**

# Basic and simple fundamentals used in conda

* Make exact copy of an environment:\
  **conda create --clone py34 --name py34-2**

* List all packages and versions installed in active environment:\
**conda list**

* List the history of each change to the current environment
**conda list --revisions**

* Restore environment to a previous revision:\
**conda install --revision 2**

* Save environment to a text file:\
**conda list --explicit > bio-env.txt**

* Delete an environment and everything in it:\
**conda env remove --name bio-env**

* Deactivate the current environment:\
**conda deactivate**

* Create environment from a text file:\
**conda env create --file bio-env.txt**

* Stack commands: create a new environment, name 
it and install the package:\
**conda create --name bio-env biopython**

# Finding packages in Conda

* Use conda to search for a package:\
**conda search (packagename)**

* See list of all packages in Anaconda:\
**https://docs.anaconda.com/free/anaconda/packages/pkg-docs**

# Specifying version numbers

* Constraint type:\
**Fuzzy**\
**Exact**\
**Greater than or equal to**\
**OR**\
**AND**

* Specification:\
**numpy=1.11**\
**numpy==1.11**\
**numpy>=1.11**\
**numpy=1.11.1|1.11.3**\
**numpy>=1.8,<2**

* Result:\
**1.11.0, 1.11.1, 1.11.2, 1.11.18 etc.**\
**1.11.0**\
**1.11.0 or higher**\
**1.11.1, 1.11.3**
**1.8, 1.9, not 2.0**


# Other resources to Learn from

 > **Free Community Support**\
**groups.google.com/a/continuum.io/forum/#!forum/conda**

> **Online Documentation**\
**conda.io/docs**

> **Command Reference**\
**conda.io/docs/commands**

> **Paid Support Options**\
**anaconda.com/support**

> **Anaconda Onsite Training Courses**\
**anaconda.com/training**

> **Anaconda Consulting Services**\
**anaconda.com/consulting**
