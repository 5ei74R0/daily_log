# daily_log
- just a tiny diary. 
- written about my daily activities like the classes in Univ.; reading papers, articles, or books..

## **Published at** [**here**](https://otsukotsu.github.io/daily_log_publish/)
- use github pages

### **github actions**
- build docker (`FROM rust:latest`)
- run `mdbook build`
- deploy the files generated in `./book/` into [OtsuKotsu/daily_log_publish](https://github.com/OtsuKotsu/daily_log_publish)

### **structure**
```
root/
    +- src/
        +- img_folder/
        +- 2021/
            +- img_folder/
            +- top.md
            +- April/
                +- img_folder/
                +- top.md
                :
                +- 30th.md
            +- May/
                +- img_folder/
                +- top.md
                +- 1st.md
                +- 2nd.md
                :
            :
        :
        +- README.md
        +- SUMMARY.md

    +- theme/
        +- css/
        +- img_folder/
        +- favicon.png
        +- favicon.svg

    +- book.toml
    +- .github/
        +- actions/
            +- build/
                +- Dockerfile
        +- workflows/
            +- main.yml

    +- .vscode/
        +- *.code-snippets

    +- README.md
    +- .gitignore

```
