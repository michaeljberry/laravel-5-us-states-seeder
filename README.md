***This is to help simplify the creation of static state names and codes within a `State` table. Changed the 50+ `State::create` method calls from ggoforth's original repo into an array of states with a single `State::insert` call. It's an easy enough change to make on your own, but now you don't have to.***

#Laravel 5 State Seeder

**Usage**

```bash
$ php artisan make:model State
```

This will generate the model and migration for your database.  In your migration you need to include `string` fields for `code` and `name`.  Then simply drop the `StatesSeeder.php` into your `seeds` folder.  Back at the command line run:

```bash
$ php artisan migrate
$ php artisan db:seed
```

You'll now have a functional States database suitable for populating drop downs or whatever else you crazy kids do with your states tables.
