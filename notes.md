1. Project - 
      string :title 
      integer :user_id 

    belongs_to :user 
    has_many :tasks

    Need a database - generate resource

2. Task - 
      string :name 
      string :description
      date :schedule_start
      date :due_date
      images
      attach files
      integer :project_id 
    
    belongs_to :project

3. Cards
    integer :position
    integer :list_id 
    string :name 

    has_many :lists 


4. Lists
    string :name 
    integer :position 

    belongs_to :card
    