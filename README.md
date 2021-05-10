# README

###< テーブル設計 >

####1. Userモデル

|column	  |type	 |association|index|
|---------|------|-----------|-----|
|user_name|string|has_many   |tasks|	
####2. Taskモデル

|column  |type   |association    |index|
|--------|-------|---------------|-----|
|title   |string |	             |     |
|content |text   |	             |     |
|limit	 |date	 |               |     |
|status	 |string |	             |     |
|priority|string |	             |     |
|user_id |integer|belongs_to user|  ○  |

####3. Labelモデル

|column	   |type	 |association	  |index|
|----------|-------|--------------|-----|
|label_name|string |		          |     |
|task_id	 |integer|has_many tasks|	 ○  |
