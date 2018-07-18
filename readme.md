### Installation

1. Clone repo

2. Change to directory

````
cd minions-demo
````   

3. Install dependencies

````
composer install
````

4. Copy .env file

```
cp .env.example .env
```

5. Modify `DB_*` value in `.env` with your database config.

6. Generate application key:

````
php artisan key:generate
````

7. Migrate
````
php artisan migrate
````

8. Install Node modules
````
npm install
````

9. Build

````
npm run dev
````

### Dummy Data

1. Open Tinker

````
php artisan tinker
````
    
2. Use factory script
````
factory(App\Crud::class, 3)->create();
