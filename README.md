#ClientSideValidations

> 참고 : https://github.com/DavyJonesLocker/client_side_validations

- gem 설치

    `gem 'client_side_validations'`


- client_side_validations 설치

    `rails g client_side_validations:install`

    설치하면 `config/initializers/client_side_validations.rb` 가 생성된다.

-   이 후 `rails.validations.js`를 만들기 위해 아래 코드 실행

    `rails g client_side_validations:copy_assets`
    
- `rails.validations.js`를 만들었다면 `app/assets/javascripts/application.js`에 추가하기
    `//= require rails.validations`
    
-  사용할 form에서 아래처럼 validate를 ture로 설정하면 된다.

    `<%= form_for @user, validate: true do |f| %>`
