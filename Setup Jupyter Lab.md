# Setup Jupyter Lab

# Install python

Go to [python](https://www.python.org/downloads/)

# Install Jupyter Lab

1. **Install Jupyterlab**
    
    With pip3
    
    ```bash
    pip3 install jupyterlab
    ```
    
    With brew(for macOS)
    
    ```bash
    brew install --cask jupyterlab
    ```
    
2. **Run Jupyterlab**
    
    ```bash
    jupyter lab
    ```
    

# Install and use Virtualenv

1. Install Virtualenv
    
    ```bash
    pip3 install virtualenv
    ```
    
2. Create Virtual Environment
    
    ```bash
    virtualenv environment-name
    ```
    
3. Activate Virtual Environment
    
     In macOS or Linux
    
    ```bash
    source environment-name/bin/activate
    ```
    
    In Windows
    
    ```bash
    .\environment-name\Scripts\activate
    ```
    
4. Leave Virtual Environment
    
    ```bash
    deactivate
    ```
    

# Add environment to Jupyter

**Inside the environment you want to add, type:**

```bash
pip3 install ipykernel
```

```bash
python3 -m ipykernel install --user --name=environment-name
```

# More about Kernels

**If you want to see all installed kernels in jupyterlab**

```bash
jupyter kernelspec list
```

**If you want to remove a kernel from jupyterlab**

```bash
jupyter kernelspec uninstall environment-name
```

# Appendix

## Install Homebrew(For macOS)

1. **Install XCode Command Line Tools**
    
    ```bash
    xcode-select --install
    ```
    
2. ****Verify Installation and Environment Path****
    
    ```bash
    xcode-select -p
    ```
    
    **Note:** If the shell echos an environment path to “CommaldLineTools,” it means you can now install and open python. If not, you need to install Xcode again.
    
3. ****Install Homebrew****
    
    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
    
    **Source**: [Hombrew](https://brew.sh/)
    
4. **Run the steps to add Homebrew to your PATH**
    
    Example
    
    ```bash
    echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/christopherromanjaimes/.zprofile
    ```
    
    ```bash
    eval "$(/opt/homebrew/bin/brew shellenv)"
    ```
    

## **Notes about Homebrew**

Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple's operating system, macOS, as well as Linux. The name is intended to suggest the idea of building software on the Mac depending on the user's taste. 

While OS X comes with a large number of Unix utilities, those familiar with Linux systems will notice one key component missing: a package manager. [**Homebrew**](https://brew.sh/) fills this void. Also it is known as **The Missing Package Manager for macOS (or Linux).**

If you want to search packages by name, you can type:

```bash
brew search jupyter
```

# Sources

- [https://www.macdentro.com/install-jupyter-notebook-mac/](https://www.macdentro.com/install-jupyter-notebook-mac/)
- [https://sourabhbajaj.com/mac-setup/Python/virtualenv.html](https://sourabhbajaj.com/mac-setup/Python/virtualenv.html)
- [https://www.linkedin.com/pulse/how-use-virtual-environment-inside-jupyter-lab-sina-khoshgoftar](https://www.linkedin.com/pulse/how-use-virtual-environment-inside-jupyter-lab-sina-khoshgoftar)
- [https://mattgosden.medium.com/set-up-your-mac-for-python-and-jupyter-using-virtual-environments-730bf2888e05](https://mattgosden.medium.com/set-up-your-mac-for-python-and-jupyter-using-virtual-environments-730bf2888e05)