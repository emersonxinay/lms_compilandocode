# LMS compilandocode

## Recordar los pasos 
crear el proyecto que incluya base de datos postgresql 
```bash
rails new nombre_proyecto --database=postgresql --css tailwind 
```
creando la base de datos
```bash
rails db:create
```
migrar la base de datos 
```bash
rails db:migrate
```
levantar el proyecto
```bash
rails s 
``` 

# Para instalar devise 
desde el archivo gemfile
```bash
gem "devise", "~> 4.9"
```
Actualizando las gemas
```bash
bundle install
```
ahora instalando devise
```bash
rails g devise:install
```
para que se muestre codigo de devise
```bash
rails g devise:views
```
generar devise para usuario
```bash
rails g devise User
```
generar devise para Admin
```bash
rails g devise Admin
```
migrando las tablas generados por devise 
```bash
rails db:migrate
```





# para generar los modelos y vistas con scaffold 
```bash
rails g scaffold Course title:string description:string
```

# Para abrir la consola de rails 
```bash
rails c 
```
para crear un usuario en la tabla Admin 
```rails c
Admin.create!(email: "admin@example.com", password: "password")
```
# Para precompilar los assets y funcione tailwind o extras cargas 
Para local
```bash
rails assets:precompile
```
Para producción
```bash
RAILS_ENV=production bundle exec rails assets:precompile
```



