# AlphaBlog

# Cơ bản ruby 
* Tạo project mới: 
```	rails new [project_name] ```
* Tạo một migrate table mới
``` rails generate migration create_articales ```
* Thực hiện migrate 
```rake db:migrate```
* Hoàn tác migration
```rake db:rollback```
* Modify migrate 
``` rails generate migration add_description_to_articles ```