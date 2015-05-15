(rake db:drop) if already connected to a db 
rake db:create 

rake db:create_migration NAME=create_questions 
---make tables in migration files-----
rake db:create_migration NAME=create_lists 
---make tables in migration files-----
rake db:create_migration NAME=add_four_choices_to_questions 
---make tables in migration files-----
rake db:create_migration NAME=remove_correct_answer_from_questions 
---make tables in migration files-----
rake db:create_migration NAME=results 
---make tables in migration files-----
rake db:create_migration NAME=add_surveyid_to_results 
---make tables in migration files-----


after all migrations run:
rake db:migrate rake db:test:prepare

