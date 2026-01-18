# Building a portfolio
we will use mkdocs to build a portfolio website. Mkdocs is a static site generator that's geared towards project documentation. It is written in Python and uses the Jinja2 template engine. Mkdocs is easy to install and use, and it has a simple configuration file format.

Link to the official mkdocs documentation: [here](https://www.mkdocs.org/getting-started/)

## 1_Install mkdocs
To install mkdocs, you need to have Python installed on your system. You can check if Python is installed by running the following command in your terminal or command prompt:

```bash
conda create -n mkdocs python=3.12 -y
conda activate mkdocs
pip install mkdocs
```

## 2_Create a new mkdocs project
To create a new mkdocs project, run the following command in your terminal or command prompt:

```bash
mkdocs new Muhammad-Usman-portfolio
cd Muhammad-Usman-portfolio
```
This will create a new directory called `Muhammad-Usman-portfolio` with the following structure:

```Muhammad-Usman-portfolio/
    mkdocs.yml # The configuration file.
    docs/
        index.md # The home page of your site
```

## 3_Run the mkdocs development server
To run the mkdocs development server, navigate to the project directory and run the following command:

```bash
mkdocs serve
```
this is how can specify the port and host

```bash
mkdocs serve -a 127.0.0.1:9377
```


## 4_Build the project
To build the mkdocs project, run the following command in your terminal or command prompt:

```bash
mkdocs build
```

## theme
You can change the theme of your mkdocs site by editing the `mkdocs.yml` file. For example, to use the "readthedocs" theme, you can add the following lines to your `mkdocs.yml` file:

```bash
pip install mkdocs-material
theme:
  name: readthedocs
```
You can find a list of available themes in the [mkdocs documentation](https://www.mkdocs.org/user-guide/styling-your-docs/#built-in-themes).

## 5_Deploy the project
To deploy the mkdocs project, you can use GitHub Pages. First, you need to create a new repository on GitHub. Then, run the following command in your terminal or command prompt:

```bash
mkdocs gh-deploy
```
link of my portfolio: [here](https://muhammad-usman.github.io/Muhammad-Usman-portfolio/)


## 6_upload to github
To upload your mkdocs project to GitHub, you need to initialize a git repository in your project directory. Run the following commands in your terminal or command prompt:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin[ https://github.com/Usman9377/My-Portfolio.git](https://github.com/Usman9377/My-Portfolio.git)
git push -u origin main
```
Replace `yourusername` and `your-repo-name` with your GitHub username and the name of your repository, respectively.
This will upload your mkdocs project to GitHub. You can then use GitHub Pages to host your mkdocs site.
de
```bash 
pip install mkdocs-git-revision-date-localized-plugin mkdocs-material mkdocs-material-extensions mkdocs-git-authors-plugin
```
then run 
```bash
This is my portfolio link, https://usman9377.github.io/My-Portfolio/
mkdocs github-deploy
```
