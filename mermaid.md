```{mermaid}
flowchart LR

A(数据分析) --> R(R语言)
R -->|数据采集| web(网络爬虫) --> html(HTML,CSS,JavaScript) == Pandoc ==> result
R -->|版本控制| github(GitHub) --> md
R -->|可重复报告| rmd(rmd/qmd) -->|knitr| md(((markdown)))
zotero(Zotero) -->|文献管理| rmd
md == Pandoc ==> result(Word,PDF,PPT,Blog,etc)
R -->|大数据| SQL(SQL) --> D(并行计算)

style D fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
```
