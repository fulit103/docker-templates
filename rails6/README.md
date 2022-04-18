https://docs.docker.com/samples/rails/


docker-compose run --no-deps web rails new . --force --database=postgresql 
docker-compose run --no-deps web rails new . --force --database=postgresql && rails webpacker:install

docker-compose run web rails webpacker:install

adapter: postgresql
  encoding: unicode
  host: db
  username: root
  password: colombia
  pool: 5

docker-compose build

docker-compose run web rake db:create

