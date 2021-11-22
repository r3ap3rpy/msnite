### Migrations

This allows you to prepare the python script which would create the specified table in your masonite sql database.

For example we would like to create a **posts** table we have to issue the following command.

``` bash
craft migration create_posts_table --create posts
```

Now we have a new file under **databases/migrations/create_posts_table.py**

Lets add some stuff to the skeleton.

``` bash
def up(self):
    with self.schema.create('posts') as table:
            table.string('post_type')
            table.string('post_category')
            table.string('post_body')
```

Now we can make the changes live, or rather apply them to our schema.

``` bash
craft migrate
```