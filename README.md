# daily_log
- just a tiny diary. 
- written about my daily activities like the classes in Univ.; reading papers, articles, or books..

## **Published at** [**here**](https://otsukotsu.github.io/daily_log_publish/)


## settings
### **github actions**
- build docker (`FROM rust:latest`)
- run `mdbook build`
- deploy generated files in `./book/` to [OtsuKotsu/daily_log_publish](https://github.com/OtsuKotsu/daily_log_publish)

### **structure**
```
root/
    +- src/
        +- 2021/
            +- top.md
            +- April/
                +- top.md
                :
                +- 30th.md
            +- May/
                +- top.md
                +- 1st.md
                +- 2nd.md
                :
            :
        :
        +- README.md
        +- SUMMARY.md

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
