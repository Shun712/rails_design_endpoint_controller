| やりたいこと                        | HTTPメソッド  | エンドポイント | コントローラ#アクション |
|:----------------------------------|------------:|:------------:|:-------------------:|
| ユーザー登録画面を表示する        	   | GET         | /users/new   |	users#new           |
| ユーザー登録をする                   | POST         | /users       | users#create        |
| ログイン画面を表示する                | GET         | /login | sessions#new 
| ログインする                        | POST         | /login       | sessions#create        |
| 質問一覧を表示する（全て）            | GET         | /questions       | questions#index        |
| 質問一覧を表示する（未解決）          | GET        | /questions?solved_check=false | questions#index |
| 質問一覧を表示する（解決済み）         | GET       | /questions?solved_check=true | questions#index |  
| 質問投稿ページを表示する              | GET        | /questions/new       | questions#new       |
| 質問投稿をする                      | POST         | /questions     | questions#create       |
| 質問詳細を表示する                   | GET         | /questions/:id       | questions#show        |
| 質問編集ページを表示する              | GET         | /questions/:id/edit    | questions#edit        |
| 質問を削除する                      | DELETE         | /questions/:id       | questions#destroy        |
| 回答する                           | POST         | /questions/:id/answers   | answers#create   |
| ユーザー一覧を表示する               | GET         | /users       | users#index        |
| 管理画面用のログインページを表示する    | GET         | /admin/login | admin/sessions#new       |
| （管理画面）質問一覧ページを表示する    | GET          | /admin/quesions       | admin/questions#index |
| （管理画面）質問を削除する            | DELETE        | /admin/questions/:id | admin/questions#destroy |
| （管理画面）ユーザー一覧ページを表示する| GET          | /admin/users       | admin/users#index |
| （管理画面）ユーザーを削除する         | DELETE         | admin/users/:id       | admin/users#destroy |
