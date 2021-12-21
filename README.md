# Creating yml and ENV

## Prerequisites:
You need to have any python text editors. I am suggesting the sublime. Also, you need to install conda on your computer.

## Introduction

This repo contains all you need to create the yml file and convert it to a conda env file.  

## Creating the .yml file:
- Download the [sample_env.yml](https://github.com/1)
- Use sublime to open the downloaded sample.yml 
- Add the required libraries to the "dependencies":
        -   Removing any of the packages in the sample_env.yml file is not recommended.
        -   You can find the last version of libraries in [pypi.org](https://pypi.org/). As an example for [numpy](https://pypi.org/project/numpy/)
- Save your .yml file in the desirede location:
        -   Do not forget to update the name: in the .yml file
        -   save the file like: chooseaname.yml (do not forget to put the .yml on the naming part)  

    -   

## Creating the conda environment by use of .yml 

    -   Open the Anaconda Prompt
    -   Navigate to the address where you saved the .yml file.
        -   cd address
    -   try to create a conda environment by writing the following command:
        conda env create -f chooseaname.yml
    -   use tap for auto complete

## Troubleshooting:
    -   Most probably you would get an error like: "ResolvePackageNotFound:". It is mostly happening whenever you want to install the most updated version. In this case, you need to:
        -   get back to the sublime
        -   open the .yml file again
        -   cut the packages mentioned below the “ResolvePackageNotFound:" from the "dependencies:" and past it under "- pip:"
    -   close the Anaconda Prompt and reopen it again
    -   Navigate to the address where you saved the .yml file.
        -   cd address
    -   try to create a conda environment by writing the following command:
        conda env create -f chooseaname.yml
    -   use tap for auto complete.
# Have Fun!!
