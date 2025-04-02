# TerneraShop
Demo for the two parts of a web store

## Back SpringBoot+JPA+PostgreSQL
 - [x] Connected to db
 - [x] openapi for documentation. Swagger UI: "/" , json: "/api-docs"
    
 - [x] product and vendor endpoints
 - [ ] ManyToOne product to vendor 
 - [ ] payment endpoints
 - [ ] buyer endpoints
 - [ ] cors config, currently bypassed
 - [ ] Hibernate validation

Runs with 
`"back\mvnw.cmd" spring-boot:run -f "back\pom.xml"`

In development uses `http://localhost:8080`

More specifics in [./back/README.md](./back/README.md)

## Front Angular
 - [x] Product catalog
 - [x] consume the product api
 - [x] shopping cart
 - [x] check back server health
 - [x] show errors in toasts
 - [ ] payment (pending)

Runs with 
`"npm run dev --prefix front/`
where `dev` corresponds with `"dev": "ng dev --host=0.0.0.0"` in  [package.json](./front/package.json)

In development uses `http://localhost:4200`

More specifics in [./front/README.md](./front/README.md)