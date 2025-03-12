# Scrapy Commands:

## Initiate a project

```sh
scrapy startproject <project_name>

```

#### Scafolds a project with the name **project_name**

- Create a spyder in the **project_name/spiders** folder
- Run the spyder using:

```sh
scrapy crawl <spider_name>
```

## Scrapy from the Shell

```sh
> > > scrapy shell "https://www.amazon.in/gp/bestsellers/watches/ref=zg_bs_watches_sm"
> > > response
> > > [gives an OK response]
> > > products = response.css('div.\_cDEzb_grid-column_2hIsc') ## returns all the products
> > > len(products)
> > > [gives the number of products]

###Name of product(s)

> > > products.css('div.\_cDEzb_p13n-sc-css-line-clamp-3_g3dy1::text').get()
> > > products.css('div.\_cDEzb_p13n-sc-css-line-clamp-3_g3dy1::text').getall()

###Price of product(s)
```
