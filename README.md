# Creating yml and ENV

## Prerequisites:
You need to have any python text editors. I am suggesting the sublime. Also, you need to install conda on your computer.

## Introduction

This repo contains all you need to create the yml file and convert it to a conda env file.  

## Creating the .yml file:
- Download the [sample_env_1.yml](https://github.com/MehdiMahmoodi/ENV_with_yml/blob/main/sample_env_1.yml)
- Use sublime to open the downloaded sample.yml        
- Add the required libraries to the "dependencies":
        -   Removing any of the packages in the sample_env.yml file is not recommended.
        -   You can find the last version of libraries in [pypi.org](https://pypi.org/). As an example for [numpy](https://pypi.org/project/numpy/)
        -   If you are using the sublime, you can take advantage of highlighting the desire columns(all columns if you want) then Ctrl+Shift+l . It would help you for arrangmenting the text.
  
- Save your .yml file in the desirede location:
    -   Do not forget to update the name: in the .yml file
    -   Save the file like: chooseaname.yml (do not forget to save it as    .yml    file) 

## Creating the conda environment by use of .yml 
-   Open the Anaconda Prompt
-   Navigate to the address where you saved the .yml file.
        -   cd address
-   try to create a conda environment by writing the following command:
-       conda env create -f sample_env_1.yml
-   use tap for auto complete

## Troubleshooting:
-   Most probably you would get an error like: "ResolvePackageNotFound:". It is mostly happening whenever you want to install the most updated version. In this case, you need to:
        -   get back to the sublime
        -   open the .yml file again
        -   cut the packages mentioned below the “ResolvePackageNotFound:" from the "dependencies:" and past it under "- pip:"
        -   As an example compare the [sample_env_1.yml](https://github.com/MehdiMahmoodi/ENV_with_yml/blob/main/sample_env_1.yml) with [sample_env.yml](https://github.com/MehdiMahmoodi/ENV_with_yml/blob/main/sample_env.yml)
    -   close the Anaconda Prompt and reopen it again
    -   Navigate to the address where you saved the .yml file.
        -   cd address
    -   try to create a conda environment by writing the following command:
        conda env create -f sample_en.yml
    -   use tap for auto complete.
## Activating/Deactivating the environment:
Now, you can be at any location, your command prompt to activate or deactivate.You no longer need to CD into the location where the .yml created.
just run the Anaconda Prompt and type:
                -       conda activate sample_env.yml
For deactivating, just simply type:
        -              conda deactivate sample_env.yml 
## Removing a environment:
-       conda remove --name myenv --all
-       conda info --envs
# Have Fun!!
