# daily_log
- just a tiny diary. 
- written about my daily activities like the classes in Univ.; reading papers, articles, or books..

## **Published at** [**Here**](https://otsukotsu.github.io/daily_log_publish/)
- use github pages

### How is this page generated ?
- use **mdBook** to generate html, css, js
- published with [**GitHub Pages**](https://docs.github.com/en/pages)
- leverage [**GitHub Actions**](https://github.com/features/actions) to reflect the changes to published web page (see following section)  
    　  
  <img src="./src/img_folder/github_actions.png" alt="github_actions" width="100"/>  

- customize a little by myself  
  the patterns in the background is drawn on my own  
    
  ![my-favicon](./src/img_folder/favicon.png)  

## **github actions**
- ~~build docker (`FROM rust:latest`)~~
- ~~run `mdbook build`~~
- install mdBook v0.4.8 from release page of mdBook.  
  This is because mdBook v0.1.4~v0.4.4 has cross site scripting vulnerability.
  - see [here](https://blog.rust-lang.org/2021/01/04/mdbook-security-advisory.html)  
    and [CVE-2020-26297](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-26297)  
    and [security advisory in mdbook repository](https://github.com/rust-lang/mdBook/security/advisories/GHSA-gx5w-rrhp-f436)
- deploy the files generated in `./book/` into [**OtsuKotsu/daily_log_publish**](https://github.com/OtsuKotsu/daily_log_publish)

## **structure**
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
        +- 404.md

    +- theme/
        +- css/
        +- img_folder/
        +- favicon.png
        +- favicon.svg

    +- book.toml
    +- .github/
        +- workflows/
            +- main.yml

    +- .vscode/
        +- *.code-snippets

    +- README.md
    +- .gitignore

```
