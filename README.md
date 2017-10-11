
# Phần 1: Migration ([Link tham khảo)](http://guides.rubyonrails.org/active_record_migrations.html) 
Tạo project mới: 

```	rails new [project_name] ```

Tạo một migrate table mới:

``` rails generate migration create_articales ```

Thực hiện migrate 

```rake db:migrate```

Hoàn tác migration

```rake db:rollback```

Modify migrate 

Cách 1:

``` rails generate migration add_description_to_articles ```

Sau đó thêm cột theo như sau:
```ruby
    class AddPartNumberToProducts < ActiveRecord::Migration[5.0]
      def change
        add_column :products, :part_number, :string
      end
```
Cách 2: 

```rails generate migration AddPartNumberToProducts part_number:string```
